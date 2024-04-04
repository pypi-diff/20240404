# Comparing `tmp/rpg_xml-0.1.1-py3-none-any.whl.zip` & `tmp/rpg_xml-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,14 @@
-Zip file size: 9107 bytes, number of entries: 15
--rw-------  2.0 unx      134 b- defN 24-Mar-31 17:07 rpg_xml/__init__.py
--rw-------  2.0 unx     1270 b- defN 24-Apr-02 00:35 rpg_xml/engine.py
--rw-------  2.0 unx     1116 b- defN 24-Mar-31 17:02 rpg_xml/music_controller.py
--rw-------  2.0 unx     1174 b- defN 24-Mar-31 09:48 rpg_xml/music_player.py
--rw-------  2.0 unx     2218 b- defN 24-Apr-01 02:31 rpg_xml/scene_controller.py
--rw-------  2.0 unx     2068 b- defN 24-Mar-31 17:07 rpg_xml/scene_processor.py
--rw-------  2.0 unx     2313 b- defN 24-Mar-31 16:23 rpg_xml/scene_processor_old.py
--rw-------  2.0 unx     2662 b- defN 24-Apr-02 00:35 rpg_xml/util.py
--rw-------  2.0 unx     2857 b- defN 24-Mar-31 06:37 rpg_xml/util_old.py
--rw-------  2.0 unx     1007 b- defN 24-Mar-31 17:17 rpg_xml/xmlparser.py
--rw-------  2.0 unx     1070 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/LICENSE
--rw-------  2.0 unx      135 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/WHEEL
--rw-------  2.0 unx        8 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1176 b- defN 24-Apr-02 00:51 rpg_xml-0.1.1.dist-info/RECORD
-15 files, 19300 bytes uncompressed, 7181 bytes compressed:  62.8%
+Zip file size: 6336 bytes, number of entries: 12
+-rw-------  2.0 unx      143 b- defN 24-Apr-04 17:04 rpg_xml/__init__.py
+-rw-------  2.0 unx     1277 b- defN 24-Apr-04 17:04 rpg_xml/engine.py
+-rw-------  2.0 unx     1116 b- defN 24-Apr-03 15:33 rpg_xml/music_controller.py
+-rw-------  2.0 unx     1188 b- defN 24-Apr-03 15:33 rpg_xml/music_player.py
+-rw-------  2.0 unx     2218 b- defN 24-Apr-03 15:33 rpg_xml/scene_controller.py
+-rw-------  2.0 unx     2662 b- defN 24-Apr-04 17:04 rpg_xml/terminal_ui.py
+-rw-------  2.0 unx     1007 b- defN 24-Apr-03 15:33 rpg_xml/xmlparser.py
+-rw-------  2.0 unx     1070 b- defN 24-Apr-04 17:04 rpg_xml-0.1.2.dist-info/LICENSE
+-rw-------  2.0 unx      135 b- defN 24-Apr-04 17:04 rpg_xml-0.1.2.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 24-Apr-04 17:04 rpg_xml-0.1.2.dist-info/WHEEL
+-rw-------  2.0 unx        8 b- defN 24-Apr-04 17:04 rpg_xml-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      937 b- defN 24-Apr-04 17:04 rpg_xml-0.1.2.dist-info/RECORD
+12 files, 11853 bytes uncompressed, 4774 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -9,38 +9,29 @@
 
 Filename: rpg_xml/music_player.py
 Comment: 
 
 Filename: rpg_xml/scene_controller.py
 Comment: 
 
-Filename: rpg_xml/scene_processor.py
-Comment: 
-
-Filename: rpg_xml/scene_processor_old.py
-Comment: 
-
-Filename: rpg_xml/util.py
-Comment: 
-
-Filename: rpg_xml/util_old.py
+Filename: rpg_xml/terminal_ui.py
 Comment: 
 
 Filename: rpg_xml/xmlparser.py
 Comment: 
 
-Filename: rpg_xml-0.1.1.dist-info/LICENSE
+Filename: rpg_xml-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: rpg_xml-0.1.1.dist-info/METADATA
+Filename: rpg_xml-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: rpg_xml-0.1.1.dist-info/WHEEL
+Filename: rpg_xml-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: rpg_xml-0.1.1.dist-info/top_level.txt
+Filename: rpg_xml-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rpg_xml-0.1.1.dist-info/RECORD
+Filename: rpg_xml-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rpg_xml/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .engine import Engine
-from .util import TerminalUI
+from .terminal_ui import TerminalUI
 from .xmlparser import XmlParser
 
-from .scene_processor import SceneProcessor
+from .scene_controller import SceneController
```

## rpg_xml/engine.py

```diff
@@ -1,8 +1,8 @@
-from .util import TerminalUI
+from .terminal_ui import TerminalUI
 from .xmlparser import XmlParser
 from .scene_controller import SceneController
 
 
 class Engine:
     def __init__(self, path) -> None:
         self.parser = XmlParser(path)
```

## rpg_xml/music_player.py

```diff
@@ -5,15 +5,15 @@
     def __init__(self, file_path):
         self.file_path = file_path
         self.process = None
 
     def play(self):
         if not self.process:
             self.process = subprocess.Popen(
-                ["mpv", "--loop=inf", self.file_path],
+                ["mpv", "--loop=inf", "--no-video", self.file_path],
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
         else:
             print("A música já está sendo reproduzida.")
 
     def stop(self):
```

## Comparing `rpg_xml/util.py` & `rpg_xml/terminal_ui.py`

 * *Files identical despite different names*

## Comparing `rpg_xml-0.1.1.dist-info/LICENSE` & `rpg_xml-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

