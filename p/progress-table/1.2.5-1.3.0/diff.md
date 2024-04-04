# Comparing `tmp/progress-table-1.2.5.tar.gz` & `tmp/progress-table-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-1.2.5.tar", last modified: Wed Mar 13 09:35:49 2024, max compression
+gzip compressed data, was "progress-table-1.3.0.tar", last modified: Thu Apr  4 15:48:45 2024, max compression
```

## Comparing `progress-table-1.2.5.tar` & `progress-table-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-03-13 09:35:49.113512 progress-table-1.2.5/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-1.2.5/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-03-13 09:35:49.113512 progress-table-1.2.5/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4143 2024-03-11 20:12:42.000000 progress-table-1.2.5/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-03-13 09:35:49.110179 progress-table-1.2.5/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      282 2024-03-13 09:35:04.000000 progress-table-1.2.5/progress_table/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1725 2023-10-29 15:02:10.000000 progress-table-1.2.5/progress_table/test_docs_automated.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-03-13 09:35:49.113512 progress-table-1.2.5/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)        0 2024-03-11 20:11:56.000000 progress-table-1.2.5/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23208 2024-03-11 20:11:56.000000 progress-table-1.2.5/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2986 2024-03-11 20:11:56.000000 progress-table-1.2.5/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-03-13 09:35:49.113512 progress-table-1.2.5/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)        0 2024-03-11 20:11:56.000000 progress-table-1.2.5/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    28311 2024-03-13 09:22:41.000000 progress-table-1.2.5/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3089 2024-03-11 20:11:56.000000 progress-table-1.2.5/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-03-13 09:35:49.113512 progress-table-1.2.5/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-03-13 09:35:49.000000 progress-table-1.2.5/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      498 2024-03-13 09:35:49.000000 progress-table-1.2.5/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-03-13 09:35:49.000000 progress-table-1.2.5/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-03-13 09:35:49.000000 progress-table-1.2.5/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-03-13 09:35:49.000000 progress-table-1.2.5/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-1.2.5/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-03-13 09:35:49.113512 progress-table-1.2.5/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1499 2024-03-13 09:22:41.000000 progress-table-1.2.5/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-1.3.0/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-04 15:48:45.159666 progress-table-1.3.0/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4143 2024-03-12 12:06:20.000000 progress-table-1.3.0/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.156332 progress-table-1.3.0/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      287 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23213 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    28478 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3132 2024-04-04 15:47:39.000000 progress-table-1.3.0/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-04 15:48:45.159666 progress-table-1.3.0/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4907 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-1.3.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      531 2024-04-04 15:48:45.000000 progress-table-1.3.0/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-04 15:48:44.000000 progress-table-1.3.0/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-1.3.0/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-04 15:48:45.162999 progress-table-1.3.0/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-04 15:47:39.000000 progress-table-1.3.0/setup.py
```

### Comparing `progress-table-1.2.5/LICENSE.txt` & `progress-table-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-1.2.5/PKG-INFO` & `progress-table-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 1.2.5
+Version: 1.3.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-1.2.5/README.md` & `progress-table-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `progress-table-1.2.5/progress_table/v0/progress_table.py` & `progress-table-1.3.0/progress_table/v0/progress_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022 Szymon Mikler
+#  Copyright (c) 2022-2024 Szymon Mikler
 
 from __future__ import annotations
 
 import inspect
 import logging
 import math
 import shutil
```

### Comparing `progress-table-1.2.5/progress_table/v0/symbols.py` & `progress-table-1.3.0/progress_table/v0/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#  Copyright (c) 2022-2024 Szymon Mikler
+
 from dataclasses import dataclass
 
 
 @dataclass
 class Symbols:
     pbar_filled: str
     pbar_empty: str
```

### Comparing `progress-table-1.2.5/progress_table/v1/progress_table.py` & `progress-table-1.3.0/progress_table/v1/progress_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022 Szymon Mikler
+#  Copyright (c) 2022-2024 Szymon Mikler
 
 from __future__ import annotations
 
 import inspect
 import logging
 import math
 import shutil
@@ -655,21 +655,25 @@
             pbar.extend(row[:2] + infobar)
             row = row[2 + len(infobar) :]
 
             if not self._total:  # When total is unknown
                 total = len(row)
                 step = self._step % total
 
-            new_row = []
+            new_row = [Style.BRIGHT]
             for letter_idx, letter in enumerate(row):
-                if letter == " ":
-                    if letter_idx / len(row) <= (step / total) % (1 + EPS):
-                        letter = self.table.table_style.embedded_pbar_filled
-                    elif (letter_idx - 1) / len(row) <= (step / total) % (1 + EPS):
-                        letter = self.table.table_style.embedded_pbar_head
+                is_bar = letter_idx / len(row) <= (step / total) % (1 + EPS)
+                is_head = (letter_idx - 1) / len(row) <= (step / total) % (1 + EPS)
+                if letter == " " and is_bar:
+                    letter = self.table.table_style.embedded_pbar_filled
+                if letter == " " and is_head:
+                    letter = self.table.table_style.embedded_pbar_head
+
+                if not is_bar and not is_head:
+                    new_row.append(Style.RESET_ALL)
                 new_row.append(letter)
             pbar.extend(new_row)
         pbar.append(CURSOR_UP * self.level)
         self.table._print("".join(pbar), end="\r")
 
     def _update(self, n):
         self._step += n
```

### Comparing `progress-table-1.2.5/progress_table/v1/styles.py` & `progress-table-1.3.0/progress_table/v1/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#  Copyright (c) 2022-2024 Szymon Mikler
+
+
 class StyleNormal:
     name = "normal"
     pbar_filled = "■"
     pbar_empty = "□"
     embedded_pbar_filled = "ꞏ"
     embedded_pbar_head = ">"
     cell_overflow = "…"
```

### Comparing `progress-table-1.2.5/progress_table.egg-info/PKG-INFO` & `progress-table-1.3.0/progress_table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 1.2.5
+Version: 1.3.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-1.2.5/setup.py` & `progress-table-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-#  Copyright (c) 2022 Szymon Mikler
+#  Copyright (c) 2022-2024 Szymon Mikler
 
 from pathlib import Path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 
 def package_relative_path(path):
     return Path(__file__).parent / path
 
 
 def get_version():
```

