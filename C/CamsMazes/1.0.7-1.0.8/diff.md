# Comparing `tmp/CamsMazes-1.0.7.tar.gz` & `tmp/CamsMazes-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CamsMazes-1.0.7.tar", last modified: Wed Apr  3 19:18:44 2024, max compression
+gzip compressed data, was "CamsMazes-1.0.8.tar", last modified: Thu Apr  4 16:54:16 2024, max compression
```

## Comparing `CamsMazes-1.0.7.tar` & `CamsMazes-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.717388 CamsMazes-1.0.7/
--rw-rw-rw-   0        0        0     3413 2024-04-03 19:18:44.716389 CamsMazes-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2024-04-03 19:17:18.000000 CamsMazes-1.0.7/README.md
--rw-rw-rw-   0        0        0      427 2024-04-03 19:18:31.000000 CamsMazes-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 19:18:44.717388 CamsMazes-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.690389 CamsMazes-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.694392 CamsMazes-1.0.7/src/CamsMazes/
--rw-rw-rw-   0        0        0        0 2024-04-03 19:04:55.000000 CamsMazes-1.0.7/src/CamsMazes/__init__.py
--rw-rw-rw-   0        0        0    12405 2024-04-03 19:04:58.000000 CamsMazes-1.0.7/src/CamsMazes/maze.py
--rw-rw-rw-   0        0        0     3546 2024-04-03 19:03:20.000000 CamsMazes-1.0.7/src/CamsMazes/maze_visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:18:44.715417 CamsMazes-1.0.7/src/CamsMazes.egg-info/
--rw-rw-rw-   0        0        0     3413 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 19:18:44.000000 CamsMazes-1.0.7/src/CamsMazes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.693913 CamsMazes-1.0.8/
+-rw-rw-rw-   0        0        0     3413 2024-04-04 16:54:16.690914 CamsMazes-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2024-04-03 19:17:18.000000 CamsMazes-1.0.8/README.md
+-rw-rw-rw-   0        0        0      427 2024-04-04 16:52:53.000000 CamsMazes-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 16:54:16.694913 CamsMazes-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.566058 CamsMazes-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.603706 CamsMazes-1.0.8/src/CamsMazes/
+-rw-rw-rw-   0        0        0        0 2024-04-03 19:04:55.000000 CamsMazes-1.0.8/src/CamsMazes/__init__.py
+-rw-rw-rw-   0        0        0    12789 2024-04-04 16:51:23.000000 CamsMazes-1.0.8/src/CamsMazes/maze.py
+-rw-rw-rw-   0        0        0     3521 2024-04-04 16:52:44.000000 CamsMazes-1.0.8/src/CamsMazes/maze_visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.687915 CamsMazes-1.0.8/src/CamsMazes.egg-info/
+-rw-rw-rw-   0        0        0     3413 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/top_level.txt
```

### Comparing `CamsMazes-1.0.7/PKG-INFO` & `CamsMazes-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.7
+Version: 1.0.8
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

### Comparing `CamsMazes-1.0.7/README.md` & `CamsMazes-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.7/src/CamsMazes/maze.py` & `CamsMazes-1.0.8/src/CamsMazes/maze.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import random
 from random import randint
 import json
 import copy
 from PIL import Image, ImageDraw
+from io import BytesIO
+import base64
 
 class Maze:
     class Cell:
         def __init__(self, row, col):
             self.col = col
             self.row = row
             self.walls = {"top": 1, "right": 1, "bottom": 1, "left": 1}
@@ -201,14 +203,15 @@
         self.solution = solution_path # Add solution to Maze
         self.solved = True
         self.grid_solution = grid
         return grid
 
     # Returns JSON representation of Maze
     def to_json(self):
+        img_str = self.to_image(save = False)[1]
         maze = {
             "numCols": self.num_cols,
             "numRows": self.num_rows,
             "startCol": self.start_col,
             "startRow": self.start_row,
             "endCol": self.end_col,
             "endRow": self.end_row,
@@ -218,15 +221,16 @@
                 "cols": self.grid_cols,
                 "startCell": self.start_grid_cell,
                 "endCell": self.end_grid_cell, 
                 "maze": self.grid,
                 "mazeSolution": self.grid_solution,
                 "generationPath": self.generation_path,
                 "solutionPath": self.solution
-            }
+            },
+            "img_base64": img_str
         }
         return json.dumps(maze)
     
     # Prints maze
     def print(self, show_solution = False):
         print(self._get_maze_text(show_solution))
 
@@ -264,27 +268,31 @@
             if (not curr_row == self.grid_rows-1): maze_str+="\n"
             curr_row+=1
         return maze_str
 
     def __str__(self):
         return self._get_maze_text(show_solution=False)
 
-    # Creates png image of maze
-    def to_image(self, fileName = "maze", cell_size=15, showSolution = False):
+    # Creates image of maze
+    def to_image(self, file_name = "maze", file_ext = "png", cell_size=15, save=True, show_solution = False):
         image = Image.new("RGB", self._get_image_size(cell_size), "black")
         draw = ImageDraw.Draw(image)
         img_colour_map = {0: "white", 1: "black", 2: "green", 3: "yellow", 4: "red"}
-        grid = self.grid_solution if showSolution else self.grid
+        grid = self.grid_solution if show_solution else self.grid
+        buff = BytesIO()
         for row in range(self.grid_rows):
             for col in range(self.grid_cols):
                 cell_type = grid[row][col]
                 cell_colour = img_colour_map[cell_type]
                 draw.rectangle(self._convert_to_image_coords(cell_size, row, col), fill=cell_colour)
-        image.save(f"{fileName}.png")
-        return image
+        if (save): image.save(f"{file_name}.{file_ext}")
+        file_ext = "jpeg" if file_ext == "jpg" else file_ext 
+        image.save(buff, format=file_ext)
+        img_str = base64.b64encode(buff.getvalue()).decode("utf-8")
+        return [image, img_str]
     
     # Creates gif of maze generation
     def to_gif(self, file_name="maze", cell_size=10):
         images = []
         image = Image.new("P", self._get_image_size(cell_size), "black") 
         draw = ImageDraw.Draw(image)
         images.append(image)
```

### Comparing `CamsMazes-1.0.7/src/CamsMazes/maze_visualizer.py` & `CamsMazes-1.0.8/src/CamsMazes/maze_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from tkinter import *
 import time
-#from .maze import Maze
 from maze import Maze
 
 class MazeVisualizer:
     class CellVisualizer:
         def __init__(self, canvas, cell_size):
             self.canvas = canvas
             self.cell_size = cell_size
```

### Comparing `CamsMazes-1.0.7/src/CamsMazes.egg-info/PKG-INFO` & `CamsMazes-1.0.8/src/CamsMazes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.7
+Version: 1.0.8
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

