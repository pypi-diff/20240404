# Comparing `tmp/chess-notation-0.1.6.tar.gz` & `tmp/chess-notation-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-notation-0.1.6.tar", last modified: Sun Mar 31 16:21:33 2024, max compression
+gzip compressed data, was "chess-notation-0.1.7.tar", last modified: Thu Apr  4 08:50:30 2024, max compression
```

## Comparing `chess-notation-0.1.6.tar` & `chess-notation-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 16:21:33.929845 chess-notation-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-31 08:32:00.000000 chess-notation-0.1.6/MANIFEST.in
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      422 2024-03-31 16:21:33.929845 chess-notation-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-03-31 08:21:38.000000 chess-notation-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-03-31 16:21:17.000000 chess-notation-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-03-31 16:21:33.929845 chess-notation-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 16:21:33.919845 chess-notation-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 16:21:33.929845 chess-notation-0.1.6/src/chess_notation/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-03-31 08:24:21.000000 chess-notation-0.1.6/src/chess_notation/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 16:21:33.929845 chess-notation-0.1.6/src/chess_notation/language/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-03-31 08:26:21.000000 chess-notation-0.1.6/src/chess_notation/language/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      629 2024-03-31 13:25:28.000000 chess-notation-0.1.6/src/chess_notation/language/language.py
--rwxrwxrwx   0 m4rs      (1000) m4rs      (1000)     1641 2024-03-31 08:31:52.000000 chess-notation-0.1.6/src/chess_notation/language/translations.json
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 16:21:33.929845 chess-notation-0.1.6/src/chess_notation/represent/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-03-31 13:29:36.000000 chess-notation-0.1.6/src/chess_notation/represent/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2000 2024-03-31 13:29:43.000000 chess-notation-0.1.6/src/chess_notation/represent/represent.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 16:21:33.929845 chess-notation-0.1.6/src/chess_notation/styles/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      363 2024-03-31 16:21:10.000000 chess-notation-0.1.6/src/chess_notation/styles/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1240 2024-03-31 16:20:48.000000 chess-notation-0.1.6/src/chess_notation/styles/apply.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1057 2024-03-31 16:04:06.000000 chess-notation-0.1.6/src/chess_notation/styles/classify.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2357 2024-03-31 12:49:36.000000 chess-notation-0.1.6/src/chess_notation/styles/map.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-03-31 16:04:09.000000 chess-notation-0.1.6/src/chess_notation/styles/styles.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-31 16:21:33.929845 chess-notation-0.1.6/src/chess_notation.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      422 2024-03-31 16:21:33.000000 chess-notation-0.1.6/src/chess_notation.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-03-31 16:21:33.000000 chess-notation-0.1.6/src/chess_notation.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-03-31 16:21:33.000000 chess-notation-0.1.6/src/chess_notation.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-03-31 16:21:33.000000 chess-notation-0.1.6/src/chess_notation.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-03-31 16:21:33.000000 chess-notation-0.1.6/src/chess_notation.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-31 08:32:00.000000 chess-notation-0.1.7/MANIFEST.in
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      422 2024-04-04 08:50:30.919821 chess-notation-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-03-31 08:21:38.000000 chess-notation-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-04 08:50:07.000000 chess-notation-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 08:50:30.919821 chess-notation-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.909821 chess-notation-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-03-31 08:24:21.000000 chess-notation-0.1.7/src/chess_notation/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/language/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-03-31 08:26:21.000000 chess-notation-0.1.7/src/chess_notation/language/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      629 2024-03-31 13:25:28.000000 chess-notation-0.1.7/src/chess_notation/language/language.py
+-rwxrwxrwx   0 m4rs      (1000) m4rs      (1000)     1641 2024-03-31 08:31:52.000000 chess-notation-0.1.7/src/chess_notation/language/translations.json
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/represent/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-03-31 13:29:36.000000 chess-notation-0.1.7/src/chess_notation/represent/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2000 2024-03-31 13:29:43.000000 chess-notation-0.1.7/src/chess_notation/represent/represent.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/styles/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      363 2024-03-31 16:21:10.000000 chess-notation-0.1.7/src/chess_notation/styles/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1329 2024-04-04 08:49:59.000000 chess-notation-0.1.7/src/chess_notation/styles/apply.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1057 2024-03-31 16:04:06.000000 chess-notation-0.1.7/src/chess_notation/styles/classify.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2364 2024-04-04 08:49:34.000000 chess-notation-0.1.7/src/chess_notation/styles/map.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-03-31 16:04:09.000000 chess-notation-0.1.7/src/chess_notation/styles/styles.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      422 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/top_level.txt
```

### Comparing `chess-notation-0.1.6/src/chess_notation/language/language.py` & `chess-notation-0.1.7/src/chess_notation/language/language.py`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.6/src/chess_notation/language/translations.json` & `chess-notation-0.1.7/src/chess_notation/language/translations.json`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.6/src/chess_notation/represent/represent.py` & `chess-notation-0.1.7/src/chess_notation/represent/represent.py`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.6/src/chess_notation/styles/apply.py` & `chess-notation-0.1.7/src/chess_notation/styles/apply.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from pydantic import BaseModel
 from .styles import Check, Mate, Castle, PawnCapture, PieceCapture
 from .classify import is_castle, is_check, is_mate, is_pawn_capture, is_piece_capture
 from .map import castle, check, mate, pawn_capture, piece_capture, CapturedPiece
 
 class KingEffects(BaseModel):
-  check: Check = 'NONE'
-  mate: Mate = 'NONE'
+  check: Check | None = None
+  mate: Mate | None = None
 
 class Motions(BaseModel):
-  castle: Castle = 'O-O'
-  pawn_capture: PawnCapture = 'dxe4'
-  piece_capture: PieceCapture = 'Nxe4'
+  castle: Castle | None = None
+  pawn_capture: PawnCapture | None = None
+  piece_capture: PieceCapture | None = None
 
 class Styles(KingEffects, Motions):
   ...
 
-def style_motions(san: str, motions: Motions, captured_piece: CapturedPiece = None) -> str:
+def style_motions(san: str, motions: Motions, captured_piece: CapturedPiece | None = None) -> str:
   if is_pawn_capture(san):
-    return pawn_capture(san, motions.pawn_capture, captured_piece)
+    return pawn_capture(san, motions.pawn_capture or 'dxe4', captured_piece)
   elif is_piece_capture(san):
-    return piece_capture(san, motions.piece_capture, captured_piece)
+    return piece_capture(san, motions.piece_capture or 'Nxe4', captured_piece)
   elif is_castle(san):
-    return castle(san, motions.castle)
+    return castle(san, motions.castle or 'O-O')
   else:
     return san
   
 def style_effects(san: str, effects: KingEffects) -> str:
   if is_check(san):
-    return check(san, effects.check)
+    return check(san, effects.check or 'NONE')
   elif is_mate(san):
-    return mate(san, effects.mate)
+    return mate(san, effects.mate or 'NONE')
   else:
     return san
   
-def style(san: str, styles: Styles, captured_piece: CapturedPiece = None) -> str:
+def style(san: str, styles: Styles, captured_piece: CapturedPiece | None = None) -> str:
   return style_effects(style_motions(san, styles, captured_piece), styles)
```

### Comparing `chess-notation-0.1.6/src/chess_notation/styles/classify.py` & `chess-notation-0.1.7/src/chess_notation/styles/classify.py`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.6/src/chess_notation/styles/map.py` & `chess-notation-0.1.7/src/chess_notation/styles/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             return san.replace("-", "")
         case 'O-O':
             return san
 
 def pawn_capture(
     san: str,
     style: PawnCapture,
-    captured_piece: CapturedPiece = None,
+    captured_piece: CapturedPiece | None = None,
     pawn: str = "P"
 ) -> str:
     """Apply pawn capture `style`
     - If `style == PawnCatpure.PxN` but `captured_piece is None`, `san` will be returned as is
     """
     [d, x, e, n, *tail] = san
     rest = "".join(tail)
```

### Comparing `chess-notation-0.1.6/src/chess_notation.egg-info/SOURCES.txt` & `chess-notation-0.1.7/src/chess_notation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

