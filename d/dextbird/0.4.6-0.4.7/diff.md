# Comparing `tmp/dextbird-0.4.6.tar.gz` & `tmp/dextbird-0.4.7.tar.gz`

## Comparing `dextbird-0.4.6.tar` & `dextbird-0.4.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 dextbird-0.4.6/Cargo.toml
--rw-r--r--   0     1001      127      387 2024-04-03 22:13:09.000000 dextbird-0.4.6/.bashrc
--rw-r--r--   0     1001      127     1367 2024-04-03 22:13:09.000000 dextbird-0.4.6/.github/workflows/docs.yml
--rw-r--r--   0     1001      127     1940 2024-04-03 22:13:09.000000 dextbird-0.4.6/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1025 2024-04-03 22:13:09.000000 dextbird-0.4.6/.github/workflows/test.yml
--rw-r--r--   0     1001      127      713 2024-04-03 22:13:09.000000 dextbird-0.4.6/.gitignore
--rw-r--r--   0     1001      127     1065 2024-04-03 22:13:09.000000 dextbird-0.4.6/LICENSE
--rw-r--r--   0     1001      127     1392 2024-04-03 22:13:09.000000 dextbird-0.4.6/README.md
--rw-r--r--   0     1001      127       67 2024-04-03 22:13:09.000000 dextbird-0.4.6/dextbird/__init__.py
--rw-r--r--   0     1001      127     1326 2024-04-03 22:13:09.000000 dextbird-0.4.6/dextbird/core.pyi
--rw-r--r--   0     1001      127      759 2024-04-03 22:13:09.000000 dextbird-0.4.6/dextbird/plug.py
--rw-r--r--   0     1001      127     2662 2024-04-03 22:13:09.000000 dextbird-0.4.6/dextbird/voice_client.py
--rw-r--r--   0     1001      127     1310 2024-04-03 22:13:09.000000 dextbird-0.4.6/examples/basic.py
--rw-r--r--   0     1001      127      107 2024-04-03 22:13:09.000000 dextbird-0.4.6/renovate.json
--rw-r--r--   0     1001      127 15660281 2024-04-03 22:13:09.000000 dextbird-0.4.6/result.txt
--rw-r--r--   0     1001      127     7151 2024-04-03 22:13:09.000000 dextbird-0.4.6/src/core.rs
--rw-r--r--   0     1001      127      320 2024-04-03 22:13:09.000000 dextbird-0.4.6/src/lib.rs
--rw-r--r--   0     1001      127     2376 2024-04-03 22:13:09.000000 dextbird-0.4.6/src/track.rs
--rw-r--r--   0     1001      127     1401 2024-04-03 22:13:09.000000 dextbird-0.4.6/src/update_voice_state.rs
--rw-r--r--   0     1001      127       49 2024-04-03 22:13:09.000000 dextbird-0.4.6/test.sh
--rw-r--r--   0     1001      127     1434 2024-04-03 22:13:09.000000 dextbird-0.4.6/tests/test_simple.py
--rw-r--r--   0     1001      127    73821 2024-04-03 22:13:12.000000 dextbird-0.4.6/Cargo.lock
--rw-r--r--   0     1001      127      814 2024-04-03 22:13:09.000000 dextbird-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 dextbird-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 dextbird-0.4.7/Cargo.toml
+-rw-r--r--   0     1001      127      387 2024-04-03 22:31:30.000000 dextbird-0.4.7/.bashrc
+-rw-r--r--   0     1001      127     1367 2024-04-03 22:31:30.000000 dextbird-0.4.7/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127     2030 2024-04-03 22:31:30.000000 dextbird-0.4.7/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1025 2024-04-03 22:31:30.000000 dextbird-0.4.7/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      713 2024-04-03 22:31:30.000000 dextbird-0.4.7/.gitignore
+-rw-r--r--   0     1001      127     1065 2024-04-03 22:31:30.000000 dextbird-0.4.7/LICENSE
+-rw-r--r--   0     1001      127     1392 2024-04-03 22:31:30.000000 dextbird-0.4.7/README.md
+-rw-r--r--   0     1001      127       67 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/__init__.py
+-rw-r--r--   0     1001      127     1326 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/core.pyi
+-rw-r--r--   0     1001      127      759 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/plug.py
+-rw-r--r--   0     1001      127     2662 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/voice_client.py
+-rw-r--r--   0     1001      127     1310 2024-04-03 22:31:30.000000 dextbird-0.4.7/examples/basic.py
+-rw-r--r--   0     1001      127      107 2024-04-03 22:31:30.000000 dextbird-0.4.7/renovate.json
+-rw-r--r--   0     1001      127 15660281 2024-04-03 22:31:30.000000 dextbird-0.4.7/result.txt
+-rw-r--r--   0     1001      127     7151 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/core.rs
+-rw-r--r--   0     1001      127      320 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/lib.rs
+-rw-r--r--   0     1001      127     2376 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/track.rs
+-rw-r--r--   0     1001      127     1401 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/update_voice_state.rs
+-rw-r--r--   0     1001      127       49 2024-04-03 22:31:30.000000 dextbird-0.4.7/test.sh
+-rw-r--r--   0     1001      127     1434 2024-04-03 22:31:30.000000 dextbird-0.4.7/tests/test_simple.py
+-rw-r--r--   0     1001      127    73821 2024-04-03 22:31:39.000000 dextbird-0.4.7/Cargo.lock
+-rw-r--r--   0     1001      127      814 2024-04-03 22:31:30.000000 dextbird-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 dextbird-0.4.7/PKG-INFO
```

### Comparing `dextbird-0.4.6/Cargo.toml` & `dextbird-0.4.7/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dextbird"
-version = "0.4.6"
+version = "0.4.7"
 description = "Discord extensions voice library made with rust"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "dextbird"
 crate-type = ["cdylib"]
```

### Comparing `dextbird-0.4.6/.github/workflows/docs.yml` & `dextbird-0.4.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/.github/workflows/release.yml` & `dextbird-0.4.7/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,45 +28,46 @@
       run: pip3 install maturin[patchelf]
     - name: Install musl-tools
       if: "matrix.target == 'x86_64-unknown-linux-musl'"
       run: sudo apt-get update && sudo apt-get install musl-tools
     - name: Build library
       run: maturin build -r -o dist --target=${{ matrix.target }}
     - name: Upload wheels
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: wheels
+        name: wheels-${{ matrix.python-version }}-${{ matrix.target }}
         path: dist
 
   sdist:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
       with:
         python-version: "3.11"
     - name: Install maturin
       run: pip3 install maturin
     - name: Build sdist
       run: maturin sdist -o dist
     - name: Upload sdist
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: wheels
+        name: wheels-sdist
         path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [ build, sdist ]
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
       with:
-        name: wheels
+        pattern: wheels-*
+        merge-multiple: true
     - name: Release
       uses: softprops/action-gh-release@v2
       if: startsWith(github.ref, 'refs/tags/')
       with:
         files: "*"
     - name: Publish to PyPI
       uses: PyO3/maturin-action@v1
```

### Comparing `dextbird-0.4.6/.github/workflows/test.yml` & `dextbird-0.4.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/.gitignore` & `dextbird-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/LICENSE` & `dextbird-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/README.md` & `dextbird-0.4.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
 If you are using linux, we are only support this python version.
 3.8.10+, 3.9.5+, 3.10.0+
 
 ### Why I am not supporting windows?
 It's too hard for me.
 
-## install
+## Install
 ```sh
 pip install "dextbird @ git+https://github.com/tuna2134/discord-ext-songbird.git"
 ```
 
-## sample code
+## Sample code
 ```python
 from dextbird import VoiceClient
 import discord
 
 import os
 import logging
```

### Comparing `dextbird-0.4.6/dextbird/core.pyi` & `dextbird-0.4.7/dextbird/core.pyi`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/dextbird/plug.py` & `dextbird-0.4.7/dextbird/plug.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/dextbird/voice_client.py` & `dextbird-0.4.7/dextbird/voice_client.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/examples/basic.py` & `dextbird-0.4.7/examples/basic.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/result.txt` & `dextbird-0.4.7/result.txt`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/src/core.rs` & `dextbird-0.4.7/src/core.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/src/track.rs` & `dextbird-0.4.7/src/track.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/src/update_voice_state.rs` & `dextbird-0.4.7/src/update_voice_state.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/tests/test_simple.py` & `dextbird-0.4.7/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/Cargo.lock` & `dextbird-0.4.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dextbird"
-version = "0.4.6"
+version = "0.4.7"
 dependencies = [
  "async-dropper",
  "async-trait",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "reqwest",
```

### Comparing `dextbird-0.4.6/pyproject.toml` & `dextbird-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.6/PKG-INFO` & `dextbird-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dextbird
-Version: 0.4.6
+Version: 0.4.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Discord extensions voice library made with rust
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -23,20 +23,20 @@
 
 If you are using linux, we are only support this python version.
 3.8.10+, 3.9.5+, 3.10.0+
 
 ### Why I am not supporting windows?
 It's too hard for me.
 
-## install
+## Install
 ```sh
 pip install "dextbird @ git+https://github.com/tuna2134/discord-ext-songbird.git"
 ```
 
-## sample code
+## Sample code
 ```python
 from dextbird import VoiceClient
 import discord
 
 import os
 import logging
```

