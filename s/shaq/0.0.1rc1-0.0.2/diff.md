# Comparing `tmp/shaq-0.0.1rc1.tar.gz` & `tmp/shaq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaq-0.0.1rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shaq-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shaq-0.0.1rc1.tar` & `shaq-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0     1322 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/README.md
--rw-r--r--   0        0        0     1664 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0       25 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/shaq/__init__.py
--rw-r--r--   0        0        0       70 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/shaq/__main__.py
--rw-r--r--   0        0        0     5759 2023-07-14 01:07:46.706841 shaq-0.0.1rc1/shaq/_cli.py
--rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 shaq-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2024-04-04 02:18:27.776173 shaq-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1430 2024-04-04 02:18:27.776173 shaq-0.0.2/README.md
+-rw-r--r--   0        0        0     1608 2024-04-04 02:18:27.776173 shaq-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-04 02:18:27.776173 shaq-0.0.2/shaq/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-04 02:18:27.776173 shaq-0.0.2/shaq/__main__.py
+-rw-r--r--   0        0        0     6448 2024-04-04 02:18:27.776173 shaq-0.0.2/shaq/_cli.py
+-rw-r--r--   0        0        0     2659 1970-01-01 00:00:00.000000 shaq-0.0.2/PKG-INFO
```

### Comparing `shaq-0.0.1rc1/LICENSE` & `shaq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shaq-0.0.1rc1/README.md` & `shaq-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 If you run into installation errors, make sure that you have PortAudio
 installed. On Debian-based systems:
 
 ```bash
 sudo apt install -y portaudio19-dev
 ```
 
+`shaq` is also available on the Arch User Repository as [`shaq`](https://aur.archlinux.org/packages/shaq).
+
 ## Usage
 
 Detect by listening to the system microphone:
 
 ```bash
 # shaq listens for 10 seconds by default
 shaq --listen
```

### Comparing `shaq-0.0.1rc1/pyproject.toml` & `shaq-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Multimedia :: Sound/Audio :: Analysis",
 ]
 dependencies = [
     "pyaudio ~= 0.2.13",
     "pydub ~= 0.25.1",
     "rich ~= 13.4",
-    "shazamio ~= 0.4.0.1",
+    "shazamio >= 0.4.0.1,< 0.5.2.0",
 ]
 requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://pypi.org/project/shaq/"
 Issues = "https://github.com/woodruffw/shaq/issues"
 Source = "https://github.com/woodruffw/shaq"
 
 [project.scripts]
 shaq = "shaq._cli:main"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "pretend"]
-lint = ["black", "mypy", "ruff"]
+lint = ["mypy", "ruff"]
 dev = ["build", "shaq[test,lint]"]
 
 [tool.mypy]
 allow_redefinition = true
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
@@ -52,14 +52,10 @@
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-[tool.black]
-line-length = 100
-
 [tool.ruff]
 line-length = 100
 select = ["E", "F", "I", "W", "UP"]
-target-version = "py310"
```

### Comparing `shaq-0.0.1rc1/shaq/_cli.py` & `shaq-0.0.2/shaq/_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import asyncio
 import json
 import logging
 import os
+import shutil
 import sys
 import wave
 from collections.abc import Iterator
 from contextlib import contextmanager
 from io import BytesIO
 from pathlib import Path
 from typing import Any
@@ -128,14 +129,15 @@
         type=int,
         default=_DEFAULT_DURATION,
         help="only analyze the first SECS of the input (microphone or file)",
     )
     parser.add_argument(
         "-j", "--json", action="store_true", help="emit Shazam's response as JSON on stdout"
     )
+    parser.add_argument("--albumcover", action="store_true", help="return url to HD album cover")
 
     advanced_group = parser.add_argument_group(
         title="Advanced Options",
         description="Advanced users only: options to tweak recording, transcoding, etc. behavior.",
     )
     advanced_group.add_argument(
         "--chunk-size",
@@ -161,25 +163,37 @@
 
 def main() -> None:
     args = _parser().parse_args()
     with _console() as console:
         logger.addHandler(RichHandler(console=console))
         logger.debug(f"parsed {args=}")
 
+        if not shutil.which("ffmpeg"):
+            console.print("[red]Fatal: ffmpeg not found on $PATH[/red]")
+            sys.exit(1)
+
         try:
             raw = asyncio.run(_shaq(console, args))
             track = Serialize.full_track(raw)
         except KeyboardInterrupt:
             console.print("[red]Interrupted.[/red]")
+            sys.exit(2)
 
     if args.json:
         json.dump(raw, sys.stdout, indent=2)
     else:
         track = Serialize.full_track(raw)
         if not track.matches:
             print("No matches.")
         else:
             print(f"Track: {track.track.title}")
             print(f"Artist: {track.track.subtitle}")
+            if args.albumcover:
+                if "images" in raw["track"]:
+                    album_cover = raw["track"]["images"]["coverart"]
+                    # Forces the shazam image server to fetch a
+                    # high-resolution album cover.
+                    album_cover_hq = album_cover.replace("/400x400cc.jpg", "/1000x1000cc.png")
+                    print(f"Album Cover: {album_cover_hq}")
 
     if not track.matches:
         sys.exit(1)
```

### Comparing `shaq-0.0.1rc1/PKG-INFO` & `shaq-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: shaq
-Version: 0.0.1rc1
+Version: 0.0.2
 Summary: A bare-bones Shazam CLI client
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Requires-Dist: pyaudio ~= 0.2.13
 Requires-Dist: pydub ~= 0.25.1
 Requires-Dist: rich ~= 13.4
-Requires-Dist: shazamio ~= 0.4.0.1
+Requires-Dist: shazamio >= 0.4.0.1,< 0.5.2.0
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: shaq[test,lint] ; extra == "dev"
-Requires-Dist: black ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: ruff ; extra == "lint"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pretend ; extra == "test"
 Project-URL: Homepage, https://pypi.org/project/shaq/
 Project-URL: Issues, https://github.com/woodruffw/shaq/issues
@@ -52,14 +51,16 @@
 If you run into installation errors, make sure that you have PortAudio
 installed. On Debian-based systems:
 
 ```bash
 sudo apt install -y portaudio19-dev
 ```
 
+`shaq` is also available on the Arch User Repository as [`shaq`](https://aur.archlinux.org/packages/shaq).
+
 ## Usage
 
 Detect by listening to the system microphone:
 
 ```bash
 # shaq listens for 10 seconds by default
 shaq --listen
```

