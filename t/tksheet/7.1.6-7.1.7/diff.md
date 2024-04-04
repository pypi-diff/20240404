# Comparing `tmp/tksheet-7.1.6.tar.gz` & `tmp/tksheet-7.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-7.1.6.tar", last modified: Mon Apr  1 18:46:23 2024, max compression
+gzip compressed data, was "tksheet-7.1.7.tar", last modified: Thu Apr  4 19:00:53 2024, max compression
```

## Comparing `tksheet-7.1.6.tar` & `tksheet-7.1.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-01 18:46:23.587094 tksheet-7.1.6/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.6/LICENSE.txt
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-01 18:46:23.587094 tksheet-7.1.6/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.6/README.md
--rw-rw-r--   0 rg        (1000) rg        (1000)     1064 2024-03-31 10:01:25.000000 tksheet-7.1.6/pyproject.toml
--rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-01 18:46:23.587094 tksheet-7.1.6/setup.cfg
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-01 18:46:23.583094 tksheet-7.1.6/tksheet/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1874 2024-03-31 10:01:25.000000 tksheet-7.1.6/tksheet/__init__.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.6/tksheet/colors.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    99449 2024-04-01 08:20:52.000000 tksheet-7.1.6/tksheet/column_headers.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.6/tksheet/formatters.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    39610 2024-04-01 08:19:58.000000 tksheet-7.1.6/tksheet/functions.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   321201 2024-04-01 18:36:21.000000 tksheet-7.1.6/tksheet/main_table.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13604 2024-03-30 16:31:45.000000 tksheet-7.1.6/tksheet/other_classes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   104750 2024-04-01 18:30:11.000000 tksheet-7.1.6/tksheet/row_index.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   257417 2024-04-01 18:28:12.000000 tksheet-7.1.6/tksheet/sheet.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    11906 2024-03-19 09:32:45.000000 tksheet-7.1.6/tksheet/sheet_options.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.6/tksheet/text_editor.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.6/tksheet/themes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.6/tksheet/top_left_rectangle.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.6/tksheet/types.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     2092 2024-03-23 14:39:32.000000 tksheet-7.1.6/tksheet/vars.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-01 18:46:23.587094 tksheet-7.1.6/tksheet.egg-info/
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-01 18:46:23.000000 tksheet-7.1.6/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-04 19:00:53.996107 tksheet-7.1.7/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.7/LICENSE.txt
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-04 19:00:53.996107 tksheet-7.1.7/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.7/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-04-01 18:49:27.000000 tksheet-7.1.7/pyproject.toml
+-rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-04 19:00:53.996107 tksheet-7.1.7/setup.cfg
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-04 19:00:53.996107 tksheet-7.1.7/tksheet/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2010 2024-04-04 06:38:42.000000 tksheet-7.1.7/tksheet/__init__.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.7/tksheet/colors.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    99870 2024-04-04 18:51:50.000000 tksheet-7.1.7/tksheet/column_headers.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.7/tksheet/formatters.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    39612 2024-04-04 07:10:00.000000 tksheet-7.1.7/tksheet/functions.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      384 2024-04-04 18:57:38.000000 tksheet-7.1.7/tksheet/listbox.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   323154 2024-04-04 18:54:36.000000 tksheet-7.1.7/tksheet/main_table.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13604 2024-03-30 16:31:45.000000 tksheet-7.1.7/tksheet/other_classes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   105354 2024-04-04 18:51:54.000000 tksheet-7.1.7/tksheet/row_index.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   256166 2024-04-04 14:40:53.000000 tksheet-7.1.7/tksheet/sheet.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    11978 2024-04-04 14:40:28.000000 tksheet-7.1.7/tksheet/sheet_options.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.7/tksheet/text_editor.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.7/tksheet/themes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.7/tksheet/top_left_rectangle.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.7/tksheet/types.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2092 2024-03-23 14:39:32.000000 tksheet-7.1.7/tksheet/vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-04 19:00:53.996107 tksheet-7.1.7/tksheet.egg-info/
+-rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      500 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-04 19:00:53.000000 tksheet-7.1.7/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-7.1.6/LICENSE.txt` & `tksheet-7.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/PKG-INFO` & `tksheet-7.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.6
+Version: 7.1.7
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `tksheet-7.1.6/README.md` & `tksheet-7.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/pyproject.toml` & `tksheet-7.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "tksheet"
-description = "Tkinter table / sheet widget"
-readme = "README.md"
-version = "7.1.6"
-authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
-requires-python = ">=3.8"
-license = {file = "LICENSE.txt"}
-keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: Libraries",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/ragardner/tksheet"
-"Bug Reports" = "https://github.com/ragardner/tksheet/issues"
-"Funding" = "https://github.com/ragardner"
-
-[tool.black]
-line-length = 120
-
-[tool.ruff]
-line-length = 120
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "tksheet"
+description = "Tkinter table / sheet widget"
+readme = "README.md"
+version = "7.1.7"
+authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
+requires-python = ">=3.8"
+license = {file = "LICENSE.txt"}
+keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Libraries",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/ragardner/tksheet"
+"Bug Reports" = "https://github.com/ragardner/tksheet/issues"
+"Funding" = "https://github.com/ragardner"
+
+[tool.black]
+line-length = 120
+
+[tool.ruff]
+line-length = 120
```

### Comparing `tksheet-7.1.6/tksheet/__init__.py` & `tksheet-7.1.7/tksheet/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,99 @@
-# ruff: noqa: F401
-
-"""
-tksheet - A Python tkinter table widget
-"""
-
-__version__ = "7.1.6"
-
-from .colors import (
-    color_map,
-)
-from .column_headers import ColumnHeaders
-from .formatters import (
-    Formatter,
-    bool_formatter,
-    data_to_str,
-    float_formatter,
-    float_to_str,
-    format_data,
-    formatter,
-    get_clipboard_data,
-    get_data_with_valid_check,
-    int_formatter,
-    is_bool_like,
-    is_none_like,
-    percentage_formatter,
-    percentage_to_str,
-    to_bool,
-    to_float,
-    to_int,
-    to_str,
-    try_to_bool,
-)
-from .functions import (
-    alpha2idx,
-    alpha2num,
-    consecutive_chunks,
-    data_to_displayed_idxs,
-    displayed_to_data_idxs,
-    dropdown_search_function,
-    event_dict,
-    get_checkbox_dict,
-    get_checkbox_kwargs,
-    get_checkbox_points,
-    get_dropdown_dict,
-    get_dropdown_kwargs,
-    get_index_of_gap_in_sorted_integer_seq_forward,
-    get_index_of_gap_in_sorted_integer_seq_reverse,
-    get_n2a,
-    get_new_indexes,
-    get_seq_without_gaps_at_index,
-    is_iterable,
-    move_elements_by_mapping,
-    move_elements_to,
-    num2alpha,
-    span_dict,
-    tksheet_type_error,
-)
-from .main_table import MainTable
-from .other_classes import (
-    DotDict,
-    DraggedRowColumn,
-    DrawnItem,
-    EventDataDict,
-    GeneratedMouseEvent,
-    Selected,
-    Span,
-    SpanRange,
-    TextCfg,
-)
-from .row_index import RowIndex
-from .sheet import Dropdown, Sheet
-from .sheet_options import new_sheet_options
-from .text_editor import (
-    TextEditor,
-    TextEditorTkText,
-)
-from .themes import (
-    theme_black,
-    theme_dark,
-    theme_dark_blue,
-    theme_dark_green,
-    theme_light_blue,
-    theme_light_green,
-)
-from .top_left_rectangle import TopLeftRectangle
-from .vars import (
-    USER_OS,
-    ctrl_key,
-    emitted_events,
-    falsy,
-    nonelike,
-    rc_binding,
-    symbols_set,
-    truthy,
-)
+# ruff: noqa: F401
+
+"""
+tksheet - A Python tkinter table widget
+"""
+
+__version__ = "7.1.7"
+
+from .colors import (
+    color_map,
+)
+from .column_headers import ColumnHeaders
+from .formatters import (
+    Formatter,
+    bool_formatter,
+    data_to_str,
+    float_formatter,
+    float_to_str,
+    format_data,
+    formatter,
+    get_clipboard_data,
+    get_data_with_valid_check,
+    int_formatter,
+    is_bool_like,
+    is_none_like,
+    percentage_formatter,
+    percentage_to_str,
+    to_bool,
+    to_float,
+    to_int,
+    to_str,
+    try_to_bool,
+)
+from .functions import (
+    alpha2idx,
+    alpha2num,
+    consecutive_chunks,
+    data_to_displayed_idxs,
+    displayed_to_data_idxs,
+    dropdown_search_function,
+    event_dict,
+    get_checkbox_dict,
+    get_checkbox_kwargs,
+    rounded_box_coords,
+    get_dropdown_dict,
+    get_dropdown_kwargs,
+    get_index_of_gap_in_sorted_integer_seq_forward,
+    get_index_of_gap_in_sorted_integer_seq_reverse,
+    get_n2a,
+    get_new_indexes,
+    get_seq_without_gaps_at_index,
+    is_iterable,
+    move_elements_by_mapping,
+    move_elements_to,
+    num2alpha,
+    span_dict,
+    tksheet_type_error,
+)
+from .listbox import (
+    ListBox,
+)
+from .main_table import MainTable
+from .other_classes import (
+    DotDict,
+    DraggedRowColumn,
+    DrawnItem,
+    EventDataDict,
+    GeneratedMouseEvent,
+    Selected,
+    Span,
+    SpanRange,
+    TextCfg,
+)
+from .row_index import RowIndex
+from .sheet import Dropdown, Sheet
+from .sheet_options import new_sheet_options
+from .text_editor import (
+    TextEditor,
+    TextEditorTkText,
+)
+from .themes import (
+    theme_black,
+    theme_dark,
+    theme_dark_blue,
+    theme_dark_green,
+    theme_light_blue,
+    theme_light_green,
+)
+from .top_left_rectangle import TopLeftRectangle
+from .vars import (
+    USER_OS,
+    ctrl_key,
+    emitted_events,
+    falsy,
+    nonelike,
+    rc_binding,
+    symbols_set,
+    truthy,
+)
```

### Comparing `tksheet-7.1.6/tksheet/colors.py` & `tksheet-7.1.7/tksheet/colors.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/tksheet/column_headers.py` & `tksheet-7.1.7/tksheet/column_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     color_map,
 )
 from .formatters import is_bool_like, try_to_bool
 from .functions import (
     consecutive_ranges,
     ev_stack_dict,
     event_dict,
-    get_checkbox_points,
+    rounded_box_coords,
     get_n2a,
     is_contiguous,
     try_binding,
 )
 from .other_classes import (
     DotDict,
     DraggedRowColumn,
@@ -931,22 +931,34 @@
         y1: int,
         x2: int,
         y2: int,
         fill: str,
         outline: str,
         state: str,
         tags: str | tuple[str],
+        iid: None | int = None,
     ) -> int:
-        if self.hidd_boxes:
-            iid = self.hidd_boxes.pop()
-            self.coords(iid, x1, y1, x2, y2)
+        coords = rounded_box_coords(
+            x1,
+            y1,
+            x2,
+            y2,
+            radius=9 if self.PAR.ops.rounded_boxes else 0,
+        )
+        if isinstance(iid, int):
+            self.coords(iid, coords)
             self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags)
         else:
-            iid = self.create_rectangle(x1, y1, x2, y2, fill=fill, outline=outline, state=state, tags=tags)
-        self.disp_boxes.add(iid)
+            if self.hidd_boxes:
+                iid = self.hidd_boxes.pop()
+                self.coords(iid, coords)
+                self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags)
+            else:
+                iid = self.create_polygon(coords, fill=fill, outline=outline, state=state, tags=tags, smooth=True)
+            self.disp_boxes.add(iid)
         return iid
 
     def hide_box(self, item: int) -> None:
         if isinstance(item, int):
             self.disp_boxes.discard(item)
             self.hidd_boxes.add(item)
             self.itemconfig(item, state="hidden")
@@ -1272,15 +1284,15 @@
                     capstyle=tk.ROUND,
                     joinstyle=tk.ROUND,
                     tag=tag,
                 )
             self.disp_dropdown[t] = True
 
     def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check=False):
-        points = get_checkbox_points(x1, y1, x2, y2)
+        points = rounded_box_coords(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
                 self.itemconfig(t, fill=outline, outline=fill, tag=tag, state="normal")
@@ -1290,15 +1302,15 @@
         self.disp_checkbox[t] = True
         if draw_check:
             # draw filled box
             x1 = x1 + 4
             y1 = y1 + 4
             x2 = x2 - 3
             y2 = y2 - 3
-            points = get_checkbox_points(x1, y1, x2, y2, radius=4)
+            points = rounded_box_coords(x1, y1, x2, y2, radius=4)
             if self.hidd_checkbox:
                 t, sh = self.hidd_checkbox.popitem()
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill, outline=outline)
                 else:
                     self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
@@ -1570,24 +1582,22 @@
         for dct in (self.hidd_text, self.hidd_high, self.hidd_grid, self.hidd_dropdown, self.hidd_checkbox):
             for iid, showing in dct.items():
                 if showing:
                     self.itemconfig(iid, state="hidden")
                     dct[iid] = False
         return True
 
-    def get_redraw_selections(self, startc, endc):
-        d = defaultdict(list)
+    def get_redraw_selections(self, startc: int, endc: int) -> dict[str, set[int]]:
+        d = defaultdict(set)
         for item, box in self.MT.get_selection_items(rows=False):
-            d[box.type_].append(box.coords)
-        d2 = {}
-        if "cells" in d:
-            d2["cells"] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d["cells"] if c1 <= c and c2 > c}
-        if "columns" in d:
-            d2["columns"] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d["columns"] if c1 <= c and c2 > c}
-        return d2
+            r1, c1, r2, c2 = box.coords
+            for c in range(startc, endc):
+                if c1 <= c and c2 > c:
+                    d[box.type_].add(c)
+        return d
 
     def open_cell(self, event: object = None, ignore_existing_editor=False):
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor.open):
             return
         if not self.MT.selected:
             return
         c = self.MT.selected.column
@@ -1813,14 +1823,16 @@
                     self.MT.col_positions[c],
                     0,
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
+            for b in ("<Alt-Return>", "<Option-Return>", "<Tab>", "<Return>", "<FocusOut>", "<Escape>"):
+                self.text_editor.tktext.unbind(b)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     # c is displayed col
     def close_text_editor(
@@ -1836,40 +1848,40 @@
             pass
         if focused is None and editor_info:
             return "break"
         if editor_info[1] == "Escape":
             self.hide_text_editor_and_dropdown()
             return
         # setting cell data with text editor value
-        self.text_editor_value = self.text_editor.get()
+        text_editor_value = self.text_editor.get()
         c = editor_info[0]
         datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         event_data = event_dict(
             name="end_edit_header",
             sheet=self.PAR.name,
             cells_header={datacn: self.get_cell_data(datacn)},
             key=editor_info[1] if len(editor_info) >= 2 else "FocusOut",
-            value=self.text_editor_value,
+            value=text_editor_value,
             loc=c,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
         set_data = partial(
             self.set_cell_data_undo,
             c=c,
             datacn=datacn,
             check_input_valid=False,
         )
         if self.MT.edit_validation_func:
-            self.text_editor_value = self.MT.edit_validation_func(event_data)
-            if self.text_editor_value is not None and self.input_valid_for_cell(datacn, self.text_editor_value):
-                edited = set_data(value=self.text_editor_value)
-        elif self.input_valid_for_cell(datacn, self.text_editor_value):
-            edited = set_data(value=self.text_editor_value)
+            text_editor_value = self.MT.edit_validation_func(event_data)
+            if text_editor_value is not None and self.input_valid_for_cell(datacn, text_editor_value):
+                edited = set_data(value=text_editor_value)
+        elif self.input_valid_for_cell(datacn, text_editor_value):
+            edited = set_data(value=text_editor_value)
         if edited:
             try_binding(self.extra_end_edit_cell_func, event_data)
         self.MT.recreate_all_selection_boxes()
         self.hide_text_editor_and_dropdown()
         if editor_info[1] != "FocusOut":
             self.focus_set()
         return "break"
@@ -2033,14 +2045,15 @@
     def mouseclick_outside_editor_or_dropdown_all_canvases(self, inside: bool = False):
         self.RI.mouseclick_outside_editor_or_dropdown()
         self.MT.mouseclick_outside_editor_or_dropdown()
         return self.mouseclick_outside_editor_or_dropdown(inside)
 
     def hide_dropdown_window(self) -> None:
         if self.dropdown.open:
+            self.dropdown.window.unbind("<FocusOut>")
             self.itemconfig(self.dropdown.canvas_id, state="hidden")
             self.dropdown.open = False
 
     # internal event use
     def set_cell_data_undo(
         self,
         c=0,
```

### Comparing `tksheet-7.1.6/tksheet/formatters.py` & `tksheet-7.1.7/tksheet/formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/tksheet/functions.py` & `tksheet-7.1.7/tksheet/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
 
 
 def consecutive_chunks(seq: list[int]) -> Generator[list[int]]:
     start = 0
     for index, value in enumerate(seq, 1):
         try:
             if seq[index] > value + 1:
-                yield seq[start:(start := index)]
+                yield seq[start : (start := index)]
         except Exception:
             yield seq[start : len(seq)]
 
 
 def consecutive_ranges(seq: Sequence[int]) -> Generator[tuple[int, int]]:
     start = 0
     for index, value in enumerate(seq, 1):
@@ -500,22 +500,22 @@
 def displayed_to_data_idxs(
     to_convert: list[int],
     displayed: list[int],
 ) -> list[int]:
     return [displayed[e] for e in to_convert]
 
 
-def get_checkbox_points(
+def rounded_box_coords(
     x1: float,
     y1: float,
     x2: float,
     y2: float,
     radius: int = 8,
-) -> list[float]:
-    return [
+) -> tuple[float]:
+    return (
         x1 + radius,
         y1,
         x1 + radius,
         y1,
         x2 - radius,
         y1,
         x2 - radius,
@@ -548,15 +548,15 @@
         y2 - radius,
         x1,
         y1 + radius,
         x1,
         y1 + radius,
         x1,
         y1,
-    ]
+    )
 
 
 def diff_list(seq: list[float]) -> list[int]:
     return [
         int(b - a)
         for a, b in zip(
             seq,
```

### Comparing `tksheet-7.1.6/tksheet/main_table.py` & `tksheet-7.1.7/tksheet/main_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     consecutive_ranges,
     decompress_load,
     diff_gen,
     diff_list,
     ev_stack_dict,
     event_dict,
     gen_formatted,
-    get_checkbox_points,
+    rounded_box_coords,
     get_new_indexes,
     get_seq_without_gaps_at_index,
     index_exists,
     insert_items,
     int_x_iter,
     is_iterable,
     is_type_int,
@@ -995,109 +995,112 @@
             }
             self.cell_options = {(k[0], full_new_idxs[k[1]]): v for k, v in self.cell_options.items()}
             self.col_options = {full_new_idxs[k]: v for k, v in self.col_options.items()}
             self.tagged_columns = {
                 tags: {full_new_idxs[k] for k in tagged} for tags, tagged in self.tagged_columns.items()
             }
             self.CH.cell_options = {full_new_idxs[k]: v for k, v in self.CH.cell_options.items()}
-            totalrows = self.total_data_rows()
-            new_ops = self.PAR.create_options_from_span
-            qkspan = self.span()
-            for span in self.named_spans.values():
-                # span is neither a cell options nor col options span, continue
-                if not isinstance(span["from_c"], int):
-                    continue
-                oldupto_colrange, newupto_colrange, newfrom, newupto = span_idxs_post_move(
-                    data_new_idxs,
-                    full_new_idxs,
-                    totalcols,
-                    span,
-                    "c",
-                )
-                # add cell/col kwargs for columns that are new to the span
-                old_span_idxs = set(full_new_idxs[k] for k in range(span["from_c"], oldupto_colrange))
-                for k in range(newfrom, newupto_colrange):
-                    if k not in old_span_idxs:
-                        oldidx = full_old_idxs[k]
-                        # event_data is used to preserve old cell value
-                        # in case cells are modified by
-                        # formatting, checkboxes, dropdown boxes
-                        if (
-                            span["type_"] in val_modifying_options
-                            and span["header"]
-                            and oldidx not in event_data["cells"]["header"]
-                        ):
-                            event_data["cells"]["header"][oldidx] = self.CH.get_cell_data(k)
-                        # the span targets columns
-                        if span["from_r"] is None:
-                            if span["type_"] in val_modifying_options:
-                                for datarn in range(len(self.data)):
-                                    if (datarn, oldidx) not in event_data["cells"]["table"]:
-                                        event_data["cells"]["table"][(datarn, oldidx)] = self.get_cell_data(datarn, k)
-                            # create new col options
-                            new_ops(
-                                mod_span(
-                                    qkspan,
-                                    span,
-                                    from_c=k,
-                                    upto_c=k + 1,
-                                )
-                            )
-                        # the span targets cells
-                        else:
-                            rng_upto_r = totalrows if span["upto_r"] is None else span["upto_r"]
-                            for datarn in range(span["from_r"], rng_upto_r):
-                                if (
-                                    span["type_"] in val_modifying_options
-                                    and (datarn, oldidx) not in event_data["cells"]["table"]
-                                ):
-                                    event_data["cells"]["table"][(datarn, oldidx)] = self.get_cell_data(datarn, k)
-                                # create new cell options
+            if self.named_spans:
+                totalrows = self.total_data_rows()
+                new_ops = self.PAR.create_options_from_span
+                qkspan = self.span()
+                for span in self.named_spans.values():
+                    # span is neither a cell options nor col options span, continue
+                    if not isinstance(span["from_c"], int):
+                        continue
+                    oldupto_colrange, newupto_colrange, newfrom, newupto = span_idxs_post_move(
+                        data_new_idxs,
+                        full_new_idxs,
+                        totalcols,
+                        span,
+                        "c",
+                    )
+                    # add cell/col kwargs for columns that are new to the span
+                    old_span_idxs = set(full_new_idxs[k] for k in range(span["from_c"], oldupto_colrange))
+                    for k in range(newfrom, newupto_colrange):
+                        if k not in old_span_idxs:
+                            oldidx = full_old_idxs[k]
+                            # event_data is used to preserve old cell value
+                            # in case cells are modified by
+                            # formatting, checkboxes, dropdown boxes
+                            if (
+                                span["type_"] in val_modifying_options
+                                and span["header"]
+                                and oldidx not in event_data["cells"]["header"]
+                            ):
+                                event_data["cells"]["header"][oldidx] = self.CH.get_cell_data(k)
+                            # the span targets columns
+                            if span["from_r"] is None:
+                                if span["type_"] in val_modifying_options:
+                                    for datarn in range(len(self.data)):
+                                        if (datarn, oldidx) not in event_data["cells"]["table"]:
+                                            event_data["cells"]["table"][(datarn, oldidx)] = self.get_cell_data(
+                                                datarn, k
+                                            )
+                                # create new col options
                                 new_ops(
                                     mod_span(
                                         qkspan,
                                         span,
-                                        from_r=datarn,
-                                        upto_r=datarn + 1,
                                         from_c=k,
                                         upto_c=k + 1,
                                     )
                                 )
-                # remove span specific kwargs from cells/columns
-                # that are no longer in the span,
-                # cell options/col options keys are new idxs
-                for k in range(span["from_c"], oldupto_colrange):
-                    # has it moved outside of new span coords
-                    if (isinstance(newupto, int) and (full_new_idxs[k] < newfrom or full_new_idxs[k] >= newupto)) or (
-                        newupto is None and full_new_idxs[k] < newfrom
-                    ):
-                        # span includes header
+                            # the span targets cells
+                            else:
+                                rng_upto_r = totalrows if span["upto_r"] is None else span["upto_r"]
+                                for datarn in range(span["from_r"], rng_upto_r):
+                                    if (
+                                        span["type_"] in val_modifying_options
+                                        and (datarn, oldidx) not in event_data["cells"]["table"]
+                                    ):
+                                        event_data["cells"]["table"][(datarn, oldidx)] = self.get_cell_data(datarn, k)
+                                    # create new cell options
+                                    new_ops(
+                                        mod_span(
+                                            qkspan,
+                                            span,
+                                            from_r=datarn,
+                                            upto_r=datarn + 1,
+                                            from_c=k,
+                                            upto_c=k + 1,
+                                        )
+                                    )
+                    # remove span specific kwargs from cells/columns
+                    # that are no longer in the span,
+                    # cell options/col options keys are new idxs
+                    for k in range(span["from_c"], oldupto_colrange):
+                        # has it moved outside of new span coords
                         if (
-                            span["header"]
-                            and full_new_idxs[k] in self.CH.cell_options
-                            and span["type_"] in self.CH.cell_options[full_new_idxs[k]]
-                        ):
-                            del self.CH.cell_options[full_new_idxs[k]][span["type_"]]
-                        # span is for col options
-                        if span["from_r"] is None:
+                            isinstance(newupto, int) and (full_new_idxs[k] < newfrom or full_new_idxs[k] >= newupto)
+                        ) or (newupto is None and full_new_idxs[k] < newfrom):
+                            # span includes header
                             if (
-                                full_new_idxs[k] in self.col_options
-                                and span["type_"] in self.col_options[full_new_idxs[k]]
+                                span["header"]
+                                and full_new_idxs[k] in self.CH.cell_options
+                                and span["type_"] in self.CH.cell_options[full_new_idxs[k]]
                             ):
-                                del self.col_options[full_new_idxs[k]][span["type_"]]
-                        # span is for cell options
-                        else:
-                            rng_upto_r = totalrows if span["upto_r"] is None else span["upto_r"]
-                            for r in range(span["from_r"], rng_upto_r):
-                                if (r, full_new_idxs[k]) in self.cell_options and span["type_"] in self.cell_options[
-                                    (r, full_new_idxs[k])
-                                ]:
-                                    del self.cell_options[(r, full_new_idxs[k])][span["type_"]]
-                # finally, change the span coords
-                span["from_c"], span["upto_c"] = newfrom, newupto
+                                del self.CH.cell_options[full_new_idxs[k]][span["type_"]]
+                            # span is for col options
+                            if span["from_r"] is None:
+                                if (
+                                    full_new_idxs[k] in self.col_options
+                                    and span["type_"] in self.col_options[full_new_idxs[k]]
+                                ):
+                                    del self.col_options[full_new_idxs[k]][span["type_"]]
+                            # span is for cell options
+                            else:
+                                rng_upto_r = totalrows if span["upto_r"] is None else span["upto_r"]
+                                for r in range(span["from_r"], rng_upto_r):
+                                    if (r, full_new_idxs[k]) in self.cell_options and span[
+                                        "type_"
+                                    ] in self.cell_options[(r, full_new_idxs[k])]:
+                                        del self.cell_options[(r, full_new_idxs[k])][span["type_"]]
+                    # finally, change the span coords
+                    span["from_c"], span["upto_c"] = newfrom, newupto
             if data_indexes:
                 self.displayed_columns = sorted(full_new_idxs[k] for k in self.displayed_columns)
         return data_new_idxs, disp_new_idxs, event_data
 
     def get_max_column_idx(self, maxidx: int | None = None) -> int:
         if maxidx is None:
             maxidx = len_to_idx(self.total_data_cols())
@@ -1212,109 +1215,112 @@
                 tags: {(full_new_idxs[k[0]], k[1]) for k in tagged} for tags, tagged in self.tagged_cells.items()
             }
             self.cell_options = {(full_new_idxs[k[0]], k[1]): v for k, v in self.cell_options.items()}
             self.tagged_rows = {tags: {full_new_idxs[k] for k in tagged} for tags, tagged in self.tagged_rows.items()}
             self.row_options = {full_new_idxs[k]: v for k, v in self.row_options.items()}
             self.RI.cell_options = {full_new_idxs[k]: v for k, v in self.RI.cell_options.items()}
             self.RI.tree_rns = {v: full_new_idxs[k] for v, k in self.RI.tree_rns.items()}
-            totalcols = self.total_data_cols()
-            new_ops = self.PAR.create_options_from_span
-            qkspan = self.span()
-            for span in self.named_spans.values():
-                # span is neither a cell options nor row options span, continue
-                if not isinstance(span["from_r"], int):
-                    continue
-                oldupto_rowrange, newupto_rowrange, newfrom, newupto = span_idxs_post_move(
-                    data_new_idxs,
-                    full_new_idxs,
-                    totalrows,
-                    span,
-                    "r",
-                )
-                # add cell/row kwargs for rows that are new to the span
-                old_span_idxs = set(full_new_idxs[k] for k in range(span["from_r"], oldupto_rowrange))
-                for k in range(newfrom, newupto_rowrange):
-                    if k not in old_span_idxs:
-                        oldidx = full_old_idxs[k]
-                        # event_data is used to preserve old cell value
-                        # in case cells are modified by
-                        # formatting, checkboxes, dropdown boxes
-                        if (
-                            span["type_"] in val_modifying_options
-                            and span["index"]
-                            and oldidx not in event_data["cells"]["index"]
-                        ):
-                            event_data["cells"]["index"][oldidx] = self.RI.get_cell_data(k)
-                        # the span targets rows
-                        if span["from_c"] is None:
-                            if span["type_"] in val_modifying_options:
-                                for datacn in range(len(self.data[k])):
-                                    if (oldidx, datacn) not in event_data["cells"]["table"]:
-                                        event_data["cells"]["table"][(oldidx, datacn)] = self.get_cell_data(k, datacn)
-                            # create new row options
-                            new_ops(
-                                mod_span(
-                                    qkspan,
-                                    span,
-                                    from_r=k,
-                                    upto_r=k + 1,
-                                )
-                            )
-                        # the span targets cells
-                        else:
-                            rng_upto_c = totalcols if span["upto_c"] is None else span["upto_c"]
-                            for datacn in range(span["from_c"], rng_upto_c):
-                                if (
-                                    span["type_"] in val_modifying_options
-                                    and (oldidx, datacn) not in event_data["cells"]["table"]
-                                ):
-                                    event_data["cells"]["table"][(oldidx, datacn)] = self.get_cell_data(k, datacn)
-                                # create new cell options
+            if self.named_spans:
+                totalcols = self.total_data_cols()
+                new_ops = self.PAR.create_options_from_span
+                qkspan = self.span()
+                for span in self.named_spans.values():
+                    # span is neither a cell options nor row options span, continue
+                    if not isinstance(span["from_r"], int):
+                        continue
+                    oldupto_rowrange, newupto_rowrange, newfrom, newupto = span_idxs_post_move(
+                        data_new_idxs,
+                        full_new_idxs,
+                        totalrows,
+                        span,
+                        "r",
+                    )
+                    # add cell/row kwargs for rows that are new to the span
+                    old_span_idxs = set(full_new_idxs[k] for k in range(span["from_r"], oldupto_rowrange))
+                    for k in range(newfrom, newupto_rowrange):
+                        if k not in old_span_idxs:
+                            oldidx = full_old_idxs[k]
+                            # event_data is used to preserve old cell value
+                            # in case cells are modified by
+                            # formatting, checkboxes, dropdown boxes
+                            if (
+                                span["type_"] in val_modifying_options
+                                and span["index"]
+                                and oldidx not in event_data["cells"]["index"]
+                            ):
+                                event_data["cells"]["index"][oldidx] = self.RI.get_cell_data(k)
+                            # the span targets rows
+                            if span["from_c"] is None:
+                                if span["type_"] in val_modifying_options:
+                                    for datacn in range(len(self.data[k])):
+                                        if (oldidx, datacn) not in event_data["cells"]["table"]:
+                                            event_data["cells"]["table"][(oldidx, datacn)] = self.get_cell_data(
+                                                k, datacn
+                                            )
+                                # create new row options
                                 new_ops(
                                     mod_span(
                                         qkspan,
                                         span,
                                         from_r=k,
                                         upto_r=k + 1,
-                                        from_c=datacn,
-                                        upto_c=datacn + 1,
                                     )
                                 )
-                # remove span specific kwargs from cells/rows
-                # that are no longer in the span,
-                # cell options/row options keys are new idxs
-                for k in range(span["from_r"], oldupto_rowrange):
-                    # has it moved outside of new span coords
-                    if (isinstance(newupto, int) and (full_new_idxs[k] < newfrom or full_new_idxs[k] >= newupto)) or (
-                        newupto is None and full_new_idxs[k] < newfrom
-                    ):
-                        # span includes index
+                            # the span targets cells
+                            else:
+                                rng_upto_c = totalcols if span["upto_c"] is None else span["upto_c"]
+                                for datacn in range(span["from_c"], rng_upto_c):
+                                    if (
+                                        span["type_"] in val_modifying_options
+                                        and (oldidx, datacn) not in event_data["cells"]["table"]
+                                    ):
+                                        event_data["cells"]["table"][(oldidx, datacn)] = self.get_cell_data(k, datacn)
+                                    # create new cell options
+                                    new_ops(
+                                        mod_span(
+                                            qkspan,
+                                            span,
+                                            from_r=k,
+                                            upto_r=k + 1,
+                                            from_c=datacn,
+                                            upto_c=datacn + 1,
+                                        )
+                                    )
+                    # remove span specific kwargs from cells/rows
+                    # that are no longer in the span,
+                    # cell options/row options keys are new idxs
+                    for k in range(span["from_r"], oldupto_rowrange):
+                        # has it moved outside of new span coords
                         if (
-                            span["index"]
-                            and full_new_idxs[k] in self.RI.cell_options
-                            and span["type_"] in self.RI.cell_options[full_new_idxs[k]]
-                        ):
-                            del self.RI.cell_options[full_new_idxs[k]][span["type_"]]
-                        # span is for row options
-                        if span["from_c"] is None:
+                            isinstance(newupto, int) and (full_new_idxs[k] < newfrom or full_new_idxs[k] >= newupto)
+                        ) or (newupto is None and full_new_idxs[k] < newfrom):
+                            # span includes index
                             if (
-                                full_new_idxs[k] in self.row_options
-                                and span["type_"] in self.row_options[full_new_idxs[k]]
+                                span["index"]
+                                and full_new_idxs[k] in self.RI.cell_options
+                                and span["type_"] in self.RI.cell_options[full_new_idxs[k]]
                             ):
-                                del self.row_options[full_new_idxs[k]][span["type_"]]
-                        # span is for cell options
-                        else:
-                            rng_upto_c = totalcols if span["upto_c"] is None else span["upto_c"]
-                            for c in range(span["from_c"], rng_upto_c):
-                                if (full_new_idxs[k], c) in self.cell_options and span["type_"] in self.cell_options[
-                                    (full_new_idxs[k], c)
-                                ]:
-                                    del self.cell_options[(full_new_idxs[k], c)][span["type_"]]
-                # finally, change the span coords
-                span["from_r"], span["upto_r"] = newfrom, newupto
+                                del self.RI.cell_options[full_new_idxs[k]][span["type_"]]
+                            # span is for row options
+                            if span["from_c"] is None:
+                                if (
+                                    full_new_idxs[k] in self.row_options
+                                    and span["type_"] in self.row_options[full_new_idxs[k]]
+                                ):
+                                    del self.row_options[full_new_idxs[k]][span["type_"]]
+                            # span is for cell options
+                            else:
+                                rng_upto_c = totalcols if span["upto_c"] is None else span["upto_c"]
+                                for c in range(span["from_c"], rng_upto_c):
+                                    if (full_new_idxs[k], c) in self.cell_options and span[
+                                        "type_"
+                                    ] in self.cell_options[(full_new_idxs[k], c)]:
+                                        del self.cell_options[(full_new_idxs[k], c)][span["type_"]]
+                    # finally, change the span coords
+                    span["from_r"], span["upto_r"] = newfrom, newupto
             if data_indexes:
                 self.displayed_rows = sorted(full_new_idxs[k] for k in self.displayed_rows)
         return data_new_idxs, disp_new_idxs, event_data
 
     def get_max_row_idx(self, maxidx: int | None = None) -> int:
         if maxidx is None:
             maxidx = len_to_idx(self.total_data_rows())
@@ -2781,14 +2787,15 @@
             or self.identify_row(y=event.y, allow_end=False) is None
         ):
             self.deselect("all")
         r = self.identify_row(y=event.y)
         c = self.identify_col(x=event.x)
         if self.single_selection_enabled and self.not_currently_resizing():
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
+                self.being_drawn_item = True
                 self.being_drawn_item = self.select_cell(r, c, redraw=True)
         elif self.toggle_selection_enabled and self.not_currently_resizing():
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.toggle_select_cell(r, c, redraw=True)
         self.b1_pressed_loc = (r, c)
@@ -3017,15 +3024,19 @@
             self.hide_selection_box(self.being_drawn_item)
             self.being_drawn_item = None
             self.set_currently_selected(
                 r_to_sel,
                 c_to_sel,
                 item=self.create_selection_box(
                     *to_sel,
-                    state="hidden" if (to_sel[2] - to_sel[0] == 1 and to_sel[3] - to_sel[1] == 1) else "normal",
+                    state=(
+                        "hidden"
+                        if (to_sel.upto_r - to_sel.from_r == 1 and to_sel.upto_c - to_sel.from_c == 1)
+                        else "normal"
+                    ),
                     set_current=False,
                 ),
             )
             sel_event = self.get_select_event(being_drawn_item=self.being_drawn_item)
             if self.drag_selection_binding_func:
                 self.drag_selection_binding_func(sel_event)
             self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
@@ -5143,15 +5154,15 @@
         x2: int | float,
         y2: int | float,
         fill: str,
         outline: str,
         tag: str | tuple,
         draw_check: bool = False,
     ) -> None:
-        points = get_checkbox_points(x1, y1, x2, y2)
+        points = rounded_box_coords(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
                 self.itemconfig(t, fill=outline, outline=fill, tag=tag, state="normal")
@@ -5160,15 +5171,15 @@
             t = self.create_polygon(points, fill=outline, outline=fill, tag=tag, smooth=True)
         self.disp_checkbox[t] = True
         if draw_check:
             x1 = x1 + 4
             y1 = y1 + 4
             x2 = x2 - 3
             y2 = y2 - 3
-            points = get_checkbox_points(x1, y1, x2, y2, radius=4)
+            points = rounded_box_coords(x1, y1, x2, y2, radius=4)
             if self.hidd_checkbox:
                 t, sh = self.hidd_checkbox.popitem()
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill, outline=outline)
                 else:
                     self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
@@ -5792,32 +5803,42 @@
         x2: int,
         y2: int,
         fill: str,
         outline: str,
         state: str,
         tags: str | tuple[str],
         width: int,
+        iid: None | int = None,
     ) -> int:
-        if self.hidd_boxes:
-            iid = self.hidd_boxes.pop()
+        coords = rounded_box_coords(
+            x1,
+            y1,
+            x2,
+            y2,
+            radius=9 if self.PAR.ops.rounded_boxes else 0,
+        )
+        if isinstance(iid, int):
             self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags, width=width)
-            self.coords(iid, x1, y1, x2, y2)
+            self.coords(iid, coords)
         else:
-            iid = self.create_rectangle(
-                x1,
-                y1,
-                x2,
-                y2,
-                fill=fill,
-                outline=outline,
-                state=state,
-                tags=tags,
-                width=width,
-            )
-        self.disp_boxes.add(iid)
+            if self.hidd_boxes:
+                iid = self.hidd_boxes.pop()
+                self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags, width=width)
+                self.coords(iid, coords)
+            else:
+                iid = self.create_polygon(
+                    coords,
+                    fill=fill,
+                    outline=outline,
+                    state=state,
+                    tags=tags,
+                    width=width,
+                    smooth=True,
+                )
+            self.disp_boxes.add(iid)
         return iid
 
     def hide_box(self, item: int | None) -> None:
         if isinstance(item, int):
             self.disp_boxes.discard(item)
             self.hidd_boxes.add(item)
             self.itemconfig(item, state="hidden")
@@ -5862,37 +5883,40 @@
             mt_border_col = self.PAR.ops.table_selected_cells_border_fg
         elif type_ == "rows":
             mt_bg = self.PAR.ops.table_selected_rows_bg
             mt_border_col = self.PAR.ops.table_selected_rows_border_fg
         elif type_ == "columns":
             mt_bg = self.PAR.ops.table_selected_columns_bg
             mt_border_col = self.PAR.ops.table_selected_columns_border_fg
+        if self.selection_boxes:
+            self.itemconfig(next(reversed(self.selection_boxes)), state="normal")
+        x1, y1, x2, y2 = self.box_sheet_coords_x_canvas_coords(r1, c1, r2, c2, type_)
         fill_iid = self.display_box(
-            self.col_positions[c1],
-            self.row_positions[r1],
-            self.canvasx(self.winfo_width()) if self.PAR.ops.selected_rows_to_end_of_window else self.col_positions[c2],
-            self.row_positions[r2],
+            x1,
+            y1,
+            x2,
+            y2,
             fill=mt_bg,
             outline="",
-            state=state,
+            state=state if self.PAR.ops.show_selected_cells_border else "normal",
             tags=type_,
             width=1,
         )
         index_iid = self.RI.display_box(
-            0,
-            self.row_positions[r1],
+            1,
+            y1,
             self.RI.current_width - 1,
-            self.row_positions[r2],
+            y2,
             fill=self.PAR.ops.index_selected_rows_bg if type_ == "rows" else self.PAR.ops.index_selected_cells_bg,
             outline="",
             state="normal",
             tags="cells" if type_ == "columns" else type_,
         )
         header_iid = self.CH.display_box(
-            self.col_positions[c1],
+            x1,
             0,
             self.col_positions[c2],
             self.CH.current_height - 1,
             fill=(
                 self.PAR.ops.header_selected_columns_bg if type_ == "columns" else self.PAR.ops.header_selected_cells_bg
             ),
             outline="",
@@ -5901,18 +5925,18 @@
         )
         bd_iid = None
         if self.PAR.ops.show_selected_cells_border and (
             (self.being_drawn_item is None and self.RI.being_drawn_item is None and self.CH.being_drawn_item is None)
             or self.selection_boxes
         ):
             bd_iid = self.display_box(
-                self.col_positions[c1],
-                self.row_positions[r1],
-                self.col_positions[c2],
-                self.row_positions[r2],
+                x1,
+                y1,
+                x2,
+                y2,
                 fill="",
                 outline=mt_border_col,
                 state="normal",
                 tags=f"{type_}bd",
                 width=1,
             )
             self.tag_raise(bd_iid)
@@ -5947,14 +5971,31 @@
             self.RI.tag_lower("rows")
             self.RI.tag_lower("cells")
             self.CH.tag_lower("columns")
             self.CH.tag_lower("cells")
             if self.PAR.ops.show_selected_cells_border:
                 self.tag_raise(self.selected.iid)
 
+    def box_sheet_coords_x_canvas_coords(
+        self,
+        r1: int,
+        c1: int,
+        r2: int,
+        c2: int,
+        type_: Literal["cells", "rows", "columns"],
+    ) -> tuple[float, float, float, float]:
+        x1 = self.col_positions[c1]
+        y1 = self.row_positions[r1]
+        y2 = self.row_positions[r2]
+        if type_ == "rows" and self.PAR.ops.selected_rows_to_end_of_window:
+            x2 = self.canvasx(self.winfo_width())
+        else:
+            x2 = self.col_positions[c2]
+        return x1, y1, x2, y2
+
     def recreate_selection_box(
         self,
         r1: int,
         c1: int,
         r2: int,
         c2: int,
         fill_iid: int,
@@ -5969,74 +6010,61 @@
         elif type_ == "rows":
             mt_bg = self.PAR.ops.table_selected_rows_bg
             mt_border_col = self.PAR.ops.table_selected_rows_border_fg
         elif type_ == "columns":
             mt_bg = self.PAR.ops.table_selected_columns_bg
             mt_border_col = self.PAR.ops.table_selected_columns_border_fg
         if not state:
-            state = "normal" if (r2 - r1 > 1 or c2 - c1 > 1) else "hidden"
+            if r2 - r1 > 1 or c2 - c1 > 1:
+                state = "normal"
+            elif next(reversed(self.selection_boxes)) == fill_iid:
+                state = "hidden"
+            else:
+                state = "normal"
         if self.selected.fill_iid == fill_iid:
             self.selected = self.selected._replace(box=Box_nt(r1, c1, r2, c2))
-        self.coords(
-            fill_iid,
-            self.col_positions[c1],
-            self.row_positions[r1],
-            self.canvasx(self.winfo_width()) if self.PAR.ops.selected_rows_to_end_of_window else self.col_positions[c2],
-            self.row_positions[r2],
-        )
-        self.itemconfig(
-            fill_iid,
-            fill=mt_bg,
-            outline="",
-            tags=type_,
-            state=state,
-        )
-        self.RI.coords(
-            self.selection_boxes[fill_iid].index,
-            0,
-            self.row_positions[r1],
+        x1, y1, x2, y2 = self.box_sheet_coords_x_canvas_coords(r1, c1, r2, c2, type_)
+        self.display_box(x1, y1, x2, y2, fill=mt_bg, outline="", state=state, tags=type_, width=1, iid=fill_iid)
+        self.RI.display_box(
+            1,
+            y1,
             self.RI.current_width - 1,
-            self.row_positions[r2],
-        )
-        self.RI.itemconfig(
-            self.selection_boxes[fill_iid].index,
+            y2,
             fill=self.PAR.ops.index_selected_rows_bg if type_ == "rows" else self.PAR.ops.index_selected_cells_bg,
             outline="",
+            state="normal",
             tags="cells" if type_ == "columns" else type_,
+            iid=self.selection_boxes[fill_iid].index,
         )
-        self.CH.coords(
-            self.selection_boxes[fill_iid].header,
-            self.col_positions[c1],
+        self.CH.display_box(
+            x1,
             0,
             self.col_positions[c2],
             self.CH.current_height - 1,
-        )
-        self.CH.itemconfig(
-            self.selection_boxes[fill_iid].header,
             fill=(
                 self.PAR.ops.header_selected_columns_bg if type_ == "columns" else self.PAR.ops.header_selected_cells_bg
             ),
             outline="",
+            state="normal",
             tags="cells" if type_ == "rows" else type_,
+            iid=self.selection_boxes[fill_iid].header,
         )
-        if bd_iid := self.selection_boxes[fill_iid].bd_iid:
+        if (bd_iid := self.selection_boxes[fill_iid].bd_iid):
             if self.PAR.ops.show_selected_cells_border:
-                self.coords(
-                    bd_iid,
-                    self.col_positions[c1],
-                    self.row_positions[r1],
-                    self.col_positions[c2],
-                    self.row_positions[r2],
-                )
-                self.itemconfig(
-                    bd_iid,
+                self.display_box(
+                    x1,
+                    y1,
+                    x2,
+                    y2,
                     fill="",
                     outline=mt_border_col,
-                    tags=f"{type_}bd",
                     state="normal",
+                    tags=f"{type_}bd",
+                    width=1,
+                    iid=bd_iid,
                 )
                 self.tag_raise(bd_iid)
             else:
                 self.hide_box(bd_iid)
         if run_binding:
             self.run_selection_binding(type_)
         return fill_iid
@@ -6075,31 +6103,31 @@
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.set_currently_selected(r, c, item=self.selected.fill_iid)
             else:
                 box = self.selection_boxes[self.selected.fill_iid]
                 self.set_currently_selected(box.coords.from_r, box.coords.from_c, item=box.fill_iid)
 
     def get_redraw_selections(self, startr: int, endr: int, startc: int, endc: int) -> dict:
-        d = defaultdict(list)
+        d = defaultdict(set)
         for item, box in self.get_selection_items():
-            d[box.type_].append(box.coords)
-        d2 = {}
-        if "cells" in d:
-            d2["cells"] = {
-                (r, c)
-                for r in range(startr, endr)
-                for c in range(startc, endc)
-                for r1, c1, r2, c2 in d["cells"]
-                if r1 <= r and c1 <= c and r2 > r and c2 > c
-            }
-        if "rows" in d:
-            d2["rows"] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d["rows"] if r1 <= r and r2 > r}
-        if "columns" in d:
-            d2["columns"] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d["columns"] if c1 <= c and c2 > c}
-        return d2
+            r1, c1, r2, c2 = box.coords
+            if box.type_ == "cells":
+                for r in range(startr, endr):
+                    for c in range(startc, endc):
+                        if r1 <= r and c1 <= c and r2 > r and c2 > c:
+                            d["cells"].add((r, c))
+            elif box.type_ == "rows":
+                for r in range(startr, endr):
+                    if r1 <= r and r2 > r:
+                        d["rows"].add(r)
+            elif box.type_ == "columns":
+                for c in range(startc, endc):
+                    if c1 <= c and c2 > c:
+                        d["columns"].add(c)
+        return d
 
     def get_selected_min_max(self) -> tuple[int, int, int, int] | tuple[None, None, None, None]:
         min_x = float("inf")
         min_y = float("inf")
         max_x = 0
         max_y = 0
         for item, box in self.get_selection_items():
@@ -6595,14 +6623,16 @@
                     self.col_positions[c],
                     self.row_positions[r],
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
+            for b in ("<Alt-Return>", "<Option-Return>", "<Tab>", "<Return>", "<FocusOut>", "<Escape>"):
+                self.text_editor.tktext.unbind(b)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     def close_text_editor(
         self,
@@ -6617,23 +6647,23 @@
             pass
         if focused is None and editor_info:
             return "break"
         if editor_info[2] == "Escape":
             self.hide_text_editor_and_dropdown()
             return
         # setting cell data with text editor value
-        self.text_editor_value = self.text_editor.get()
+        text_editor_value = self.text_editor.get()
         r, c = editor_info[0], editor_info[1]
         datarn, datacn = self.datarn(r), self.datacn(c)
         event_data = event_dict(
             name="end_edit_table",
             sheet=self.PAR.name,
-            cells_table={(datarn, datacn): self.text_editor_value},
+            cells_table={(datarn, datacn): text_editor_value},
             key=editor_info[2],
-            value=self.text_editor_value,
+            value=text_editor_value,
             loc=(r, c),
             boxes=self.get_boxes(),
             selected=self.selected,
         )
         edited = False
         set_data = partial(
             self.set_cell_data_undo,
@@ -6641,29 +6671,29 @@
             c=c,
             datarn=datarn,
             datacn=datacn,
             redraw=False,
             check_input_valid=False,
         )
         if self.edit_validation_func:
-            self.text_editor_value = self.edit_validation_func(event_data)
-            if self.text_editor_value is not None and self.input_valid_for_cell(datarn, datacn, self.text_editor_value):
-                edited = set_data(value=self.text_editor_value)
-        elif self.input_valid_for_cell(datarn, datacn, self.text_editor_value):
-            edited = set_data(value=self.text_editor_value)
+            text_editor_value = self.edit_validation_func(event_data)
+            if text_editor_value is not None and self.input_valid_for_cell(datarn, datacn, text_editor_value):
+                edited = set_data(value=text_editor_value)
+        elif self.input_valid_for_cell(datarn, datacn, text_editor_value):
+            edited = set_data(value=text_editor_value)
         if edited:
             try_binding(self.extra_end_edit_cell_func, event_data)
         if (
             r is not None
             and c is not None
             and self.selected
             and r == self.selected.row
             and c == self.selected.column
             and (self.single_selection_enabled or self.toggle_selection_enabled)
-            and (edited or self.cell_equal_to(datarn, datacn, self.text_editor_value))
+            and (edited or self.cell_equal_to(datarn, datacn, text_editor_value))
         ):
             r1, c1, r2, c2 = self.selection_boxes[self.selected.fill_iid].coords
             numcols = c2 - c1
             numrows = r2 - r1
             if numcols == 1 and numrows == 1:
                 if editor_info[2] == "Return":
                     self.select_cell(r + 1 if r < len(self.row_positions) - 2 else r, c)
@@ -6973,14 +7003,15 @@
     def mouseclick_outside_editor_or_dropdown_all_canvases(self):
         self.CH.mouseclick_outside_editor_or_dropdown()
         self.RI.mouseclick_outside_editor_or_dropdown()
         return self.mouseclick_outside_editor_or_dropdown()
 
     def hide_dropdown_window(self) -> None:
         if self.dropdown.open:
+            self.dropdown.window.unbind("<FocusOut>")
             self.itemconfig(self.dropdown.canvas_id, state="hidden")
             self.dropdown.open = False
 
     def click_checkbox(
         self,
         r: int,
         c: int,
@@ -7024,20 +7055,22 @@
     # internal event use
     def set_cell_data_undo(
         self,
         r: int = 0,
         c: int = 0,
         datarn: int | None = None,
         datacn: int | None = None,
-        value: str = "",
+        value: str | None = None,
         undo: bool = True,
         cell_resize: bool = True,
         redraw: bool = True,
         check_input_valid: bool = True,
     ) -> bool:
+        if value is None:
+            value = ""
         if datacn is None:
             datacn = self.datacn(c)
         if datarn is None:
             datarn = self.datarn(r)
         event_data = event_dict(
             name="edit_table",
             sheet=self.PAR.name,
```

### Comparing `tksheet-7.1.6/tksheet/other_classes.py` & `tksheet-7.1.7/tksheet/other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/tksheet/row_index.py` & `tksheet-7.1.7/tksheet/row_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     is_bool_like,
     try_to_bool,
 )
 from .functions import (
     consecutive_chunks,
     ev_stack_dict,
     event_dict,
-    get_checkbox_points,
+    rounded_box_coords,
     get_n2a,
     is_contiguous,
     num2alpha,
     try_binding,
 )
 from .other_classes import (
     DotDict,
@@ -401,15 +401,15 @@
                 if (
                     self.get_cell_kwargs(datarn, key="dropdown")
                     or self.get_cell_kwargs(datarn, key="checkbox")
                     or self.edit_cell_enabled
                 ):
                     self.open_cell(event)
                 elif (iid := self.event_over_tree_arrow(r, self.canvasy(event.y), event.x)) is not None:
-                    self.PAR.item(iid, open_=iid not in self.tree_open_ids)
+                    self.PAR.item(iid, open_=iid not in self.tree_open_ids, redraw=False)
         self.rsz_h = None
         self.mouse_motion(event)
         try_binding(self.extra_double_b1_func, event)
 
     def b1_press(self, event: object):
         self.MT.unbind("<MouseWheel>")
         self.focus_set()
@@ -865,15 +865,15 @@
                 if self.event_over_dropdown(r, datarn, event, canvasy) or self.event_over_checkbox(
                     r, datarn, event, canvasy
                 ):
                     self.open_cell(event)
                 elif (iid := self.event_over_tree_arrow(r, canvasy, event.x)) is not None:
                     if self.MT.selection_boxes:
                         self.select_row(r, redraw=False)
-                    self.PAR.item(iid, open_=iid not in self.tree_open_ids)
+                    self.PAR.item(iid, open_=iid not in self.tree_open_ids, redraw=False)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases(inside=True)
             self.b1_pressed_loc = None
             self.closed_dropdown = None
         self.dragged_row = None
         self.currently_resizing_width = False
         self.currently_resizing_height = False
@@ -954,22 +954,41 @@
         y1: int,
         x2: int,
         y2: int,
         fill: str,
         outline: str,
         state: str,
         tags: str | tuple[str],
+        iid: None | int = None,
     ) -> int:
-        if self.hidd_boxes:
-            iid = self.hidd_boxes.pop()
-            self.coords(iid, x1, y1, x2, y2)
+        coords = rounded_box_coords(
+            x1,
+            y1,
+            x2,
+            y2,
+            radius=9 if self.PAR.ops.rounded_boxes else 0,
+        )
+        if isinstance(iid, int):
+            self.coords(iid, coords)
             self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags)
         else:
-            iid = self.create_rectangle(x1, y1, x2, y2, fill=fill, outline=outline, state=state, tags=tags)
-        self.disp_boxes.add(iid)
+            if self.hidd_boxes:
+                iid = self.hidd_boxes.pop()
+                self.coords(iid, coords)
+                self.itemconfig(iid, fill=fill, outline=outline, state=state, tags=tags)
+            else:
+                iid = self.create_polygon(
+                    coords,
+                    fill=fill,
+                    outline=outline,
+                    state=state,
+                    tags=tags,
+                    smooth=True,
+                )
+            self.disp_boxes.add(iid)
         return iid
 
     def hide_box(self, item: int | None) -> None:
         if isinstance(item, int):
             self.disp_boxes.discard(item)
             self.hidd_boxes.add(item)
             self.itemconfig(item, state="hidden")
@@ -1337,15 +1356,15 @@
                     capstyle=tk.ROUND,
                     joinstyle=tk.ROUND,
                     tag=tag,
                 )
             self.disp_dropdown[t] = True
 
     def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check=False):
-        points = get_checkbox_points(x1, y1, x2, y2)
+        points = rounded_box_coords(x1, y1, x2, y2)
         if self.hidd_checkbox:
             t, sh = self.hidd_checkbox.popitem()
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
                 self.itemconfig(t, fill=outline, outline=fill, tag=tag, state="normal")
@@ -1355,15 +1374,15 @@
         self.disp_checkbox[t] = True
         if draw_check:
             # draw filled box
             x1 = x1 + 4
             y1 = y1 + 4
             x2 = x2 - 3
             y2 = y2 - 3
-            points = get_checkbox_points(x1, y1, x2, y2, radius=4)
+            points = rounded_box_coords(x1, y1, x2, y2, radius=4)
             if self.hidd_checkbox:
                 t, sh = self.hidd_checkbox.popitem()
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill, outline=outline)
                 else:
                     self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
@@ -1655,24 +1674,22 @@
         for dct in (self.hidd_text, self.hidd_high, self.hidd_grid, self.hidd_dropdown, self.hidd_checkbox):
             for iid, showing in dct.items():
                 if showing:
                     self.itemconfig(iid, state="hidden")
                     dct[iid] = False
         return True
 
-    def get_redraw_selections(self, startr, endr):
-        d = defaultdict(list)
+    def get_redraw_selections(self, startr: int, endr: int) -> dict[str, set[int]]:
+        d = defaultdict(set)
         for item, box in self.MT.get_selection_items(columns=False):
-            d[box.type_].append(box.coords)
-        d2 = {}
-        if "cells" in d:
-            d2["cells"] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d["cells"] if r1 <= r and r2 > r}
-        if "rows" in d:
-            d2["rows"] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d["rows"] if r1 <= r and r2 > r}
-        return d2
+            r1, c1, r2, c2 = box.coords
+            for r in range(startr, endr):
+                if r1 <= r and r2 > r:
+                    d[box.type_].add(r)
+        return d
 
     def open_cell(self, event: object = None, ignore_existing_editor=False):
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor.open):
             return
         if not self.MT.selected:
             return
         r = self.MT.selected.row
@@ -1888,14 +1905,16 @@
                     0,
                     self.MT.row_positions[r],
                 )
                 # self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def hide_text_editor(self, reason: None | str = None) -> None:
         if self.text_editor.open:
+            for b in ("<Alt-Return>", "<Option-Return>", "<Tab>", "<Return>", "<FocusOut>", "<Escape>"):
+                self.text_editor.tktext.unbind(b)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     # r is displayed row
     def close_text_editor(
@@ -1909,40 +1928,40 @@
         except Exception:
             pass
         if focused is None and editor_info:
             return "break"
         if editor_info is not None and len(editor_info) >= 2 and editor_info[1] == "Escape":
             self.hide_text_editor_and_dropdown()
             return
-        self.text_editor_value = self.text_editor.get()
+        text_editor_value = self.text_editor.get()
         r = editor_info[0]
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         event_data = event_dict(
             name="end_edit_index",
             sheet=self.PAR.name,
             cells_index={datarn: self.get_cell_data(datarn)},
             key=editor_info[1] if len(editor_info) >= 2 else "FocusOut",
-            value=self.text_editor_value,
+            value=text_editor_value,
             loc=r,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
         set_data = partial(
             self.set_cell_data_undo,
             r=r,
             datarn=datarn,
             check_input_valid=False,
         )
         if self.MT.edit_validation_func:
-            self.text_editor_value = self.MT.edit_validation_func(event_data)
-            if self.text_editor_value is not None and self.input_valid_for_cell(datarn, self.text_editor_value):
-                edited = set_data(value=self.text_editor_value)
-        elif self.input_valid_for_cell(datarn, self.text_editor_value):
-            edited = set_data(value=self.text_editor_value)
+            text_editor_value = self.MT.edit_validation_func(event_data)
+            if text_editor_value is not None and self.input_valid_for_cell(datarn, text_editor_value):
+                edited = set_data(value=text_editor_value)
+        elif self.input_valid_for_cell(datarn, text_editor_value):
+            edited = set_data(value=text_editor_value)
         if edited:
             try_binding(self.extra_end_edit_cell_func, event_data)
         self.MT.recreate_all_selection_boxes()
         self.hide_text_editor_and_dropdown()
         if editor_info[1] != "FocusOut":
             self.focus_set()
         return "break"
@@ -2121,14 +2140,15 @@
     def mouseclick_outside_editor_or_dropdown_all_canvases(self, inside: bool = False):
         self.CH.mouseclick_outside_editor_or_dropdown()
         self.MT.mouseclick_outside_editor_or_dropdown()
         return self.mouseclick_outside_editor_or_dropdown(inside)
 
     def hide_dropdown_window(self) -> None:
         if self.dropdown.open:
+            self.dropdown.window.unbind("<FocusOut>")
             self.itemconfig(self.dropdown.canvas_id, state="hidden")
             self.dropdown.open = False
 
     # internal event use
     def set_cell_data_undo(
         self,
         r: int = 0,
```

### Comparing `tksheet-7.1.6/tksheet/sheet.py` & `tksheet-7.1.7/tksheet/sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,17 @@
         horizontal_grid_to_end_of_window: bool = False,
         vertical_grid_to_end_of_window: bool = False,
         show_vertical_grid: bool = True,
         show_horizontal_grid: bool = True,
         display_selected_fg_over_highlights: bool = False,
         show_selected_cells_border: bool = True,
         treeview: bool = False,
+        treeview_indent: str | int = "3",
+        rounded_boxes: bool = True,
+        alternate_color: str = "",
         # colors
         outline_thickness: int = 0,
         outline_color: str = theme_light_blue["outline_color"],
         theme: str = "light blue",
         frame_bg: str = theme_light_blue["table_bg"],
         popup_menu_fg: str = theme_light_blue["popup_menu_fg"],
         popup_menu_bg: str = theme_light_blue["popup_menu_bg"],
@@ -3791,16 +3794,14 @@
                 itr=self.MT.gen_row_heights,
                 to_pop=to_pop,
                 save_to=self.MT.saved_row_heights,
             ),
         )
         if deselect_all:
             self.MT.deselect(redraw=False)
-        else:
-            self.MT.deselect_any(rows=rows, redraw=False)
         self.set_refresh_timer(redraw)
         return self
 
     # uses data indexes
     def show_rows(
         self,
         rows: int | Iterator[int],
@@ -4554,14 +4555,15 @@
     def item(
         self,
         item: str,
         iid: str | None = None,
         text: str | None = None,
         values: list | None = None,
         open_: bool | None = None,
+        redraw: bool = True,
     ) -> DotDict | Sheet:
         """
         Modify options for item
         If no options are set then returns DotDict of options for item
         Else returns Sheet
         """
         if not (item := item.lower()) or item not in self.RI.tree:
@@ -4596,15 +4598,15 @@
                         redraw=False,
                         deselect_all=False,
                         data_indexes=True,
                     )
             else:
                 self.RI.tree_open_ids.discard(item)
         get = not (isinstance(iid, str) or isinstance(text, str) or isinstance(values, list) or isinstance(open_, bool))
-        self.set_refresh_timer(redraw=not get)
+        self.set_refresh_timer(redraw=not get or redraw)
         if get:
             return DotDict(
                 text=self.RI.tree[item].text,
                 values=self[self.RI.tree_rns[item]].options(ndim=1).data,
                 open_=item in self.RI.tree_open_ids,
             )
         return self
@@ -4612,18 +4614,19 @@
     def itemrow(self, item: str) -> int:
         try:
             return self.RI.tree_rns[item.lower()]
         except Exception:
             raise ValueError(f"item '{item.lower()}' does not exist.")
 
     def rowitem(self, row: int, data_index: bool = False) -> str | None:
-        if not data_index:
-            row = self.data_r(row)
-        if isinstance(row, int) and len(self.MT._row_index) > row:
-            return self.MT._row_index[row].iid
+        if isinstance(row, int):
+            if not data_index:
+                row = self.data_r(row)
+            if len(self.MT._row_index) > row:
+                return self.MT._row_index[row].iid
         return None
 
     def get_children(self, item: None | str = None) -> Generator[str]:
         if item is None:
             for n in self.RI.tree.values():
                 if not n.parent:
                     yield n.iid
@@ -4656,75 +4659,31 @@
             self.RI.tree_open_ids.discard(iid)
             if self.RI.tree[iid].parent and len(self.RI.tree[iid].parent.children) == 1:
                 self.RI.tree_open_ids.discard(self.RI.tree[iid].parent.iid)
             del self.RI.tree[iid]
         self.set_refresh_timer(True)
         return self
 
-    def set_children(self, item: str, *newchildren) -> Sheet:
+    def set_children(self, parent: str, *newchildren) -> Sheet:
         """
-        Moves everything in '*newchildren' under 'item'
+        Moves everything in '*newchildren' under 'parent'
         """
-        if (item := item.lower()) and item not in self.RI.tree:
-            raise ValueError(f"Item '{item}' does not exist.")
-        mapping = {}
-        to_show = []
-        if item:
-            new_parent = self.RI.tree[item]
-            if new_parent.children:
-                ctr = self.RI.tree_rns[new_parent.children[-1].iid] + 1
-            else:
-                ctr = self.RI.tree_rns[new_parent.iid] + 1
-            for cid in unpack(newchildren):
-                if self.RI.pid_causes_recursive_loop(cid, item):
-                    raise ValueError(f"iid '{cid}' causes a recursive loop with parent '{item}'.")
-                cid_node = self.RI.tree[cid]
-                mapping[self.RI.tree_rns[cid]] = ctr
-                if item in self.RI.tree_open_ids and self.item_displayed(item):
-                    to_show.append(ctr)
-                ctr += 1
-                for did in self.RI.get_iid_descendants(cid):
-                    mapping[self.RI.tree_rns[did]] = ctr
-                    if to_show and self.RI.ancestors_all_open(did, self.RI.tree[cid].parent):
-                        to_show.append(ctr)
-                    ctr += 1
-                self.RI.remove_node_from_parents_children(cid_node)
-                cid_node.parent = new_parent
-                new_parent.children.append(cid_node)
-        else:
-            ctr = (
-                len(self.MT._row_index)
-                - len(newchildren)
-                - sum(1 for cid in unpack(newchildren) for _ in self.RI.get_iid_descendants(cid))
-            )
-            for cid in unpack(newchildren):
-                cid_node = self.RI.tree[cid]
-                mapping[self.RI.tree_rns[cid]] = ctr
-                to_show.append(ctr)
-                ctr += 1
-                for did in self.RI.get_iid_descendants(cid):
-                    mapping[self.RI.tree_rns[did]] = ctr
-                    if self.RI.ancestors_all_open(did, cid_node.parent):
-                        to_show.append(ctr)
-                    ctr += 1
-                self.RI.remove_node_from_parents_children(cid_node)
-                self.RI.tree[cid].parent = ""
-        self.mapping_move_rows(
-            data_new_idxs=mapping,
-            data_indexes=True,
-            create_selections=False,
-            redraw=False,
-        )
-        if item and (item not in self.RI.tree_open_ids or not self.item_displayed(item)):
-            self.hide_rows(set(mapping.values()), data_indexes=True)
-        self.show_rows(to_show)
-        self.set_refresh_timer(True)
+        for iid in unpack(newchildren):
+            self.move(iid, parent)
         return self
 
-    def move(self, item: str, parent: str, index: int = 0) -> Sheet:
+    def find_rn_at_top_index(self, index: int) -> int:
+        wo_par = 0
+        for rn, n in enumerate(self.MT._row_index):
+            if not n.parent:
+                if wo_par == index:
+                    return rn
+                wo_par += 1
+
+    def move(self, item: str, parent: str, index: int | None = None) -> Sheet:
         """
         Moves item to be under parent as child at index
         'parent' can be empty string which will make item a top node
         """
         if (item := item.lower()) and item not in self.RI.tree:
             raise ValueError(f"Item '{item}' does not exist.")
         if (parent := parent.lower()) and parent not in self.RI.tree:
@@ -4733,43 +4692,57 @@
         to_show = []
         item_node = self.RI.tree[item]
         if parent:
             if self.RI.pid_causes_recursive_loop(item, parent):
                 raise ValueError(f"iid '{item}' causes a recursive loop with parent '{parent}'.")
             parent_node = self.RI.tree[parent]
             if parent_node.children:
-                if len(parent_node.children) < index:
-                    index = len(parent_node.children)
-                ctr = self.RI.tree_rns[parent_node.children[index].iid]
+                if index is None or index >= len(parent_node.children):
+                    index = len(parent_node.children) - 1
+                item_r = self.RI.tree_rns[item]
+                new_r = self.RI.tree_rns[parent_node.children[index].iid]
+                if item_node not in parent_node.children:
+                    new_r += 1
+                new_r_desc = sum(1 for _ in self.RI.get_iid_descendants(parent_node.children[index].iid))
+                item_desc = sum(1 for _ in self.RI.get_iid_descendants(item))
+                if item_r < new_r:
+                    r_ctr = new_r + new_r_desc - item_desc
+                else:
+                    r_ctr = new_r
             else:
-                ctr = self.RI.tree_rns[parent_node.iid] + 1
-            mapping[self.RI.tree_rns[item]] = ctr
+                r_ctr = self.RI.tree_rns[parent_node.iid] + 1
+            mapping[item_r] = r_ctr
             if parent in self.RI.tree_open_ids and self.item_displayed(parent):
-                to_show.append(ctr)
-            ctr += 1
+                to_show.append(r_ctr)
+            r_ctr += 1
             for did in self.RI.get_iid_descendants(item):
-                mapping[self.RI.tree_rns[did]] = ctr
+                mapping[self.RI.tree_rns[did]] = r_ctr
                 if to_show and self.RI.ancestors_all_open(did, item_node.parent):
-                    to_show.append(ctr)
-                ctr += 1
+                    to_show.append(r_ctr)
+                r_ctr += 1
             self.RI.remove_node_from_parents_children(item_node)
             item_node.parent = parent_node
             parent_node.children.append(item_node)
         else:
-            if len(self.MT._row_index) < index:
-                index = len(self.MT._row_index)
-            ctr = index
-            mapping[self.RI.tree_rns[item]] = ctr
-            to_show.append(ctr)
-            ctr += 1
+            new_r = self.find_rn_at_top_index((sum(1 for _ in self.get_children("")) - 1) if index is None else index)
+            item_r = self.RI.tree_rns[item]
+            if item_r < new_r:
+                par_desc = sum(1 for _ in self.RI.get_iid_descendants(self.rowitem(new_r, data_index=True)))
+                item_desc = sum(1 for _ in self.RI.get_iid_descendants(item))
+                r_ctr = new_r + par_desc - item_desc
+            else:
+                r_ctr = new_r
+            mapping[item_r] = r_ctr
+            to_show.append(r_ctr)
+            r_ctr += 1
             for did in self.RI.get_iid_descendants(item):
-                mapping[self.RI.tree_rns[did]] = ctr
+                mapping[self.RI.tree_rns[did]] = r_ctr
                 if to_show and self.RI.ancestors_all_open(did, item_node.parent):
-                    to_show.append(ctr)
-                ctr += 1
+                    to_show.append(r_ctr)
+                r_ctr += 1
             self.RI.remove_node_from_parents_children(item_node)
             self.RI.tree[item].parent = ""
         self.mapping_move_rows(
             data_new_idxs=mapping,
             data_indexes=True,
             create_selections=False,
             redraw=False,
```

### Comparing `tksheet-7.1.6/tksheet/sheet_options.py` & `tksheet-7.1.7/tksheet/sheet_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,10 +230,12 @@
             "horizontal_grid_to_end_of_window": False,
             "vertical_grid_to_end_of_window": False,
             "show_vertical_grid": True,
             "show_horizontal_grid": True,
             "display_selected_fg_over_highlights": False,
             "show_selected_cells_border": True,
             "treeview": False,
-            "treeview_indent": "2",
+            "treeview_indent": "3",
+            "rounded_boxes": True,
+            "alternate_color": "",
         }
     )
```

### Comparing `tksheet-7.1.6/tksheet/text_editor.py` & `tksheet-7.1.7/tksheet/text_editor.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/tksheet/themes.py` & `tksheet-7.1.7/tksheet/themes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/tksheet/top_left_rectangle.py` & `tksheet-7.1.7/tksheet/top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/tksheet/vars.py` & `tksheet-7.1.7/tksheet/vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.6/tksheet.egg-info/PKG-INFO` & `tksheet-7.1.7/tksheet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.6
+Version: 7.1.7
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

