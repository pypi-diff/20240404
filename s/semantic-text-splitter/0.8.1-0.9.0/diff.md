# Comparing `tmp/semantic_text_splitter-0.8.1.tar.gz` & `tmp/semantic_text_splitter-0.9.0.tar.gz`

## Comparing `semantic_text_splitter-0.8.1.tar` & `semantic_text_splitter-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0     1001      127       40 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/.gitignore
--rw-r--r--   0     1001      127    11027 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/CHANGELOG.md
--rw-r--r--   0     1001      127     5229 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1072 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/LICENSE.txt
--rw-r--r--   0     1001      127     9940 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/README.md
--rw-r--r--   0     1001      127     3891 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/benches/chunk_size.rs
--rw-r--r--   0     1001      127    55840 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/benches/output.txt
--rw-r--r--   0     1001      127      322 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/clippy.toml
--rw-r--r--   0     1001      127      952 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/src/chunk_size/characters.rs
--rw-r--r--   0     1001      127     2406 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/src/chunk_size/huggingface.rs
--rw-r--r--   0     1001      127     1300 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/src/chunk_size/tiktoken.rs
--rw-r--r--   0     1001      127    13100 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/src/chunk_size.rs
--rw-r--r--   0     1001      127    12856 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/src/lib.rs
--rw-r--r--   0     1001      127    38979 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/src/markdown.rs
--rw-r--r--   0     1001      127    18431 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/src/text.rs
--rw-r--r--   0     1001      127     4356 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/tests/markdown.rs
--rw-r--r--   0     1001      127     1960 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/tests/text_splitter.rs
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 semantic_text_splitter-0.8.1/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      718 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/bindings/python/.gitignore
--rw-r--r--   0     1001      127     2876 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127     6998 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/bindings/python/README.md
--rw-r--r--   0     1001      127    17938 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/bindings/python/semantic_text_splitter.pyi
--rw-r--r--   0     1001      127    26104 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127   711396 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/bindings/python/tests/bert-base-cased.json
--rw-r--r--   0     1001      127     5848 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/bindings/python/tests/test_integration.py
--rw-r--r--   0     1001      127    45501 2024-03-26 21:32:17.000000 semantic_text_splitter-0.8.1/Cargo.lock
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 semantic_text_splitter-0.8.1/Cargo.toml
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 semantic_text_splitter-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 semantic_text_splitter-0.8.1/PKG-INFO
+-rw-r--r--   0     1001      127       40 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/.gitignore
+-rw-r--r--   0     1001      127    12460 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     5229 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1072 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/LICENSE.txt
+-rw-r--r--   0     1001      127     9928 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/README.md
+-rw-r--r--   0     1001      127     3891 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/benches/chunk_size.rs
+-rw-r--r--   0     1001      127      322 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/clippy.toml
+-rw-r--r--   0     1001      127      952 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size/characters.rs
+-rw-r--r--   0     1001      127     2689 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size/huggingface.rs
+-rw-r--r--   0     1001      127     1300 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size/tiktoken.rs
+-rw-r--r--   0     1001      127    13100 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size.rs
+-rw-r--r--   0     1001      127    12856 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      127    38979 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/markdown.rs
+-rw-r--r--   0     1001      127    18431 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/text.rs
+-rw-r--r--   0     1001      127     4356 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/tests/markdown.rs
+-rw-r--r--   0     1001      127     2889 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/tests/text_splitter.rs
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      718 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/.gitignore
+-rw-r--r--   0     1001      127     2876 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127     6998 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/README.md
+-rw-r--r--   0     1001      127    17938 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/semantic_text_splitter.pyi
+-rw-r--r--   0     1001      127    26104 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127   711396 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/tests/bert-base-cased.json
+-rw-r--r--   0     1001      127     5848 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/tests/test_integration.py
+-rw-r--r--   0     1001      127    45485 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/Cargo.toml
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/PKG-INFO
```

### Comparing `semantic_text_splitter-0.8.1/CHANGELOG.md` & `semantic_text_splitter-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## v0.9.0
+
+### What's New
+
+[More robust handling of Hugging Face tokenizers as chunk sizers.](https://github.com/benbrandt/text-splitter/pull/131)
+
+- **Tokenizers with padding enabled no longer count padding tokens when generating chunks**. This caused some unexpected behavior, especially if the chunk capacity didn't perfectly line up with the padding size(s). Now, the tokenizer's padding token is ignored when counting the number of tokens generated in a chunk.
+- In the process, it also became clear there were some false assumptions about how the byte offset ranges were calculated for each token. This has been fixed, and the byte offset ranges should now be more accurate when determining the boundaries of each token. This only affects some optimizations in chunk sizing, and should not affect the actual chunk output.
+
+### Breaking Changes
+
+There should only be breaking chunk output for those of you using a Hugging Face tokenizer with padding enabled. Because padding tokens are no longer counted, the chunks will likely be larger than before, and closer to the desired behavior.
+
+**Note:** This will mean the generated chunks may also be larger than the chunk capacity when tokenized, because padding tokens will be added when you tokenize the chunk. The chunk capacity for these tokenizers reflects the number of tokens used in the text, not necessarily the number of tokens that the tokenizer will generate in total.
+
 ## v0.8.1
 
 ### What's New
 
 - Updates to documentation and examples.
 - Update pyo3 to 0.21.0 in Python package, which should bring some performance improvements.
```

### Comparing `semantic_text_splitter-0.8.1/CODE_OF_CONDUCT.md` & `semantic_text_splitter-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/LICENSE.txt` & `semantic_text_splitter-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/README.md` & `semantic_text_splitter-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,14 @@
 
 All of the above examples also can also work with Markdown text. If you enable the `markdown` feature, you can use the `MarkdownSplitter` in the same ways as the `TextSplitter`.
 
 ```sh
 cargo add text-splitter --features markdown
 ```
 
-</details>
-
 ```rust
 use text_splitter::MarkdownSplitter;
 // Maximum number of characters in a chunk. Can also use a range.
 let max_characters = 1000;
 // Default implementation uses character count for chunk size.
 // Can also use all of the same tokenizer implementations as `TextSplitter`.
 let splitter = MarkdownSplitter::default()
```

### Comparing `semantic_text_splitter-0.8.1/benches/chunk_size.rs` & `semantic_text_splitter-0.9.0/benches/chunk_size.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/src/chunk_size/characters.rs` & `semantic_text_splitter-0.9.0/src/chunk_size/characters.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/src/chunk_size/huggingface.rs` & `semantic_text_splitter-0.9.0/src/chunk_size/huggingface.rs`

 * *Files 25% similar despite different names*

```diff
@@ -9,35 +9,27 @@
     ///
     /// Will panic if you don't have a byte-level tokenizer and the splitter
     /// encounters text it can't tokenize.
     fn chunk_size(&self, chunk: &str, capacity: &impl ChunkCapacity) -> ChunkSize {
         let encoding = self
             .encode(chunk, false)
             .expect("Unable to tokenize the following string {chunk}");
-        let mut offsets = encoding
-            .get_offsets()
+
+        let pad_id = self.get_padding().map(|params| params.pad_id);
+
+        let offsets = encoding
+            .get_ids()
             .iter()
-            .map(|(start, end)| {
-                let end = *end + 1;
-                *start..end
-            })
-            .collect::<Vec<_>>();
-        // Sometimes the offsets are off by one because of whitespace prefixing
-        let prefixed = offsets.last().is_some_and(|r| r.end != chunk.len());
-
-        if prefixed {
-            for range in &mut offsets {
-                if range.start != 0 {
-                    range.start -= 1;
-                }
-                range.end -= 1;
-            }
-        }
+            .zip(encoding.get_offsets())
+            // Skip padding tokens at beginning and end so they don't count towards the chunk size
+            .skip_while(|&(id, _)| pad_id.map_or(false, |pad_id| id == &pad_id))
+            .take_while(|&(id, _)| pad_id.map_or(true, |pad_id| id != &pad_id))
+            .map(|(_, (start, end))| *start..*end);
 
-        ChunkSize::from_offsets(offsets.into_iter(), capacity)
+        ChunkSize::from_offsets(offsets, capacity)
     }
 }
 
 impl ChunkSizer for Tokenizer {
     /// Returns the number of tokens in a given text after tokenization.
     ///
     /// # Panics
@@ -56,23 +48,35 @@
     #[test]
     fn returns_offsets() {
         let tokenizer = Tokenizer::from_pretrained("bert-base-cased", None).unwrap();
         let capacity = 10;
         let offsets = tokenizer.chunk_size(" An apple a", &capacity);
         assert_eq!(
             offsets,
-            ChunkSize::from_offsets([0..3, 3..9, 9..11].into_iter(), &capacity)
+            ChunkSize::from_offsets([1..3, 4..9, 10..11].into_iter(), &capacity)
         );
     }
 
     #[test]
     fn returns_offsets_handles_prefix() {
-        let tokenizer = Tokenizer::from_pretrained("bert-base-cased", None).unwrap();
+        let tokenizer =
+            tokenizers::Tokenizer::from_file("./tests/tokenizers/huggingface.json").unwrap();
 
         let capacity = 10;
         let offsets = tokenizer.chunk_size("An apple a", &capacity);
         assert_eq!(
             offsets,
-            ChunkSize::from_offsets([0..2, 2..8, 8..10].into_iter(), &capacity)
+            ChunkSize::from_offsets([0..2, 3..8, 9..10].into_iter(), &capacity)
+        );
+    }
+
+    #[test]
+    fn handles_padding() {
+        let tokenizer = Tokenizer::from_pretrained("thenlper/gte-small", None).unwrap();
+        let capacity = 10;
+        let offsets = tokenizer.chunk_size("An apple a", &capacity);
+        assert_eq!(
+            offsets,
+            ChunkSize::from_offsets([0..2, 3..8, 9..10].into_iter(), &capacity)
         );
     }
 }
```

### Comparing `semantic_text_splitter-0.8.1/src/chunk_size/tiktoken.rs` & `semantic_text_splitter-0.9.0/src/chunk_size/tiktoken.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/src/chunk_size.rs` & `semantic_text_splitter-0.9.0/src/chunk_size.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/src/lib.rs` & `semantic_text_splitter-0.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/src/markdown.rs` & `semantic_text_splitter-0.9.0/src/markdown.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/src/text.rs` & `semantic_text_splitter-0.9.0/src/text.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/tests/markdown.rs` & `semantic_text_splitter-0.9.0/tests/markdown.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/tests/text_splitter.rs` & `semantic_text_splitter-0.9.0/tests/text_splitter.rs`

 * *Files 11% similar despite different names*

```diff
@@ -66,7 +66,39 @@
     let text = "12345\n12345";
     let splitter = TextSplitter::default();
     let chunks = splitter.chunks(text, 5..10).collect::<Vec<_>>();
 
     // \n goes in the second chunk because capacity is reached after first paragraph.
     assert_eq!(vec!["12345", "\n12345"], chunks);
 }
+
+#[cfg(feature = "tokenizers")]
+#[test]
+fn huggingface_small_chunk_behavior() {
+    let tokenizer =
+        tokenizers::Tokenizer::from_file("./tests/tokenizers/huggingface.json").unwrap();
+    let splitter = TextSplitter::new(tokenizer);
+
+    let text = "notokenexistsforthisword";
+    let chunks = splitter.chunks(text, 5).collect::<Vec<_>>();
+
+    assert_eq!(chunks, ["notokenexistsforth", "isword"]);
+}
+
+#[cfg(feature = "tokenizers")]
+#[test]
+fn huggingface_tokenizer_with_padding() {
+    let tokenizer = tokenizers::Tokenizer::from_pretrained("thenlper/gte-small", None).unwrap();
+    let splitter = TextSplitter::new(tokenizer);
+    let text = "\nThis is an example text This is an example text\n";
+
+    let chunks = splitter.chunks(text, 5).collect::<Vec<_>>();
+
+    assert_eq!(
+        chunks,
+        [
+            "\n",
+            "This is an example text ",
+            "This is an example text\n"
+        ]
+    );
+}
```

### Comparing `semantic_text_splitter-0.8.1/bindings/python/Cargo.toml` & `semantic_text_splitter-0.9.0/bindings/python/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "semantic_text_splitter"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.21.0", features = ["abi3-py38"] }
+pyo3 = { version = "0.21.1", features = ["abi3-py38"] }
 text-splitter = { path = "../..", features = [
     "markdown",
     "tiktoken-rs",
     "tokenizers",
 ] }
 tiktoken-rs = "0.5.8"
 tokenizers = { version = "0.15.2", default_features = false, features = [
```

### Comparing `semantic_text_splitter-0.8.1/bindings/python/.gitignore` & `semantic_text_splitter-0.9.0/bindings/python/.gitignore`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/bindings/python/CHANGELOG.md` & `semantic_text_splitter-0.9.0/bindings/python/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/bindings/python/README.md` & `semantic_text_splitter-0.9.0/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/bindings/python/semantic_text_splitter.pyi` & `semantic_text_splitter-0.9.0/bindings/python/semantic_text_splitter.pyi`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/bindings/python/src/lib.rs` & `semantic_text_splitter-0.9.0/bindings/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/bindings/python/tests/bert-base-cased.json` & `semantic_text_splitter-0.9.0/bindings/python/tests/bert-base-cased.json`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/bindings/python/tests/test_integration.py` & `semantic_text_splitter-0.9.0/bindings/python/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/Cargo.lock` & `semantic_text_splitter-0.9.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1899bfcfd9340ceea3533ea157360ba8fa864354eccbceab58e1006ecab35393"
 dependencies = [
  "derive_utils",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
@@ -287,15 +287,15 @@
 name = "derive_utils"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61bb5a1014ce6dfc2a378578509abe775a5aa06bff584a547555d9efdb81b926"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "deunicode"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6e854126756c496b8c81dec88f9a706b15b875c5849d4097a3854476b9fdf94"
@@ -339,15 +339,15 @@
 name = "divan-macros"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27540baf49be0d484d8f0130d7d8da3011c32a44d4fc873368154f1510e574a2"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
@@ -520,17 +520,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "insta"
-version = "1.37.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1718b3f2b85bb5054baf8ce406e36401f27c3169205f4175504c4b1d98252d3f"
+checksum = "3eab73f58e59ca6526037208f0e98851159ec1633cf17b6cd2e1f2c3fd5d53cc"
 dependencies = [
  "console",
  "globset",
  "lazy_static",
  "linked-hash-map",
  "serde",
  "similar",
@@ -580,21 +580,20 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
  "bitflags 2.5.0",
  "libc",
- "redox_syscall",
 ]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
@@ -635,17 +634,17 @@
 name = "macro_rules_attribute-proc_macro"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8dd856d451cc0da70e2ef2ce95a18e39a93b7558bedf10201ad28503f918568"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
@@ -681,15 +680,15 @@
 name = "monostate-impl"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f686d68a09079e63b1d2c64aa305095887ce50565f00a922ebfaeeee0d9ba6ce"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "more-asserts"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fafa6961cabd9c63bcd77a45d7e3b7f3b552b70417831fb0f56db717e72407e"
@@ -775,28 +774,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.101"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dda2b0f344e78efc2facf7d195d098df0dd72151b26ab98da807afc26c198dff"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -866,28 +865,28 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulldown-cmark"
-version = "0.10.0"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dce76ce678ffc8e5675b22aa1405de0b7037e2fdf8913fea40d1926c6fe1e6e7"
+checksum = "5f0530d13d87d1f549b66a3e8d0c688952abe5994e204ed62615baaf25dc029c"
 dependencies = [
  "bitflags 2.5.0",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a02a88a17e74cadbc8ce77855e1d6c8ad0ab82901a4a9b5046bd01c1c0bd95cd"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -895,55 +894,55 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5eb0b6ecba38961f6f4bd6cd5906dfab3cd426ff37b2eed5771006aa31656f1"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba8a6e48a29b5d22e4fdaf132d8ba8d3203ee9f06362d48f244346902a594ec3"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e80493c5965f94a747d0782a607b2328a4eea5391327b152b00e2f3b001cede"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcd7d86f42004025200e12a6a8119bd878329e6fddef8178eaafa4e4b5906c5b"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -1019,17 +1018,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
@@ -1113,17 +1112,17 @@
  "rustls-webpki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "868e20fada228fefaf6b652e00cc73623d54f8171e7352c18bb281571f2d92da"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.102.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
 dependencies = [
@@ -1160,38 +1159,38 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "security-framework"
-version = "2.9.2"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semantic-text-splitter"
-version = "0.8.1"
+version = "0.9.0"
 dependencies = [
  "pyo3",
  "text-splitter",
  "tiktoken-rs",
  "tokenizers",
 ]
 
@@ -1208,15 +1207,15 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
@@ -1224,17 +1223,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "similar"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32fea41aca09ee824cc9724996433064c89f7777e60762749a4170a14abbfa21"
+checksum = "fa42c91313f1d05da9b26f267f931cf178d4aba455b4c4622dd7355eb80c6640"
 
 [[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
@@ -1277,17 +1276,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.55"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1316,15 +1315,15 @@
 dependencies = [
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "text-splitter"
-version = "0.8.1"
+version = "0.9.0"
 dependencies = [
  "ahash",
  "auto_enums",
  "divan",
  "either",
  "fake",
  "insta",
@@ -1351,15 +1350,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tiktoken-rs"
 version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "40894b788eb28bbb7e36bdc8b7b1b1488b9c93fa3730f315ab965330c94c0842"
@@ -1733,15 +1732,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `semantic_text_splitter-0.8.1/Cargo.toml` & `semantic_text_splitter-0.9.0/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [workspace]
 members = ["bindings/*"]
 
 [workspace.package]
-version = "0.8.1"
+version = "0.9.0"
 authors = ["Ben Brandt <benjamin.j.brandt@gmail.com>"]
 edition = "2021"
 description = "Split text into semantic chunks, up to a desired chunk size. Supports calculating length by characters and tokens, and is callable from Rust and Python."
 repository = "https://github.com/benbrandt/text-splitter"
 license = "MIT"
 keywords = ["text", "split", "tokenizer", "nlp", "ai"]
 categories = ["text-processing"]
@@ -21,14 +21,15 @@
 license.workspace = true
 keywords.workspace = true
 categories.workspace = true
 exclude = [
     ".github/**",
     ".vscode/**",
     "/bindings/**",
+    "/benches/output.txt",
     # Rely on large test files
     "/tests/snapshots/**",
     "/tests/text_splitter_snapshots.rs",
     "/tests/inputs/**",
     "/tests/tokenizers/**",
     "*.yml",
     "*.yaml",
@@ -43,26 +44,26 @@
 
 [dependencies]
 ahash = "0.8.11"
 auto_enums = "0.8.5"
 either = "1.10.0"
 itertools = "0.12.1"
 once_cell = "1.19.0"
-pulldown-cmark = { version = "0.10.0", default-features = false, optional = true }
+pulldown-cmark = { version = "0.10.2", default-features = false, optional = true }
 regex = "1.10.4"
 tiktoken-rs = { version = "0.5.8", optional = true }
 tokenizers = { version = "0.15.2", default_features = false, features = [
     "onig",
 ], optional = true }
 unicode-segmentation = "1.11.0"
 
 [dev-dependencies]
 divan = "0.1.14"
 fake = "2.9.2"
-insta = { version = "1.37.0", features = ["glob", "yaml"] }
+insta = { version = "1.38.0", features = ["glob", "yaml"] }
 more-asserts = "0.3.1"
 tokenizers = { version = "0.15.2", default-features = false, features = [
     "onig",
     "http",
 ] }
 
 [[bench]]
```

### Comparing `semantic_text_splitter-0.8.1/pyproject.toml` & `semantic_text_splitter-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.8.1/PKG-INFO` & `semantic_text_splitter-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: semantic-text-splitter
-Version: 0.8.1
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: black ; extra == 'test'
 Requires-Dist: tokenizers ; extra == 'test'
 Requires-Dist: pdoc ; extra == 'docs'
```

