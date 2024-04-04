# Comparing `tmp/undertext-0.2.0.tar.gz` & `tmp/undertext-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undertext-0.2.0.tar", last modified: Wed Apr  3 13:17:31 2024, max compression
+gzip compressed data, was "undertext-0.3.0.tar", last modified: Thu Apr  4 08:34:54 2024, max compression
```

## Comparing `undertext-0.2.0.tar` & `undertext-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.422301 undertext-0.2.0/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1074 2024-04-03 12:04:43.000000 undertext-0.2.0/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3741 2024-04-03 13:17:31.422301 undertext-0.2.0/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2393 2024-04-03 12:04:43.000000 undertext-0.2.0/README.md
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-03 12:04:43.000000 undertext-0.2.0/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-03 13:17:31.422301 undertext-0.2.0/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1917 2024-04-03 12:04:43.000000 undertext-0.2.0/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.410301 undertext-0.2.0/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.414301 undertext-0.2.0/src/undertext/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1216 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/__cli__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1663 2024-04-03 13:17:26.000000 undertext-0.2.0/src/undertext/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2538 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/__main__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      189 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/exceptions.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.418301 undertext-0.2.0/src/undertext/readers/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1105 2024-04-03 12:12:36.000000 undertext-0.2.0/src/undertext/readers/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1262 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/readers/microdvd.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1295 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/readers/subrip.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1003 2024-04-03 12:23:11.000000 undertext-0.2.0/src/undertext/readers/subviewer.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2684 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/readers/webvtt.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.418301 undertext-0.2.0/src/undertext/structures/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       86 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/structures/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2497 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/structures/caption.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.418301 undertext-0.2.0/src/undertext/util/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       53 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/util/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2396 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/util/time.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.422301 undertext-0.2.0/src/undertext/writers/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1165 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      942 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/microdvd.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      768 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/subrip.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      827 2024-04-03 12:23:11.000000 undertext-0.2.0/src/undertext/writers/subviewer.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1455 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/webvtt.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.422301 undertext-0.2.0/src/undertext.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3741 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      835 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       54 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/entry_points.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        7 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.946942 undertext-0.3.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1074 2024-04-03 12:04:43.000000 undertext-0.3.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3903 2024-04-04 08:34:54.942942 undertext-0.3.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2555 2024-04-04 08:15:53.000000 undertext-0.3.0/README.md
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-03 12:04:43.000000 undertext-0.3.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-04 08:34:54.946942 undertext-0.3.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1917 2024-04-03 12:04:43.000000 undertext-0.3.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.918942 undertext-0.3.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.922942 undertext-0.3.0/src/undertext/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1216 2024-04-03 12:04:43.000000 undertext-0.3.0/src/undertext/__cli__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1697 2024-04-04 08:34:40.000000 undertext-0.3.0/src/undertext/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2538 2024-04-03 12:04:43.000000 undertext-0.3.0/src/undertext/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      189 2024-04-03 12:04:43.000000 undertext-0.3.0/src/undertext/exceptions.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      376 2024-04-04 07:40:36.000000 undertext-0.3.0/src/undertext/extra.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.926942 undertext-0.3.0/src/undertext/readers/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1105 2024-04-03 12:12:36.000000 undertext-0.3.0/src/undertext/readers/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1262 2024-04-03 12:04:43.000000 undertext-0.3.0/src/undertext/readers/microdvd.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1295 2024-04-03 12:04:43.000000 undertext-0.3.0/src/undertext/readers/subrip.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1003 2024-04-03 12:23:11.000000 undertext-0.3.0/src/undertext/readers/subviewer.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2537 2024-04-04 07:17:45.000000 undertext-0.3.0/src/undertext/readers/webvtt.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.930942 undertext-0.3.0/src/undertext/structures/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       86 2024-04-03 12:04:43.000000 undertext-0.3.0/src/undertext/structures/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3115 2024-04-04 07:40:04.000000 undertext-0.3.0/src/undertext/structures/caption.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.930942 undertext-0.3.0/src/undertext/util/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       76 2024-04-04 07:26:13.000000 undertext-0.3.0/src/undertext/util/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      620 2024-04-04 07:26:04.000000 undertext-0.3.0/src/undertext/util/cleanup.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2396 2024-04-03 12:04:43.000000 undertext-0.3.0/src/undertext/util/time.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.934942 undertext-0.3.0/src/undertext/writers/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1169 2024-04-04 07:51:07.000000 undertext-0.3.0/src/undertext/writers/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      946 2024-04-04 07:51:07.000000 undertext-0.3.0/src/undertext/writers/microdvd.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      772 2024-04-04 07:51:07.000000 undertext-0.3.0/src/undertext/writers/subrip.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      831 2024-04-04 07:51:07.000000 undertext-0.3.0/src/undertext/writers/subviewer.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1244 2024-04-04 07:51:07.000000 undertext-0.3.0/src/undertext/writers/webvtt.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-04 08:34:54.942942 undertext-0.3.0/src/undertext.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3903 2024-04-04 08:34:54.000000 undertext-0.3.0/src/undertext.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      888 2024-04-04 08:34:54.000000 undertext-0.3.0/src/undertext.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-04 08:34:54.000000 undertext-0.3.0/src/undertext.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       54 2024-04-04 08:34:54.000000 undertext-0.3.0/src/undertext.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        7 2024-04-04 08:34:54.000000 undertext-0.3.0/src/undertext.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2024-04-04 08:34:54.000000 undertext-0.3.0/src/undertext.egg-info/top_level.txt
```

### Comparing `undertext-0.2.0/LICENSE` & `undertext-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/PKG-INFO` & `undertext-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undertext
-Version: 0.2.0
+Version: 0.3.0
 Summary: library to load, edit and save different formats of subtitles
 Home-page: https://github.com/utility-libraries/undertext-py
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-libraries
 Project-URL: Homepage, https://github.com/utility-libraries/undertext-py/
 Project-URL: Documentation, https://utility-libraries.github.io/undertext-py/
@@ -50,25 +50,33 @@
 
 ```shell
 pip3 install undertext
 ```
 
 ## File Formats
 
-| ext    | name                      | read  | write |
-|--------|---------------------------|-------|-------|
-| `.ass` | Advanced SubStation Alpha | ❌     | ❌     |
-| `.sbv` | SubViewer                 | ❌     | ✅     |
-| `.srt` | SubRip                    | ✅     | ✅     |
-| `.ssa` | Sub Station Alpha         | ❌     | ❌     |
-| `.sub` | MicroDVD                  | ✅     | ✅     |
-| `.vtt` | WebVTT                    | ✅     | ✅     |
+| ext    | name                      | read  | write | Flags |
+|--------|---------------------------|-------|-------|-------|
+| `.ass` | Advanced SubStation Alpha | ❌     | ❌     | TT    |
+| `.sbv` | SubViewer                 | ✅     | ✅     | TT    |
+| `.srt` | SubRip                    | ✅     | ✅     | TT    |
+| `.ssa` | Sub Station Alpha         | ❌     | ❌     | TT    |
+| `.sub` | MicroDVD                  | ✅     | ✅     | TF    |
+| `.vtt` | WebVTT                    | ✅     | ✅     | TT    |
 
 <small>Listed formats that are currently unsupported may be added at a later version</small>
 
+Flag Information:
+```text
+T. = Text Based
+B. = Bitmap Based
+.T = Time-Based
+.F = Frame-Based
+```
+
 ## Examples
 
 ```python
 import undertext
 
 captions = undertext.loads("example.en.srt")
 undertext.dumps(captions, "example.en.vtt")
```

### Comparing `undertext-0.2.0/README.md` & `undertext-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,25 +19,33 @@
 
 ```shell
 pip3 install undertext
 ```
 
 ## File Formats
 
-| ext    | name                      | read  | write |
-|--------|---------------------------|-------|-------|
-| `.ass` | Advanced SubStation Alpha | ❌     | ❌     |
-| `.sbv` | SubViewer                 | ❌     | ✅     |
-| `.srt` | SubRip                    | ✅     | ✅     |
-| `.ssa` | Sub Station Alpha         | ❌     | ❌     |
-| `.sub` | MicroDVD                  | ✅     | ✅     |
-| `.vtt` | WebVTT                    | ✅     | ✅     |
+| ext    | name                      | read  | write | Flags |
+|--------|---------------------------|-------|-------|-------|
+| `.ass` | Advanced SubStation Alpha | ❌     | ❌     | TT    |
+| `.sbv` | SubViewer                 | ✅     | ✅     | TT    |
+| `.srt` | SubRip                    | ✅     | ✅     | TT    |
+| `.ssa` | Sub Station Alpha         | ❌     | ❌     | TT    |
+| `.sub` | MicroDVD                  | ✅     | ✅     | TF    |
+| `.vtt` | WebVTT                    | ✅     | ✅     | TT    |
 
 <small>Listed formats that are currently unsupported may be added at a later version</small>
 
+Flag Information:
+```text
+T. = Text Based
+B. = Bitmap Based
+.T = Time-Based
+.F = Frame-Based
+```
+
 ## Examples
 
 ```python
 import undertext
 
 captions = undertext.loads("example.en.srt")
 undertext.dumps(captions, "example.en.vtt")
```

### Comparing `undertext-0.2.0/setup.py` & `undertext-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/__cli__.py` & `undertext-0.3.0/src/undertext/__cli__.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/__init__.py` & `undertext-0.3.0/src/undertext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 __copyright__ = "Copyright 2024, utility-libraries"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "library to load, edit and save different formats of subtitles"
-__version_info__ = (0, 2, 0)
+__version_info__ = (0, 3, 0)
 __version__ = '.'.join(str(_) for _ in __version_info__)
 
 from .exceptions import *
 from .structures import *
 from . import readers, writers
 from .readers import loads
 from .writers import dumps
+from .extra import clean_captions
```

### Comparing `undertext-0.2.0/src/undertext/__main__.py` & `undertext-0.3.0/src/undertext/__main__.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/readers/__init__.py` & `undertext-0.3.0/src/undertext/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/readers/microdvd.py` & `undertext-0.3.0/src/undertext/readers/microdvd.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/readers/subrip.py` & `undertext-0.3.0/src/undertext/readers/subrip.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/readers/subviewer.py` & `undertext-0.3.0/src/undertext/readers/subviewer.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/readers/webvtt.py` & `undertext-0.3.0/src/undertext/readers/webvtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,14 @@
                 style: str = match.group("style")
 
                 if style is not None:
                     for style in style.split():
                         key, sep, value = style.partition(":")
                         if sep is None:
                             raise FormatException(f"Bad style format ({style})")
-                        if key not in {"line", "position", "size", "align"}:
-                            raise KeyError(f"Invalid style: {key!r}")
                         styles[key] = value
 
                 text_lines = []
                 for text_line in lines:
                     if not text_line:
                         break
                     if text_line.startswith("- "):  # multiline
```

### Comparing `undertext-0.2.0/src/undertext/structures/caption.py` & `undertext-0.3.0/src/undertext/structures/caption.py`

 * *Files 21% similar despite different names*

```diff
@@ -68,33 +68,45 @@
         return self._lines
 
     @lines.setter
     def lines(self, lines: T_LINES) -> None:
         self._lines.clear()
         self._lines.extend(lines)
 
+    def with_lines(self, lines: T_LINES) -> 'Caption':
+        return Caption(start=self.start, end=self.end, text=lines, id=self.id, styles=self.styles)
+
     @property
     def text(self) -> str:
         return "\n".join(self.lines)
 
     @text.setter
     def text(self, value: T_TEXT) -> None:
         if isinstance(value, str):
             self.lines = value.splitlines(keepends=False)
         else:
             self.lines = value
 
+    def with_text(self, text: T_TEXT) -> 'Caption':
+        return Caption(start=self.start, end=self.end, text=text, id=self.id, styles=self.styles)
+
     @property
     def id(self) -> t.Optional[str]:
         return self._id
 
     @id.setter
     def id(self, value: t.Optional[str]) -> None:
         self._id = value if value is None else str(value)
 
+    def with_id(self, id: t.Optional[str]) -> 'Caption':
+        return Caption(start=self.start, end=self.end, text=self.text, id=id, styles=self.styles)
+
     @property
     def styles(self) -> t.Optional[T_STYLE]:
         return self._styles
 
     @styles.setter
     def styles(self, value: t.Optional[T_STYLE]) -> None:
         self._styles = value
+
+    def with_styles(self, styles: T_STYLE) -> 'Caption':
+        return Caption(start=self.start, end=self.end, text=self.text, id=self.id, styles=styles)
```

### Comparing `undertext-0.2.0/src/undertext/util/time.py` & `undertext-0.3.0/src/undertext/util/time.py`

 * *Files identical despite different names*

### Comparing `undertext-0.2.0/src/undertext/writers/__init__.py` & `undertext-0.3.0/src/undertext/writers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     microdvd=write_microdvd,
     subrip=write_subrip,
     subviewer=write_subviewer,
     webvtt=write_webvtt,
 )
 
 
-def dumps(captions: t.List[Caption], fp: t.Union[str, PathLike], fmt: str = None, **kwargs) -> None:
+def dumps(captions: t.Iterable[Caption], fp: t.Union[str, PathLike], fmt: str = None, **kwargs) -> None:
     r"""
     dumps some captions into a file
 
     :param captions: captions to dump
     :param fp: subtitle file to dump into
     :param fmt: specific format name
     :param kwargs: optional arguments some formats may need
```

### Comparing `undertext-0.2.0/src/undertext/writers/microdvd.py` & `undertext-0.3.0/src/undertext/writers/microdvd.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import warnings
 import typing as t
 from os import PathLike
 from ..structures import Caption
 
 
-def write_microdvd(captions: t.List[Caption], filename: t.Union[str, PathLike, t.TextIO], fps: int = None) -> None:
+def write_microdvd(captions: t.Iterable[Caption], filename: t.Union[str, PathLike, t.TextIO], fps: int = None) -> None:
     stream = io.StringIO()
 
     if fps is None:
         warnings.warn("Missing fps specification for reading MicroDVD.\n"
                       "MicroDVD works with frames instead of timestamps. "
                       "Specify fps to convert frames to timestamps or set to 1 to keep.", RuntimeWarning)
         fps = 1
```

### Comparing `undertext-0.2.0/src/undertext/writers/subrip.py` & `undertext-0.3.0/src/undertext/writers/subrip.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import typing as t
 from os import PathLike
 from ..structures import Caption
 from ..util import format_ts_comma as format_ts
 
 
-def write_subrip(captions: t.List[Caption], filename: t.Union[str, PathLike, t.TextIO]) -> None:
+def write_subrip(captions: t.Iterable[Caption], filename: t.Union[str, PathLike, t.TextIO]) -> None:
     stream = io.StringIO()
 
     for i, caption in enumerate(captions):
         if i != 0:
             stream.write("\r\n")
 
         stream.write(f"{i+1}\r\n")
```

### Comparing `undertext-0.2.0/src/undertext/writers/subviewer.py` & `undertext-0.3.0/src/undertext/writers/subviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import typing as t
 from os import PathLike
 from ..structures import Caption
 from ..util import format_ts_dot as format_ts
 
 
-def write_subviewer(captions: t.List[Caption], filename: t.Union[str, PathLike, t.TextIO]) -> None:
+def write_subviewer(captions: t.Iterable[Caption], filename: t.Union[str, PathLike, t.TextIO]) -> None:
     r"""
     writes as SubViewer 2.0
     https://wiki.videolan.org/SubViewer/
     """
     stream = io.StringIO()
 
     for i, caption in enumerate(captions):
```

### Comparing `undertext-0.2.0/src/undertext/writers/webvtt.py` & `undertext-0.3.0/src/undertext/writers/webvtt.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import typing as t
 from os import PathLike
 from ..structures import Caption
 from ..util import format_ts_dot as format_ts
 
 
-def write_webvtt(captions: t.List[Caption], filename: t.Union[str, PathLike, t.TextIO],
+def write_webvtt(captions: t.Iterable[Caption], filename: t.Union[str, PathLike, t.TextIO],
                  header: str = None) -> None:
     stream = io.StringIO()
 
     stream.write("WEBVTT")
     if header is not None:
         stream.write(f" - {header}")
     stream.write("\r\n")
@@ -22,18 +22,15 @@
         stream.write("\r\n")
         if caption.id:
             stream.write(f"{caption.id}\r\n")
         stream.write(f"{format_ts(caption.start)} --> {format_ts(caption.end)}")
         if caption.styles:
             stream.write(" ")
             for key, value in caption.styles.items():
-                if key in {"line", "position", "size", "align"}:
-                    stream.write(f"{key}:{value}")  # todo: cleanup of style values
-                # else:  # don't raise. maybe "bad" style comes from other format
-                #     raise KeyError(f"Unknown style: {key!r}")
+                stream.write(f"{key}:{value}")  # todo: cleanup of style values
         stream.write("\r\n")
         if len(caption.lines) == 1:
             stream.write(f"{caption.text}\r\n")
         else:
             for line in caption.lines:
                 stream.write(f"- {line}\r\n")
```

### Comparing `undertext-0.2.0/src/undertext.egg-info/PKG-INFO` & `undertext-0.3.0/src/undertext.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undertext
-Version: 0.2.0
+Version: 0.3.0
 Summary: library to load, edit and save different formats of subtitles
 Home-page: https://github.com/utility-libraries/undertext-py
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-libraries
 Project-URL: Homepage, https://github.com/utility-libraries/undertext-py/
 Project-URL: Documentation, https://utility-libraries.github.io/undertext-py/
@@ -50,25 +50,33 @@
 
 ```shell
 pip3 install undertext
 ```
 
 ## File Formats
 
-| ext    | name                      | read  | write |
-|--------|---------------------------|-------|-------|
-| `.ass` | Advanced SubStation Alpha | ❌     | ❌     |
-| `.sbv` | SubViewer                 | ❌     | ✅     |
-| `.srt` | SubRip                    | ✅     | ✅     |
-| `.ssa` | Sub Station Alpha         | ❌     | ❌     |
-| `.sub` | MicroDVD                  | ✅     | ✅     |
-| `.vtt` | WebVTT                    | ✅     | ✅     |
+| ext    | name                      | read  | write | Flags |
+|--------|---------------------------|-------|-------|-------|
+| `.ass` | Advanced SubStation Alpha | ❌     | ❌     | TT    |
+| `.sbv` | SubViewer                 | ✅     | ✅     | TT    |
+| `.srt` | SubRip                    | ✅     | ✅     | TT    |
+| `.ssa` | Sub Station Alpha         | ❌     | ❌     | TT    |
+| `.sub` | MicroDVD                  | ✅     | ✅     | TF    |
+| `.vtt` | WebVTT                    | ✅     | ✅     | TT    |
 
 <small>Listed formats that are currently unsupported may be added at a later version</small>
 
+Flag Information:
+```text
+T. = Text Based
+B. = Bitmap Based
+.T = Time-Based
+.F = Frame-Based
+```
+
 ## Examples
 
 ```python
 import undertext
 
 captions = undertext.loads("example.en.srt")
 undertext.dumps(captions, "example.en.vtt")
```

### Comparing `undertext-0.2.0/src/undertext.egg-info/SOURCES.txt` & `undertext-0.3.0/src/undertext.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 README.md
 pyproject.toml
 setup.py
 src/undertext/__cli__.py
 src/undertext/__init__.py
 src/undertext/__main__.py
 src/undertext/exceptions.py
+src/undertext/extra.py
 src/undertext.egg-info/PKG-INFO
 src/undertext.egg-info/SOURCES.txt
 src/undertext.egg-info/dependency_links.txt
 src/undertext.egg-info/entry_points.txt
 src/undertext.egg-info/requires.txt
 src/undertext.egg-info/top_level.txt
 src/undertext/readers/__init__.py
 src/undertext/readers/microdvd.py
 src/undertext/readers/subrip.py
 src/undertext/readers/subviewer.py
 src/undertext/readers/webvtt.py
 src/undertext/structures/__init__.py
 src/undertext/structures/caption.py
 src/undertext/util/__init__.py
+src/undertext/util/cleanup.py
 src/undertext/util/time.py
 src/undertext/writers/__init__.py
 src/undertext/writers/microdvd.py
 src/undertext/writers/subrip.py
 src/undertext/writers/subviewer.py
 src/undertext/writers/webvtt.py
```

