# Comparing `tmp/uwuify-1.3.0.tar.gz` & `tmp/uwuify-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwuify-1.3.0.tar", max compression
+gzip compressed data, was "uwuify-1.3.1.tar", max compression
```

## Comparing `uwuify-1.3.0.tar` & `uwuify-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2022-12-02 20:13:29.436187 uwuify-1.3.0/LICENSE
--rw-r--r--   0        0        0     1046 2023-05-16 06:25:18.470758 uwuify-1.3.0/README.md
--rw-r--r--   0        0        0      546 2023-05-16 07:29:22.233729 uwuify-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      222 2023-05-16 07:29:33.987253 uwuify-1.3.0/uwuify/__init__.py
--rw-r--r--   0        0        0       73 2023-05-16 07:27:24.981830 uwuify-1.3.0/uwuify/__main__.py
--rw-r--r--   0        0        0     1040 2023-05-16 07:27:24.981830 uwuify-1.3.0/uwuify/cli.py
--rw-r--r--   0        0        0     3066 2023-05-16 07:27:24.981830 uwuify-1.3.0/uwuify/core.py
--rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 uwuify-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-10-03 15:34:20.000641 uwuify-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1046 2023-10-03 15:34:20.000641 uwuify-1.3.1/README.md
+-rw-r--r--   0        0        0      545 2024-04-04 13:44:20.057638 uwuify-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-10-03 15:34:20.001641 uwuify-1.3.1/uwuify/__init__.py
+-rw-r--r--   0        0        0       71 2023-11-24 02:00:14.390477 uwuify-1.3.1/uwuify/__main__.py
+-rw-r--r--   0        0        0     1066 2023-11-24 02:00:14.388477 uwuify-1.3.1/uwuify/cli.py
+-rw-r--r--   0        0        0     3103 2024-04-04 13:43:43.335262 uwuify-1.3.1/uwuify/core.py
+-rw-r--r--   0        0        0     1703 1970-01-01 00:00:00.000000 uwuify-1.3.1/PKG-INFO
```

### Comparing `uwuify-1.3.0/LICENSE` & `uwuify-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uwuify-1.3.0/README.md` & `uwuify-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `uwuify-1.3.0/pyproject.toml` & `uwuify-1.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "uwuify"
-version = "1.3.0"
+version = "1.3.1"
 description = "uwuifys text"
 authors = ["StarrFox <starrfox6312@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/StarrFox/uwuify"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-click = "^8.0.1"
+python = "^3.8"
+click = "^8.1.7"
 
 [tool.poetry.scripts]
 uwuify = "uwuify.cli:main"
 
 [tool.poetry.group.tests.dependencies]
-pytest = "^7.3.1"
-
+pytest = "^8.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-mypy = "^1.3.0"
+black = "^24.0.0"
+mypy = "^1.7.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uwuify-1.3.0/uwuify/cli.py` & `uwuify-1.3.1/uwuify/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-from uwuify import SMILEY, YU, uwu, STUTTER, NOUWU
+from uwuify import NOUWU, SMILEY, STUTTER, YU, UwuifyFlag, uwu
 
 
 def allow_pipe(ctx, param, value):
     if not value and not click.get_text_stream("stdin").isatty():
         pipped = click.get_text_stream("stdin").read().strip()
         return pipped.split(" ")  # Compatibility with -1 garbage
     else:
@@ -17,15 +17,15 @@
 @click.option(
     "--stutter", help="Add stutter for every 4-th word.", is_flag=True, type=int
 )
 @click.option("--nouwu", is_flag=True, help="Disable uwuification.")
 @click.argument("text", nargs=-1, callback=allow_pipe)
 def main(smiley, yu, text, stutter, nouwu):
     text = " ".join(text)
-    flags = 0
+    flags = UwuifyFlag.NONE
 
     if smiley:
         flags |= SMILEY
 
     if yu:
         flags |= YU
```

### Comparing `uwuify-1.3.0/uwuify/core.py` & `uwuify-1.3.1/uwuify/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import random
 import re
 from enum import IntFlag
-from typing import Union
+from typing import List, Union
 
 
 class UwuifyFlag(IntFlag):
     NONE = 0
     SMILEY = 1
     YU = 2
     STUTTER = 4
@@ -75,21 +76,16 @@
 def _do_uwu(entry: str) -> str:
     regexed = ER_REPLACE.sub(r"\g<1>a", entry)
     translated = regexed.translate(UWU)
     return translated
 
 
 def _do_smiley(entry: str) -> str:
-    if not isinstance(entry, list):
-        entry_split = entry.split(" ")
-
-    import random
-
-    final = []
-    for word in entry_split:
+    final: List[str] = []
+    for word in entry.split(" "):
         if word.endswith((".", "?", "!")):
             final.append(word + " " + random.choice(SMILEYS))
 
         else:
             final.append(word)
 
     return " ".join(final)
@@ -97,29 +93,31 @@
 
 def _do_stutter(entry: str, stutter_every_nth_word: int = 4) -> str:
     if stutter_every_nth_word < 1:
         raise ValueError(
             f"stutter_every_nth_word must be above 0; passed {stutter_every_nth_word}"
         )
 
-    listofstr = entry.split(" ")
+    listofstr = re.split(r"(\s+)", entry)
     result = []
-    for index, word in enumerate(listofstr):
-        if index % stutter_every_nth_word == 0:
-            result.append("{}-{}{}".format(word[0], word[0], word[1:]))
-        else:
-            result.append(word)
-    return " ".join(result)
+    words_since_last_stutter = 0
+    for word in listofstr:
+        if word != "" and not word.isspace():
+            if words_since_last_stutter % stutter_every_nth_word == 0:
+                word = "{}-{}".format(word[0], word)
+            words_since_last_stutter += 1
+        result.append(word)
+    return "".join(result)
 
 
 def uwu(entry: Union[list, str], *, flags: UwuifyFlag = UwuifyFlag.NONE) -> str:
     if isinstance(entry, list):
         entry = " ".join(entry)
 
-    if len(entry) == 0:  # Maybe this should error??
+    if len(entry) == 0:  # Maybe this should error?
         return entry
 
     if flags & UwuifyFlag.YU:
         entry = _do_yu(entry)
 
     if not flags & UwuifyFlag.NOUWU:
         entry = _do_uwu(entry)
```

### Comparing `uwuify-1.3.0/PKG-INFO` & `uwuify-1.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: uwuify
-Version: 1.3.0
+Version: 1.3.1
 Summary: uwuifys text
 Home-page: https://github.com/StarrFox/uwuify
 License: MIT
 Author: StarrFox
 Author-email: starrfox6312@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: click (>=8.0.1,<9.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Project-URL: Repository, https://github.com/StarrFox/uwuify
 Description-Content-Type: text/markdown
 
 # uwuify
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/uwuify?style=for-the-badge)
```

