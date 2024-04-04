# Comparing `tmp/memfault_cli-1.0.8.tar.gz` & `tmp/memfault_cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memfault_cli-1.0.8.tar", max compression
+gzip compressed data, was "memfault_cli-1.0.9.tar", max compression
```

## Comparing `memfault_cli-1.0.8.tar` & `memfault_cli-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-02-16 20:37:58.164358 memfault_cli-1.0.8/LICENSE
--rw-r--r--   0        0        0     3853 2024-02-16 19:26:19.490627 memfault_cli-1.0.8/README.md
--rw-r--r--   0        0        0       79 2023-05-24 20:55:40.231321 memfault_cli-1.0.8/memfault_cli/__init__.py
--rw-r--r--   0        0        0      501 2024-02-06 15:53:34.991041 memfault_cli-1.0.8/memfault_cli/_version.py
--rw-r--r--   0        0        0     2576 2024-02-06 15:53:34.991133 memfault_cli-1.0.8/memfault_cli/authenticator.py
--rw-r--r--   0        0        0     3831 2024-02-06 15:53:34.991234 memfault_cli-1.0.8/memfault_cli/chunk.py
--rw-r--r--   0        0        0    30579 2024-02-06 21:29:43.754027 memfault_cli-1.0.8/memfault_cli/cli.py
--rw-r--r--   0        0        0     9820 2024-02-06 15:53:34.991510 memfault_cli-1.0.8/memfault_cli/console.py
--rw-r--r--   0        0        0    13134 2024-02-06 15:53:34.991666 memfault_cli-1.0.8/memfault_cli/context.py
--rw-r--r--   0        0        0     5122 2024-02-06 21:29:43.754272 memfault_cli-1.0.8/memfault_cli/deploy.py
--rw-r--r--   0        0        0     4126 2024-02-06 15:53:34.992054 memfault_cli-1.0.8/memfault_cli/elf.py
--rw-r--r--   0        0        0      633 2023-05-24 20:55:40.232247 memfault_cli-1.0.8/memfault_cli/functools_ext.py
--rw-r--r--   0        0        0     8990 2024-02-06 15:53:34.992188 memfault_cli-1.0.8/memfault_cli/linux.py
--rw-r--r--   0        0        0    27327 2024-02-06 15:53:34.992476 memfault_cli-1.0.8/memfault_cli/upload.py
--rw-r--r--   0        0        0     3356 2024-02-16 20:37:58.164487 memfault_cli-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     5186 1970-01-01 00:00:00.000000 memfault_cli-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 21:30:49.331248 memfault_cli-1.0.9/LICENSE
+-rw-r--r--   0        0        0     4035 2024-04-03 21:40:35.389663 memfault_cli-1.0.9/README.md
+-rw-r--r--   0        0        0       79 2023-10-05 20:24:51.463291 memfault_cli-1.0.9/memfault_cli/__init__.py
+-rw-r--r--   0        0        0      540 2024-04-03 21:40:35.389770 memfault_cli-1.0.9/memfault_cli/_version.py
+-rw-r--r--   0        0        0     2576 2023-10-05 20:24:51.463509 memfault_cli-1.0.9/memfault_cli/authenticator.py
+-rw-r--r--   0        0        0     3831 2024-01-31 04:15:08.403953 memfault_cli-1.0.9/memfault_cli/chunk.py
+-rw-r--r--   0        0        0    30579 2024-02-14 20:41:43.167723 memfault_cli-1.0.9/memfault_cli/cli.py
+-rw-r--r--   0        0        0    10368 2024-04-03 21:40:35.389900 memfault_cli-1.0.9/memfault_cli/console.py
+-rw-r--r--   0        0        0    13137 2024-04-03 21:40:35.390058 memfault_cli-1.0.9/memfault_cli/context.py
+-rw-r--r--   0        0        0     5122 2024-01-31 23:57:40.203269 memfault_cli-1.0.9/memfault_cli/deploy.py
+-rw-r--r--   0        0        0     4126 2024-01-31 04:15:08.406120 memfault_cli-1.0.9/memfault_cli/elf.py
+-rw-r--r--   0        0        0      633 2023-10-05 20:24:51.464356 memfault_cli-1.0.9/memfault_cli/functools_ext.py
+-rw-r--r--   0        0        0     8990 2024-01-31 04:15:08.406360 memfault_cli-1.0.9/memfault_cli/linux.py
+-rw-r--r--   0        0        0    27313 2024-04-03 21:40:35.390212 memfault_cli-1.0.9/memfault_cli/upload.py
+-rw-r--r--   0        0        0     3454 2024-04-03 21:58:30.949080 memfault_cli-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 memfault_cli-1.0.9/PKG-INFO
```

### Comparing `memfault_cli-1.0.8/LICENSE` & `memfault_cli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/README.md` & `memfault_cli-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,27 @@
 The purpose of the tool is to make integration with Memfault from other systems,
 like continuous integration servers, as easy as possible.
 
 Install the tool and run `memfault --help` for more info!
 
 ## Changes
 
+### [1.0.9] - 2024-03-11
+
+- Add Miniterm help text when launching the `memfault console` command, to
+  indicate how to exit the console (`Ctrl-]`).
+
+### 1.0.8
+
+- Add Apache 2 license
+
 ### 1.0.7
 
-- Fix bug when deactivating delta releases when multiple deployments match  
-  the filters.
+- Fix bug when deactivating delta releases when multiple deployments match the
+  filters.
 
 ### 1.0.6
 
 - Source pyelftools from https://github.com/memfault/pyelftools while we are
   waiting for 2 bugfixes to get merged upstream
   (https://github.com/eliben/pyelftools/pull/537 and
   https://github.com/eliben/pyelftools/pull/538).
```

### Comparing `memfault_cli-1.0.8/memfault_cli/authenticator.py` & `memfault_cli-1.0.9/memfault_cli/authenticator.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/memfault_cli/chunk.py` & `memfault_cli-1.0.9/memfault_cli/chunk.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/memfault_cli/cli.py` & `memfault_cli-1.0.9/memfault_cli/cli.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/memfault_cli/console.py` & `memfault_cli-1.0.9/memfault_cli/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
             super().start()
 
     @staticmethod
     def from_port(port: str, chunk_handler: MemfaultChunk, baudrate=115200) -> None:
         """
         Create and start a new instance of MemfaultMiniterm using the provided serial port.
 
-        Runs until KeyboardInterrupt received.
+        Runs until Miniterm is closed by the user.
 
         Args:
             port (str): String as a path or URL to create a Serial instance
             chunk_handler (MemfaultChunk): Handles sending chunks via Memfault /chunks API
             baudrate (int): Baudrate to use with underlying serial port
         """
         serial_instance = serial.serial_for_url(
@@ -246,14 +246,28 @@
             serial_instance,
             chunk_handler,
             echo=False,
             eol="crlf",
             filters=["default"],
         )
 
+        sys.stderr.write(
+            "\r\n--- Memfault Console on {p.name}  {p.baudrate},{p.bytesize},{p.parity},{p.stopbits} ---\n".format(
+                p=miniterm.serial
+            )
+        )
+        sys.stderr.write(
+            "--- Quit: {} | Menu: {} | Help: {} followed by {} ---\n".format(
+                key_description(miniterm.exit_character),
+                key_description(miniterm.menu_character),
+                key_description(miniterm.menu_character),
+                key_description("\x08"),
+            )
+        )
+
         miniterm.start()
         with contextlib.suppress(KeyboardInterrupt):
             miniterm.join(True)
 
         sys.stderr.write("\r\n--- Exiting Memfault Console ---\r\n")
         miniterm.join()
         miniterm.close()
```

### Comparing `memfault_cli-1.0.8/memfault_cli/context.py` & `memfault_cli-1.0.9/memfault_cli/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
     @property
     def android_apk_dir(self) -> Optional[str]:
         return self.obj.get("apk_dir")
 
     @property
     def extra_info(self) -> Optional[dict]:
-        extra_metadata: List[str] | None = self.obj.get("extra_metadata")
+        extra_metadata: Optional[List[str]] = self.obj.get("extra_metadata")
         if extra_metadata is None:
             return None
         else:
             try:
                 return dict(s.split("=", 1) for s in extra_metadata)
             except ValueError as error:
                 raise click.exceptions.UsageError(
```

### Comparing `memfault_cli-1.0.8/memfault_cli/deploy.py` & `memfault_cli-1.0.9/memfault_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/memfault_cli/elf.py` & `memfault_cli-1.0.9/memfault_cli/elf.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/memfault_cli/functools_ext.py` & `memfault_cli-1.0.9/memfault_cli/functools_ext.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/memfault_cli/linux.py` & `memfault_cli-1.0.9/memfault_cli/linux.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.8/memfault_cli/upload.py` & `memfault_cli-1.0.9/memfault_cli/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         )
 
 
 def url_quote(value: str) -> str:
     return urllib.parse.quote(value, safe="", encoding="utf-8")
 
 
-class Uploader(metaclass=abc.ABCMeta):
+class Uploader(abc.ABC):
     authenticator_types: Sequence[Type[Authenticator]]
 
     def __init__(
         self,
         *,
         ctx: MemfaultCliClickContext,
         file_path: Union[str, os.PathLike],
```

### Comparing `memfault_cli-1.0.8/pyproject.toml` & `memfault_cli-1.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "memfault-cli"
-version = "1.0.8"
+version = "1.0.9"
 description = "Memfault CLI tool"
 license = "Apache-2.0"
 homepage = "https://docs.memfault.com"
 documentation = "https://docs.memfault.com/docs/ci/install-memfault-cli"
 authors = ["Memfault Inc <hello@memfault.com>"]
 readme = "README.md"
 
@@ -30,14 +30,16 @@
 # dataclasses backport that supports Python 3.6
 dataclasses = { version = "0.8", python = "<3.7" }
 # extremely annoying, but we need a version of requests that's supported on
 # python3.6/3.7, and without pinning chardet, we end up with request spitting
 # out nuisance warning on 'chardet version unsupported'. so pin this to a
 # compatible version. this also forces us to be on an old tox version.
 chardet = "<5.0"
+# lxml 5.2.0 no longer supports Python 3.6. This is a dependency of pyaxmlparser.
+lxml = "<5.2.0"
 pyserial = "^3.5"
 
 [tool.poetry.dev-dependencies]
 faker = "^4"
 invoke = "^2"
 snappy = { path = "../../py-packages/snappy", develop = true }
 # pinning packaging and colorama (tox transitive deps) to exclude python 3.6 to
```

### Comparing `memfault_cli-1.0.8/PKG-INFO` & `memfault_cli-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: memfault-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Memfault CLI tool
 Home-page: https://docs.memfault.com
 License: Apache-2.0
 Author: Memfault Inc
 Author-email: hello@memfault.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Click (>=7,<9)
 Requires-Dist: chardet (<5.0)
 Requires-Dist: dataclasses (==0.8) ; python_version < "3.7"
 Requires-Dist: importlib-metadata (==4.8.3) ; python_version < "3.8"
+Requires-Dist: lxml (<5.2.0)
 Requires-Dist: mflt-build-id (>=1.0.1,<2.0.0)
 Requires-Dist: mflt-pyelftools (>=0.30.1,<0.31.0)
 Requires-Dist: more-itertools (>=8.0.2)
 Requires-Dist: pyaxmlparser (>=0.3.24,<0.4.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: tqdm (>=4.44.1,<5.0.0)
@@ -38,18 +38,27 @@
 The purpose of the tool is to make integration with Memfault from other systems,
 like continuous integration servers, as easy as possible.
 
 Install the tool and run `memfault --help` for more info!
 
 ## Changes
 
+### [1.0.9] - 2024-03-11
+
+- Add Miniterm help text when launching the `memfault console` command, to
+  indicate how to exit the console (`Ctrl-]`).
+
+### 1.0.8
+
+- Add Apache 2 license
+
 ### 1.0.7
 
-- Fix bug when deactivating delta releases when multiple deployments match  
-  the filters.
+- Fix bug when deactivating delta releases when multiple deployments match the
+  filters.
 
 ### 1.0.6
 
 - Source pyelftools from https://github.com/memfault/pyelftools while we are
   waiting for 2 bugfixes to get merged upstream
   (https://github.com/eliben/pyelftools/pull/537 and
   https://github.com/eliben/pyelftools/pull/538).
```

