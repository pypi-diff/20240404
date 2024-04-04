# Comparing `tmp/layermesh-0.4.0.tar.gz` & `tmp/layermesh-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layermesh-0.4.0.tar", last modified: Thu Feb 22 00:55:37 2024, max compression
+gzip compressed data, was "layermesh-0.4.1.tar", last modified: Thu Apr  4 04:21:53 2024, max compression
```

## Comparing `layermesh-0.4.0.tar` & `layermesh-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:55:37.268789 layermesh-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-22 00:55:26.000000 layermesh-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-02-22 00:55:37.268789 layermesh-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-22 00:55:26.000000 layermesh-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:55:37.268789 layermesh-0.4.0/layermesh/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-22 00:55:26.000000 layermesh-0.4.0/layermesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-02-22 00:55:26.000000 layermesh-0.4.0/layermesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    76938 2024-02-22 00:55:26.000000 layermesh-0.4.0/layermesh/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-02-22 00:55:26.000000 layermesh-0.4.0/layermesh/quadtree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:55:37.268789 layermesh-0.4.0/layermesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-02-22 00:55:37.000000 layermesh-0.4.0/layermesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-22 00:55:37.000000 layermesh-0.4.0/layermesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 00:55:37.000000 layermesh-0.4.0/layermesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-22 00:55:37.000000 layermesh-0.4.0/layermesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-22 00:55:37.000000 layermesh-0.4.0/layermesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-22 00:55:26.000000 layermesh-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 00:55:37.268789 layermesh-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-22 00:55:26.000000 layermesh-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 00:55:37.268789 layermesh-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-02-22 00:55:26.000000 layermesh-0.4.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    21797 2024-02-22 00:55:26.000000 layermesh-0.4.0/tests/test_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:21:53.111581 layermesh-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-04 04:21:44.000000 layermesh-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-04 04:21:53.111581 layermesh-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-04 04:21:44.000000 layermesh-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:21:53.111581 layermesh-0.4.1/layermesh/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 04:21:44.000000 layermesh-0.4.1/layermesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-04 04:21:44.000000 layermesh-0.4.1/layermesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72946 2024-04-04 04:21:44.000000 layermesh-0.4.1/layermesh/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-04 04:21:44.000000 layermesh-0.4.1/layermesh/quadtree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:21:53.111581 layermesh-0.4.1/layermesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-04 04:21:53.000000 layermesh-0.4.1/layermesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-04 04:21:53.000000 layermesh-0.4.1/layermesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:21:53.000000 layermesh-0.4.1/layermesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 04:21:53.000000 layermesh-0.4.1/layermesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 04:21:53.000000 layermesh-0.4.1/layermesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 04:21:44.000000 layermesh-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:21:53.111581 layermesh-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 04:21:44.000000 layermesh-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:21:53.111581 layermesh-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-04 04:21:44.000000 layermesh-0.4.1/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22904 2024-04-04 04:21:44.000000 layermesh-0.4.1/tests/test_mesh.py
```

### Comparing `layermesh-0.4.0/LICENSE` & `layermesh-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `layermesh-0.4.0/PKG-INFO` & `layermesh-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layermesh
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library for layered computational meshes
 Author-email: Adrian Croucher <a.croucher@auckland.ac.nz>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `layermesh-0.4.0/README.md` & `layermesh-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `layermesh-0.4.0/layermesh/geometry.py` & `layermesh-0.4.1/layermesh/geometry.py`

 * *Files 15% similar despite different names*

```diff
@@ -193,14 +193,66 @@
                 dist = np.linalg.norm(bdy - a)
                 if dist < dmin:
                     dmin = dist
                     v = bdy + ref
         except np.linalg.LinAlgError: continue
     return v
 
+def line_intersects_rectangle(rect, line):
+    # returns True if line intersects axis-aligned rectangle defined
+    # by two corners. Simplified Cohen-Sutherland algorithm, based on
+    # the pylineclip library.
+
+    INSIDE, LEFT, RIGHT, LOWER, UPPER = 0, 1, 2, 4, 8
+
+    xmin, ymin = rect[0]
+    xmax, ymax = rect[1]
+    x1, y1 = line[0]
+    x2, y2 = line[1]
+
+    def clip(xa, ya):
+        p = INSIDE
+        if xa < xmin: p |= LEFT
+        elif xa > xmax: p |= RIGHT
+        if ya < ymin: p |= LOWER
+        elif ya > ymax: p |= UPPER
+        return p
+
+    k1 = clip(x1, y1)
+    k2 = clip(x2, y2)
+
+    while (k1 | k2) != 0:
+
+        if (k1 & k2) != 0: return False
+
+        opt = k1 or k2
+        if opt & UPPER:
+            x = x1 + (x2 - x1) * (ymax - y1) / (y2 - y1)
+            y = ymax
+        elif opt & LOWER:
+            x = x1 + (x2 - x1) * (ymin - y1) / (y2 - y1)
+            y = ymin
+        elif opt & RIGHT:
+            y = y1 + (y2 - y1) * (xmax - x1) / (x2 - x1)
+            x = xmax
+        elif opt & LEFT:
+            y = y1 + (y2 - y1) * (xmin - x1) / (x2 - x1)
+            x = xmin
+        else:
+            raise RuntimeError('Undefined clipping state')
+
+        if opt == k1:
+            x1, y1 = x, y
+            k1 = clip(x1, y1)
+        elif opt == k2:
+            x2, y2 = x, y
+            k2 = clip(x2, y2)
+
+    return True
+
 def line_projection(a, line, return_xi = False):
     """Finds projection of point *a* onto a *line* (defined by two points,
     each a tuple, list or array of length 2).  Optionally returns the
     non-dimensional distance xi between the line start and end.
     """
     line = [np.array(p) for p in line]
     d = line[1] - line[0]
```

### Comparing `layermesh-0.4.0/layermesh/mesh.py` & `layermesh-0.4.1/layermesh/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1205,141 +1205,61 @@
                 isort = np.argsort(np.array([r.index for r in result]))
                 result = [result[i] for i in isort]
             return [r.index for r in result] if indices else result
         else:
             return result.index if indices else result
 
     def column_track(self, line):
-        """Returns a list of tuples of (column, entry_point, exit_point)
+        """Returns a list of tuples of (column,entrypoint,exitpoint)
         representing the horizontal track traversed by the specified
-        line through the grid.  Line is a tuple of two 2D arrays.
-
-        The resulting list is ordered by distance from the start of the
-        line. Adapted from the PyTOUGH mulgrid column_track()
-        method."""
-
-        def furthest_intersection(poly, line):
-            """Returns furthest intersection point between line and poly."""
-            from layermesh.geometry import line_polygon_intersections
-            pts, inds = line_polygon_intersections(poly, line,
-                                                   bound_line = (True, False),
-                                                   indices = True)
-            if pts:
-                d = np.array([np.linalg.norm(intpt - line[0]) for intpt in pts])
-                i = np.argmax(d)
-                return pts[i], inds[i]
-            else: return None, None
-
-        def find_track_start(line):
-            """Finds starting point for track- an arbitrary point on the line that
-            is inside the grid.  If the start point of the line is
-            inside the grid, that is used; otherwise, a recursive
-            bisection technique is used to find a point."""
-
-            col, start_type = None, None
-            for endpt, name in zip(line, ['start', 'end']):
-                pos, col, start_type = endpt, self.find(endpt), name
-                if col: break
-            if not col: # line ends are both outside the grid:
-                start_type = 'mid'
-                max_levels = 7
-
-                def find_start(line, level = 0):
-                    midpt = 0.5 * (line[0] + line[1])
-                    col = self.find(midpt)
-                    if col: return midpt, col
-                    else:
-                        if level <= max_levels:
-                            line0, line1 = [line[0], midpt], [midpt, line[1]]
-                            pos, col = find_start(line0, level + 1)
-                            if col: return pos, col
-                            else:
-                                pos, col = find_start(line1, level + 1)
-                                if col: return pos, col
-                                else: return None, None
-                        else: return None, None
-
-                pos, col = find_start(line)
-            return pos, col, start_type
-
-        def next_corner_column(col, pos, more, cols):
-            """If the line has hit a node, determine a new column containing that
-            node, not already visited."""
-
-            node_tol = 1.e-12
-            nextcol = None
-            nearnodes = [n for n in col.node if np.linalg.norm(n.pos - pos) < node_tol]
-            if nearnodes: # hit a node
-                nearnode = nearnodes[0]
-                nearcols = nearnode.column - cols
-                if nearcols: nextcol = nearcols.pop()
-                else: more = False
-            return nextcol, more
-
-        def next_neighbour_column(col, more, cols):
-            """Determine a new neighbour column not already visited."""
-
-            nbrs = col.neighbour - cols
-            if nbrs: return nbrs.pop(), more
-            else: return None, False
-
-        def find_track_segment(linesegment, pos, col):
-            """Finds track segment starting from the specified position and
-            column."""
-            track = []
-            cols, more, inpos = set(), True, pos
-            colnbr, nextcol = col.side_neighbour, None
-            lined = np.linalg.norm(linesegment[1] - linesegment[0])
-            while more:
-                cols.add(col)
-                outpos, ind = furthest_intersection(col.polygon, linesegment)
-                if outpos is not None:
-                    d = np.linalg.norm(outpos - linesegment[0])
-                    if d >= lined: # gone past end of line
-                        outpos = linesegment[1]
-                        more = False
-                    if np.linalg.norm(outpos - inpos) > 0.:
-                        track.append(tuple([col, inpos, outpos]))
-                    if more: # find next column
-                        inpos = outpos
-                        nextcol = colnbr[ind]
-                        if nextcol:
-                            if nextcol in cols:
-                                nextcol, more = next_corner_column(col, outpos, more, cols)
-                                if nextcol is None:
-                                    nextcol, more = next_neighbour_column(col, more, cols)
-                                    nbr_base_col = col
-                        else: nextcol, more = next_corner_column(col, outpos, more, cols)
+        line through the grid.  Line is a tuple of two 2D arrays.  The
+        resulting list is ordered by distance from the start of the
+        line.
+        """
+
+        from layermesh.geometry import line_intersects_rectangle, \
+            line_polygon_intersections
+
+        line = np.array(line)
+        tol = 1e-3
+        def track_dist(p): return np.linalg.norm(p - line[0])
+        dl = track_dist(line[1])
+        tol_dl = tol * dl
+
+        track, dist = [], []
+        start_col, end_col = None, None
+        for col in self.column:
+            bbox = col.bounding_box
+            if line_intersects_rectangle(bbox, line):
+                if start_col is None:
+                    if col.find(line[0]):
+                        start_col = col
+                if end_col is None:
+                    if col.find(line[1]):
+                        end_col = col
+                if col == start_col == end_col:
+                    track.append((col, line[0], line[1]))
+                    dist.append(0)
+                    break
                 else:
-                    nextcol, more = next_neighbour_column(nbr_base_col, more, cols)
-                col = nextcol
-                if col: colnbr = col.side_neighbour
-                else: more = False
-
-            return track
-
-        def reverse_track(track):
-            return [tuple([tk[0], tk[2], tk[1]]) for tk in track][::-1]
-
-        line = [np.array(p) for p in line]
-        pos, col, start_type = find_track_start(line)
-        if pos is not None and col:
-            if start_type == 'start':
-                track = find_track_segment(line, pos, col)
-            elif start_type == 'end':
-                track = find_track_segment(line[::-1], pos, col)
-                track = reverse_track(track)
-            else:
-                track1 = find_track_segment([pos, line[0]], pos, col)
-                track2 = find_track_segment([pos, line[1]], pos, col)
-                # remove arbitrary starting point from middle of track, and join:
-                midtk = tuple([track1[0][0], track1[0][2], track2[0][2]])
-                track = reverse_track(track1)[:-1] + [midtk] + track2[1:]
-            return track
-        else: return []
+                    poly = col.polygon
+                    pts = line_polygon_intersections(poly, line)
+                    if len(pts) > 0:
+                        if col == start_col:
+                            pts = [line[0], pts[-1]]
+                        elif col == end_col:
+                            pts = [pts[0], line[-1]]
+                        din, dout = track_dist(pts[0]), track_dist(pts[-1])
+                        if abs(dout - din) > tol_dl:
+                            track.append((col, pts[0], pts[-1]))
+                            dist.append(din)
+
+        sortindex = np.argsort(np.array(dist))
+        track = [track[i] for i in sortindex]
+        return track
 
     def layer_plot(self, lay = -1, **kwargs):
         """Creates a 2-D Matplotlib plot of the mesh at a specified layer. The
         *lay* parameter can be either a layer object or a layer index.
 
         Other optional parameters:
```

### Comparing `layermesh-0.4.0/layermesh/quadtree.py` & `layermesh-0.4.1/layermesh/quadtree.py`

 * *Files identical despite different names*

### Comparing `layermesh-0.4.0/layermesh.egg-info/PKG-INFO` & `layermesh-0.4.1/layermesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layermesh
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library for layered computational meshes
 Author-email: Adrian Croucher <a.croucher@auckland.ac.nz>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `layermesh-0.4.0/pyproject.toml` & `layermesh-0.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "layermesh"
-version = "0.4.0"
+version = "0.4.1"
 description = "Library for layered computational meshes"
 readme = "README.md"
 authors = [
   {name = "Adrian Croucher", email = "a.croucher@auckland.ac.nz"}
 ]
 license = {file = "LICENSE"}
 requires-python = ">=2.7"
```

### Comparing `layermesh-0.4.0/tests/test_geometry.py` & `layermesh-0.4.1/tests/test_geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -247,11 +247,31 @@
         p = np.array([0, 0])
         r = np.dot(A, p) + b
         self.assertTrue(np.allclose(r, np.array([0, 2])))
         p = np.array([2, 1])
         r = np.dot(A, p) + b
         self.assertTrue(np.allclose(r, np.array([1, 0])))
 
+    def test_line_intersects_rectangle(self):
+        """line_intersects_rectangle()"""
+        r = [np.array([1., 1.]), np.array([5., 3.])]
+        line = [np.array([0., 0.]), np.array([1., 1.])]
+        self.assertTrue(geometry.line_intersects_rectangle(r, line))
+        line = r
+        self.assertTrue(geometry.line_intersects_rectangle(r, line))
+        line = r[::-1]
+        self.assertTrue(geometry.line_intersects_rectangle(r, line))
+        line = [np.array([1., 1.]), np.array([5., 1.])]
+        self.assertTrue(geometry.line_intersects_rectangle(r, line))
+        line = [np.array([3., 1.]), np.array([4., 3.])]
+        self.assertTrue(geometry.line_intersects_rectangle(r, line))
+        line = [np.array([3., 0.]), np.array([4., 6.])]
+        self.assertTrue(geometry.line_intersects_rectangle(r, line))
+        line = [np.array([2., 2.]), np.array([4., 2.5])]
+        self.assertTrue(geometry.line_intersects_rectangle(r, line))
+        line = [np.array([6., 6.]), np.array([8., 0.])]
+        self.assertFalse(geometry.line_intersects_rectangle(r, line))
+
 if __name__ == '__main__':
 
     suite = unittest.TestLoader().loadTestsFromTestCase(geometryTestCase)
     unittest.TextTestRunner(verbosity = 1).run(suite)
```

### Comparing `layermesh-0.4.0/tests/test_mesh.py` & `layermesh-0.4.1/tests/test_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,23 +412,54 @@
         t = m.column_track(([5, 0], [5, 80]))
         self.assertEqual(track_indices(t), [0, 3, 6, 9])
         self.assertTrue(np.allclose(t[-1][1], np.array([5, 60])))
         self.assertTrue(np.allclose(t[-1][2], np.array([5, 80])))
 
         t = m.column_track(([0, 0], [30, 80]))
         self.assertEqual(track_indices(t), [0, 3, 4, 7, 8, 11])
-        self.assertTrue(np.allclose(t[0][1], np.array([0, 00])))
+        self.assertTrue(np.allclose(t[0][1], np.array([0, 0])))
         self.assertTrue(np.allclose(t[-1][2], np.array([30, 80])))
 
         t = m.column_track(([29, 1], [3, 71.5]))
         self.assertEqual(track_indices(t), [2, 5, 4, 7, 6, 9])
 
         t = m.column_track(([-2, 3.5], [40, 15]))
         self.assertEqual(track_indices(t), [0, 1, 2])
 
+        t = m.column_track(([12, 25], [18, 35]))
+        self.assertEqual(track_indices(t), [4])
+
+        t = m.column_track(([10, 20], [20, 40]))
+        self.assertEqual(track_indices(t), [4])
+
+        t = m.column_track(([35, -10], [35, 0]))
+        self.assertEqual(t, [])
+
+        # track through grid with a corner removed:
+        m = mesh.mesh(rectangular = ([100]*2, [100]*2, [10]))
+        m.translate([1e7, 1e7, 0])
+        m.delete_column(m.column[0])
+        m.rotate(30)
+        m.setup(indices = True)
+        line = [m.column[0].centre, m.column[1].centre]
+        t = m.column_track(line)
+        self.assertEqual(track_indices(t), [0, 1])
+
+        # M-grid:
+        m = mesh.mesh(rectangular= ([100]*5, [100]*3, [10]))
+        del_cols = [m.column[i] for i in [1,3,6,8]]
+        for col in del_cols: m.delete_column(col)
+        m.setup(indices = True)
+        line = [(0, 50), (500, 50)]
+        t = m.column_track(line)
+        self.assertEqual(track_indices(t), [0, 1, 2])
+        line = line[::-1]
+        t = m.column_track(line)
+        self.assertEqual(track_indices(t), [2, 1, 0])
+
     def test_io(self):
 
         import os
         dx = [10.]*3; dy = [12.] * 3
         dz = [1., 2., 3.]
         s = [0, 0, -1.5, -1.8, -2.1, -2.8, -3, -1, 0]
         m1 = mesh.mesh(rectangular = (dx, dy, dz), surface = s)
```

