# Comparing `tmp/CamsMazes-1.0.8.tar.gz` & `tmp/CamsMazes-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CamsMazes-1.0.8.tar", last modified: Thu Apr  4 16:54:16 2024, max compression
+gzip compressed data, was "CamsMazes-1.0.9.tar", last modified: Thu Apr  4 19:14:06 2024, max compression
```

## Comparing `CamsMazes-1.0.8.tar` & `CamsMazes-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.693913 CamsMazes-1.0.8/
--rw-rw-rw-   0        0        0     3413 2024-04-04 16:54:16.690914 CamsMazes-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2024-04-03 19:17:18.000000 CamsMazes-1.0.8/README.md
--rw-rw-rw-   0        0        0      427 2024-04-04 16:52:53.000000 CamsMazes-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 16:54:16.694913 CamsMazes-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.566058 CamsMazes-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.603706 CamsMazes-1.0.8/src/CamsMazes/
--rw-rw-rw-   0        0        0        0 2024-04-03 19:04:55.000000 CamsMazes-1.0.8/src/CamsMazes/__init__.py
--rw-rw-rw-   0        0        0    12789 2024-04-04 16:51:23.000000 CamsMazes-1.0.8/src/CamsMazes/maze.py
--rw-rw-rw-   0        0        0     3521 2024-04-04 16:52:44.000000 CamsMazes-1.0.8/src/CamsMazes/maze_visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:54:16.687915 CamsMazes-1.0.8/src/CamsMazes.egg-info/
--rw-rw-rw-   0        0        0     3413 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 16:54:16.000000 CamsMazes-1.0.8/src/CamsMazes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 19:14:06.878187 CamsMazes-1.0.9/
+-rw-rw-rw-   0        0        0     3413 2024-04-04 19:14:06.877180 CamsMazes-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2024-04-03 19:17:18.000000 CamsMazes-1.0.9/README.md
+-rw-rw-rw-   0        0        0      427 2024-04-04 19:13:28.000000 CamsMazes-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:14:06.878187 CamsMazes-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 19:14:06.831096 CamsMazes-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:14:06.850387 CamsMazes-1.0.9/src/CamsMazes/
+-rw-rw-rw-   0        0        0        0 2024-04-03 19:04:55.000000 CamsMazes-1.0.9/src/CamsMazes/__init__.py
+-rw-rw-rw-   0        0        0    12917 2024-04-04 19:03:49.000000 CamsMazes-1.0.9/src/CamsMazes/maze.py
+-rw-rw-rw-   0        0        0     3521 2024-04-04 16:52:44.000000 CamsMazes-1.0.9/src/CamsMazes/maze_visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:14:06.876180 CamsMazes-1.0.9/src/CamsMazes.egg-info/
+-rw-rw-rw-   0        0        0     3413 2024-04-04 19:14:06.000000 CamsMazes-1.0.9/src/CamsMazes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-04 19:14:06.000000 CamsMazes-1.0.9/src/CamsMazes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:14:06.000000 CamsMazes-1.0.9/src/CamsMazes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-04 19:14:06.000000 CamsMazes-1.0.9/src/CamsMazes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 19:14:06.000000 CamsMazes-1.0.9/src/CamsMazes.egg-info/top_level.txt
```

### Comparing `CamsMazes-1.0.8/PKG-INFO` & `CamsMazes-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

### Comparing `CamsMazes-1.0.8/README.md` & `CamsMazes-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.8/src/CamsMazes/maze.py` & `CamsMazes-1.0.9/src/CamsMazes/maze.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,16 +202,17 @@
 
         self.solution = solution_path # Add solution to Maze
         self.solved = True
         self.grid_solution = grid
         return grid
 
     # Returns JSON representation of Maze
-    def to_json(self):
-        img_str = self.to_image(save = False)[1]
+    def to_json(self, image_cell_size = None):
+        img_arr = self.to_image(save = False, cell_size=image_cell_size) if image_cell_size else self.to_image(save=False)
+        img_str = img_arr[1]
         maze = {
             "numCols": self.num_cols,
             "numRows": self.num_rows,
             "startCol": self.start_col,
             "startRow": self.start_row,
             "endCol": self.end_col,
             "endRow": self.end_row,
```

### Comparing `CamsMazes-1.0.8/src/CamsMazes/maze_visualizer.py` & `CamsMazes-1.0.9/src/CamsMazes/maze_visualizer.py`

 * *Files identical despite different names*

### Comparing `CamsMazes-1.0.8/src/CamsMazes.egg-info/PKG-INFO` & `CamsMazes-1.0.9/src/CamsMazes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamsMazes
-Version: 1.0.8
+Version: 1.0.9
 Summary: Maze Generator and Solver using DFS
 Author-email: Cameron Rolfe <cameronrolfedev@example.com>
 Project-URL: Homepage, https://github.com/CameronRolfe/MazeGenerator
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 Requires-Dist: Pillow
```

