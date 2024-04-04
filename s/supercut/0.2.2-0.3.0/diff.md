# Comparing `tmp/supercut-0.2.2.tar.gz` & `tmp/supercut-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supercut-0.2.2.tar", max compression
+gzip compressed data, was "supercut-0.3.0.tar", max compression
```

## Comparing `supercut-0.2.2.tar` & `supercut-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-03-29 20:04:59.080839 supercut-0.2.2/LICENSE
--rw-r--r--   0        0        0     5222 2024-03-29 20:04:59.080839 supercut-0.2.2/README.md
--rw-r--r--   0        0        0     1241 2024-03-29 20:04:59.084840 supercut-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-29 20:04:59.084840 supercut-0.2.2/src/supercut/__init__.py
--rw-r--r--   0        0        0     5661 2024-03-29 20:04:59.084840 supercut-0.2.2/src/supercut/ffmpeg.py
--rw-r--r--   0        0        0     1204 2024-03-29 20:04:59.084840 supercut-0.2.2/src/supercut/subtitles.py
--rw-r--r--   0        0        0    14571 2024-03-29 20:04:59.084840 supercut-0.2.2/src/supercut/supercut.py
--rw-r--r--   0        0        0     2447 2024-03-29 20:04:59.084840 supercut-0.2.2/src/supercut/vlc.py
--rw-r--r--   0        0        0     5880 1970-01-01 00:00:00.000000 supercut-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-04 09:14:15.049523 supercut-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5222 2024-04-04 09:14:15.049523 supercut-0.3.0/README.md
+-rw-r--r--   0        0        0     1241 2024-04-04 09:14:15.049523 supercut-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/__init__.py
+-rw-r--r--   0        0        0    10503 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/ffmpeg.py
+-rw-r--r--   0        0        0     1442 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/subtitles.py
+-rw-r--r--   0        0        0    15398 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/supercut.py
+-rw-r--r--   0        0        0     2447 2024-04-04 09:14:15.049523 supercut-0.3.0/src/supercut/vlc.py
+-rw-r--r--   0        0        0     5880 1970-01-01 00:00:00.000000 supercut-0.3.0/PKG-INFO
```

### Comparing `supercut-0.2.2/LICENSE` & `supercut-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `supercut-0.2.2/README.md` & `supercut-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `supercut-0.2.2/pyproject.toml` & `supercut-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supercut"
-version = "0.2.2"
+version = "0.3.0"
 description = "Subtitle-based automatic supercut creation"
 authors = ["Tamir Bahar"]
 license = "MIT"
 readme = "README.md"
 
 
 [build-system]
```

### Comparing `supercut-0.2.2/src/supercut/subtitles.py` & `supercut-0.3.0/src/supercut/subtitles.py`

 * *Files 24% similar despite different names*

```diff
@@ -37,8 +37,13 @@
 
 
 def get_external_subs(video: Path, language: str = "eng") -> pysubs2.SSAFile:
     subs_path = find_srt_subs_for(video, language=language)
     if not subs_path:
         raise RuntimeError(f"Failed to find subs for {video}")
 
-    return pysubs2.load(str(subs_path))
+    subs = pysubs2.load(str(subs_path))
+    # Use 16 as font size because that's the default size for ffmpeg.
+    # As a result, when ffmpeg converts the subs back to .srt
+    # later it won't add a `<font>` tag to them.
+    subs.styles["Default"].fontsize = 16
+    return subs
```

### Comparing `supercut-0.2.2/src/supercut/supercut.py` & `supercut-0.3.0/src/supercut/supercut.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import io
 import operator
 import sys
 import typing
 from collections import defaultdict
-from concurrent.futures import ThreadPoolExecutor
 from copy import deepcopy
 from pathlib import Path
 from typing import Optional
 
 import attrs
 import diskcache  # type: ignore[import-untyped]
 import more_itertools
 import pysubs2  # type: ignore[import-untyped]
 import rich.console
+import rich.progress
 import rich.table
 import typer
 
 from supercut import ffmpeg, vlc
 from supercut.subtitles import get_external_subs
 
 app = typer.Typer(
@@ -24,14 +24,17 @@
     pretty_exceptions_show_locals=False,
 )
 edit_app = typer.Typer(
     help="Editable supercut generation", pretty_exceptions_show_locals=False
 )
 app.add_typer(edit_app, name="edit")
 
+util_app = typer.Typer(help="Utility commands", pretty_exceptions_show_locals=False)
+app.add_typer(util_app, name="util")
+
 
 @attrs.define
 class Core:
     _cache: diskcache.Cache
     _external_subs: bool
 
     @classmethod
@@ -138,25 +141,36 @@
 ):
     """
     Quick preview using VLC
     """
     videos = sorted(videos)
     playlists = []
     with Core.from_dir(cache_dir, external_subs=external_subs) as core:
-        with ThreadPoolExecutor() as executor:
-            subs = executor.map(lambda video: core.get_subs(video, language), videos)
-        for video, subs in zip(videos, subs):
+        all_subs = get_all_subs(videos, core, language)
+        for video, subs in zip(videos, all_subs):
             sections = get_sections(subs, query=query, name=name)
             playlist = vlc.create_supercut_playlist(video, sections)
             playlists.append(playlist)
 
         full_playlist = "\n".join(playlists)
         vlc.view_playlist(full_playlist)
 
 
+def get_all_subs(
+    videos: list[Path], core: Core, language: str
+) -> list[pysubs2.SSAFile]:
+    subs = []
+    with rich.progress.Progress() as progress:
+        task = progress.add_task("Getting subtitles", total=len(videos))
+        for video in videos:
+            subs.append(core.get_subs(video, language))
+            progress.advance(task)
+    return list(subs)
+
+
 @app.command()
 def render(
     videos: typing.Annotated[
         list[Path], typer.Argument(help="The videos to supercut, in order.")
     ],
     query: typing.Annotated[str, typer.Option(help="String to search in subtitles")],
     output: typing.Annotated[Path, typer.Option(help="Ouptut file")],
@@ -176,16 +190,16 @@
 ):
     """
     Render supercut
     """
     videos = sorted(videos)
     with Core.from_dir(cache_dir, external_subs=external_subs) as core:
         video_parts = []
-        for video in videos:
-            subs = core.get_subs(video, language)
+        all_subs = get_all_subs(videos, core, language)
+        for video, subs in zip(videos, all_subs):
             events = query_events(subs, query, name=name)
             for event in events:
                 part = ffmpeg.VideoPart(
                     video=video,
                     subs=trim_subs(subs, event.start, event.end).to_string("ass"),
                     start=event.start,
                     end=event.end,
@@ -214,17 +228,17 @@
     external_subs: typing.Annotated[
         bool, typer.Option(help="Search for external subs.")
     ] = False,
 ):
     """Show all subs that match the query and name"""
     videos = sorted(videos)
     with Core.from_dir(cache_dir, external_subs=external_subs) as core:
+        all_subs = get_all_subs(videos, core, language)
         events = more_itertools.flatten(
-            query_events(core.get_subs(video, language), query, name=name)
-            for video in videos
+            query_events(subs, query, name=name) for subs in all_subs
         )
 
     for i, event in enumerate(events):
         text = event.plaintext.replace("\n", " ").replace("  ", " ")
         print(f"{i:-4} | {event.name}: {text}")
 
 
@@ -247,16 +261,16 @@
         bool, typer.Option(help="Search for external subs.")
     ] = False,
 ):
     """Show all speaker names in the subtitles"""
     names: defaultdict[str, int] = defaultdict(int)
 
     with Core.from_dir(cache_dir, external_subs=external_subs) as core:
-        for video in videos:
-            subs = core.get_subs(video, language)
+        all_subs = get_all_subs(videos, core, language)
+        for subs in all_subs:
             events = query_events(subs, query)
             for event in events:
                 names[event.name] += 1
 
     print_names(names)
 
 
@@ -295,17 +309,17 @@
     ] = False,
 ):
     """
     Create edit list
     """
     videos = sorted(videos)
     with Core.from_dir(cache_dir, external_subs=external_subs) as core:
+        all_subs = get_all_subs(videos, core, language)
         events = more_itertools.flatten(
-            query_events(core.get_subs(video, language), query, name=name)
-            for video in videos
+            query_events(subs, query, name=name) for subs in all_subs
         )
 
     list_text = io.StringIO()
     for i, event in enumerate(events):
         text = event.plaintext.replace("\n", " ").replace("  ", " ")
         print(f"{i:-4} | {event.name}: {text}", file=list_text)
 
@@ -353,16 +367,16 @@
     """
     videos = sorted(videos)
     new_order = parse_list(listfile)
 
     playlist = []
     with Core.from_dir(cache_dir, external_subs=external_subs) as core:
         video_parts = []
-        for video in videos:
-            subs = core.get_subs(video, language)
+        all_subs = get_all_subs(videos, core, language)
+        for video, subs in zip(videos, all_subs):
             events = query_events(subs, query, name=name)
             for event in events:
                 part = (video, event.start, event.end)
                 video_parts.append(part)
 
         video_parts = [video_parts[i] for i in new_order]
 
@@ -403,16 +417,16 @@
     Render supercut based on edit list.
     """
     videos = sorted(videos)
     new_order = parse_list(listfile)
 
     with Core.from_dir(cache_dir, external_subs=external_subs) as core:
         video_parts = []
-        for video in videos:
-            subs = core.get_subs(video, language)
+        all_subs = get_all_subs(videos, core, language)
+        for video, subs in zip(videos, all_subs):
             events = query_events(subs, query, name=name)
             for event in events:
                 part = ffmpeg.VideoPart(
                     video=video,
                     subs=trim_subs(subs, event.start, event.end).to_string("ass"),
                     start=event.start,
                     end=event.end,
@@ -420,14 +434,23 @@
                 video_parts.append(part)
 
         video_parts = [video_parts[i] for i in new_order]
 
         ffmpeg.supercut_free(video_parts, output=output)
 
 
+@util_app.command()
+def hardcode_subs(
+    video: typing.Annotated[Path, typer.Argument(help="The video to hardcode subs in")],
+    output: typing.Annotated[Path, typer.Option(help="Ouptut file")],
+):
+    """Hardcode the subtitles into the video frames."""
+    ffmpeg.hardcode_subs(video, output=output)
+
+
 @app.command()
 def check():
     """Ensure all requirements are met"""
     print("All good!")
 
 
 @app.callback()
```

### Comparing `supercut-0.2.2/src/supercut/vlc.py` & `supercut-0.3.0/src/supercut/vlc.py`

 * *Files identical despite different names*

### Comparing `supercut-0.2.2/PKG-INFO` & `supercut-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supercut
-Version: 0.2.2
+Version: 0.3.0
 Summary: Subtitle-based automatic supercut creation
 License: MIT
 Author: Tamir Bahar
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

