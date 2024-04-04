# Comparing `tmp/dextbird-0.4.7.tar.gz` & `tmp/dextbird-0.4.8.tar.gz`

## Comparing `dextbird-0.4.7.tar` & `dextbird-0.4.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 dextbird-0.4.7/Cargo.toml
--rw-r--r--   0     1001      127      387 2024-04-03 22:31:30.000000 dextbird-0.4.7/.bashrc
--rw-r--r--   0     1001      127     1367 2024-04-03 22:31:30.000000 dextbird-0.4.7/.github/workflows/docs.yml
--rw-r--r--   0     1001      127     2030 2024-04-03 22:31:30.000000 dextbird-0.4.7/.github/workflows/release.yml
--rw-r--r--   0     1001      127     1025 2024-04-03 22:31:30.000000 dextbird-0.4.7/.github/workflows/test.yml
--rw-r--r--   0     1001      127      713 2024-04-03 22:31:30.000000 dextbird-0.4.7/.gitignore
--rw-r--r--   0     1001      127     1065 2024-04-03 22:31:30.000000 dextbird-0.4.7/LICENSE
--rw-r--r--   0     1001      127     1392 2024-04-03 22:31:30.000000 dextbird-0.4.7/README.md
--rw-r--r--   0     1001      127       67 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/__init__.py
--rw-r--r--   0     1001      127     1326 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/core.pyi
--rw-r--r--   0     1001      127      759 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/plug.py
--rw-r--r--   0     1001      127     2662 2024-04-03 22:31:30.000000 dextbird-0.4.7/dextbird/voice_client.py
--rw-r--r--   0     1001      127     1310 2024-04-03 22:31:30.000000 dextbird-0.4.7/examples/basic.py
--rw-r--r--   0     1001      127      107 2024-04-03 22:31:30.000000 dextbird-0.4.7/renovate.json
--rw-r--r--   0     1001      127 15660281 2024-04-03 22:31:30.000000 dextbird-0.4.7/result.txt
--rw-r--r--   0     1001      127     7151 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/core.rs
--rw-r--r--   0     1001      127      320 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/lib.rs
--rw-r--r--   0     1001      127     2376 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/track.rs
--rw-r--r--   0     1001      127     1401 2024-04-03 22:31:30.000000 dextbird-0.4.7/src/update_voice_state.rs
--rw-r--r--   0     1001      127       49 2024-04-03 22:31:30.000000 dextbird-0.4.7/test.sh
--rw-r--r--   0     1001      127     1434 2024-04-03 22:31:30.000000 dextbird-0.4.7/tests/test_simple.py
--rw-r--r--   0     1001      127    73821 2024-04-03 22:31:39.000000 dextbird-0.4.7/Cargo.lock
--rw-r--r--   0     1001      127      814 2024-04-03 22:31:30.000000 dextbird-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 dextbird-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 dextbird-0.4.8/Cargo.toml
+-rw-r--r--   0     1001      127      387 2024-04-04 18:18:24.000000 dextbird-0.4.8/.bashrc
+-rw-r--r--   0     1001      127     1367 2024-04-04 18:18:24.000000 dextbird-0.4.8/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127     2030 2024-04-04 18:18:24.000000 dextbird-0.4.8/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1025 2024-04-04 18:18:24.000000 dextbird-0.4.8/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      713 2024-04-04 18:18:24.000000 dextbird-0.4.8/.gitignore
+-rw-r--r--   0     1001      127     1065 2024-04-04 18:18:24.000000 dextbird-0.4.8/LICENSE
+-rw-r--r--   0     1001      127     1392 2024-04-04 18:18:24.000000 dextbird-0.4.8/README.md
+-rw-r--r--   0     1001      127       67 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/__init__.py
+-rw-r--r--   0     1001      127     1314 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/core.pyi
+-rw-r--r--   0     1001      127      759 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/plug.py
+-rw-r--r--   0     1001      127     2633 2024-04-04 18:18:24.000000 dextbird-0.4.8/dextbird/voice_client.py
+-rw-r--r--   0     1001      127     1310 2024-04-04 18:18:24.000000 dextbird-0.4.8/examples/basic.py
+-rw-r--r--   0     1001      127      107 2024-04-04 18:18:24.000000 dextbird-0.4.8/renovate.json
+-rw-r--r--   0     1001      127 15660281 2024-04-04 18:18:24.000000 dextbird-0.4.8/result.txt
+-rw-r--r--   0     1001      127     7151 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/core.rs
+-rw-r--r--   0     1001      127      320 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/lib.rs
+-rw-r--r--   0     1001      127     2376 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/track.rs
+-rw-r--r--   0     1001      127     1401 2024-04-04 18:18:24.000000 dextbird-0.4.8/src/update_voice_state.rs
+-rw-r--r--   0     1001      127       49 2024-04-04 18:18:24.000000 dextbird-0.4.8/test.sh
+-rw-r--r--   0     1001      127     1561 2024-04-04 18:18:24.000000 dextbird-0.4.8/tests/test_simple.py
+-rw-r--r--   0     1001      127    73821 2024-04-04 18:18:28.000000 dextbird-0.4.8/Cargo.lock
+-rw-r--r--   0     1001      127      814 2024-04-04 18:18:24.000000 dextbird-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 dextbird-0.4.8/PKG-INFO
```

### Comparing `dextbird-0.4.7/Cargo.toml` & `dextbird-0.4.8/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dextbird"
-version = "0.4.7"
+version = "0.4.8"
 description = "Discord extensions voice library made with rust"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "dextbird"
 crate-type = ["cdylib"]
```

### Comparing `dextbird-0.4.7/.github/workflows/docs.yml` & `dextbird-0.4.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/.github/workflows/release.yml` & `dextbird-0.4.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/.github/workflows/test.yml` & `dextbird-0.4.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/.gitignore` & `dextbird-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/LICENSE` & `dextbird-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/README.md` & `dextbird-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/dextbird/core.pyi` & `dextbird-0.4.8/dextbird/core.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     async def update_state(self, session_id: str, channel_id: Optional[str]) -> None:
         "Update state"
 
     async def ytdl(self, url: str) -> Track:
         "Play youtube video's mp3"
 
-    def source(self, data: bytes, opus: bool) -> Track:
+    def source(self, data: bytes) -> Track:
         "Play bytes data"
 
     async def deafen(self, deaf: bool) -> None:
         "Deaf bot"
 
     async def mute(self, mute: bool) -> None:
         "Mute bot"
```

### Comparing `dextbird-0.4.7/dextbird/plug.py` & `dextbird-0.4.8/dextbird/plug.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/dextbird/voice_client.py` & `dextbird-0.4.8/dextbird/voice_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,24 +56,24 @@
         Parameters
         ----------
         url : str
             YouTube video url
         """
         return await self._core.ytdl(url)
 
-    def source(self, data: bytes, *, opus: bool = False) -> Track:
+    def source(self, data: bytes) -> Track:
         """
         Play music from bytes
 
         Parameters
         ----------
         data : bytes
             Voice data
         """
-        return self._core.source(data, opus)
+        return self._core.source(data)
 
     def stop(self) -> None:
         "Stop to play music"
         self._core.stop()
 
     async def disconnect(self, *args) -> None:
         "Disconnect from voice channel"
```

### Comparing `dextbird-0.4.7/examples/basic.py` & `dextbird-0.4.8/examples/basic.py`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/result.txt` & `dextbird-0.4.8/result.txt`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/src/core.rs` & `dextbird-0.4.8/src/core.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/src/track.rs` & `dextbird-0.4.8/src/track.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/src/update_voice_state.rs` & `dextbird-0.4.8/src/update_voice_state.rs`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/tests/test_simple.py` & `dextbird-0.4.8/tests/test_simple.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,22 @@
     pass
 else:
     dotenv.load_dotenv()
 
 import asyncio
 import os
 import logging
+import random
+
+
+MUSICS = [
+    "https://youtu.be/fE9trKOuT3Q",
+    "https://youtu.be/TG2IgWOjtwU",
+    "https://youtu.be/yL1LYf-S2Q0"
+]
 
 
 client = discord.Client(intents=discord.Intents.all())
 logger = logging.getLogger()
 
 
 @pytest.mark.asyncio
@@ -31,15 +39,15 @@
 
         def after():
             logger.info("Finished to play music")
             wait_finished.set()
 
         await vc.deafen(True)
         logging.info("Deafen")
-        track = await vc.ytdl("https://youtu.be/fE9trKOuT3Q")
+        track = await vc.ytdl(random.choice(MUSICS))
         logging.info("Play youtube")
         track.after(after)
         track.play()
         logger.info("Waiting to finish some music")
         try:
             await asyncio.wait_for(wait_finished.wait(), timeout=60 * 5)
         except asyncio.TimeoutError:
```

### Comparing `dextbird-0.4.7/Cargo.lock` & `dextbird-0.4.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dextbird"
-version = "0.4.7"
+version = "0.4.8"
 dependencies = [
  "async-dropper",
  "async-trait",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "reqwest",
```

### Comparing `dextbird-0.4.7/pyproject.toml` & `dextbird-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dextbird-0.4.7/PKG-INFO` & `dextbird-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dextbird
-Version: 0.4.7
+Version: 0.4.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Discord extensions voice library made with rust
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

