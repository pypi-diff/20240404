# Comparing `tmp/dotlocalslashbin-0.0.1.tar.gz` & `tmp/dotlocalslashbin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotlocalslashbin-0.0.1.tar", last modified: Thu Apr  4 06:43:58 2024, max compression
+gzip compressed data, was "dotlocalslashbin-0.0.2.tar", last modified: Thu Apr  4 07:35:12 2024, max compression
```

## Comparing `dotlocalslashbin-0.0.1.tar` & `dotlocalslashbin-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    16727 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      223 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/src/
--rwxr-xr-x   0 root         (0) root         (0)     5559 2024-04-04 06:43:58.000000 dotlocalslashbin-0.0.1/src/dotlocalslashbin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    16727 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)      879 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      223 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/src/
+-rwxr-xr-x   0 root         (0) root         (0)     5579 2024-04-04 07:35:12.000000 dotlocalslashbin-0.0.2/src/dotlocalslashbin.py
```

### Comparing `dotlocalslashbin-0.0.1/LICENSES/MPL-2.0.txt` & `dotlocalslashbin-0.0.2/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `dotlocalslashbin-0.0.1/PKG-INFO` & `dotlocalslashbin-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: dotlocalslashbin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Download and extract files to ~/.local/bin/
 Author-email: Keith Maxwell <keith.maxwell@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Dist: black ; extra == "test"
+Requires-Dist: codespell ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
 Requires-Dist: flit ; extra == "test"
 Requires-Dist: nox ; extra == "test"
+Requires-Dist: usort ; extra == "test"
 Project-URL: Home, https://github.com/maxwell-k/dotlocalslashbin/
 Provides-Extra: test
 
 Download and extract files to ~/.local/bin/
 
 <!--
 .flake8
```

### Comparing `dotlocalslashbin-0.0.1/pyproject.toml` & `dotlocalslashbin-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,23 @@
   "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 license = { file = "LICENSES/MPL-2.0.txt" }
 
 [project.urls]
 Home = "https://github.com/maxwell-k/dotlocalslashbin/"
 
+[project.scripts]
+dotlocalslashbin = "dotlocalslashbin:main"
+
 [project.optional-dependencies]
 test = [
   "black",
+  "codespell",
   "flake8",
   "flit",
   "nox",
+  "usort",
 ]
 
 # pyproject.toml
 # SPDX-FileCopyrightText: 2024 Keith Maxwell <keith.maxwell@gmail.com>
 # SPDX-License-Identifier: CC0-1.0
```

### Comparing `dotlocalslashbin-0.0.1/src/dotlocalslashbin.py` & `dotlocalslashbin-0.0.2/src/dotlocalslashbin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 #!/usr/bin/env python3
 # src/dotlocalslashbin.py
 # Copyright 2022 Keith Maxwell
 # SPDX-License-Identifier: MPL-2.0
 """Download and extract files to ~/.local/bin/"""
 import tarfile
-from argparse import ArgumentDefaultsHelpFormatter as formatter_class
-from argparse import ArgumentParser
-from argparse import Namespace
+from argparse import (
+    ArgumentDefaultsHelpFormatter as formatter_class,
+    ArgumentParser,
+    Namespace,
+)
 from collections.abc import Generator
 from contextlib import contextmanager
 from hashlib import file_digest
 from pathlib import Path
 from shlex import split
 from shutil import copy
 from stat import S_IEXEC
 from subprocess import run
 from tomllib import load
 from typing import cast
 from urllib.request import urlopen
 from zipfile import ZipFile
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 @contextmanager
 def _download(
     args: Namespace,
     *,
     name: str,
@@ -51,15 +53,15 @@
         completions: whether to generate ZSH completions
         command: command to run to install after download
     """
     if target is None:
         target = cast(str, args.output) + name
 
     if url.startswith("https://"):
-        downloaded = Path(args.downloaded) / url.rsplit("/", 1)[1]
+        downloaded = Path(args.downloaded).expanduser() / url.rsplit("/", 1)[1]
         downloaded.parent.mkdir(parents=True, exist_ok=True)
         if not downloaded.is_file():
             with urlopen(url) as fp, downloaded.open("wb") as dp:
                 if "content-length" in fp.headers:
                     size = int(fp.headers["Content-Length"])
                 else:
                     size = -1
@@ -141,15 +143,17 @@
 
 
 def main() -> int:
     parser = ArgumentParser(prog=Path(__file__).name, formatter_class=formatter_class)
     parser.add_argument("--version", action="version", version=__version__)
     parser.add_argument("--input", default="bin.toml", help="TOML specification")
     parser.add_argument("--output", default="~/.local/bin/", help="Target directory")
-    parser.add_argument("--downloaded", default="downloaded", help="Download directory")
+    parser.add_argument(
+        "--downloaded", default="~/.cache/dotlocalslashbin/", help="Download directory"
+    )
     parser.add_argument(
         "--completions",
         default="~/.local/share/zsh/site-functions/",
         help="Directory for ZSH completions",
     )
     args = parser.parse_args()
```

