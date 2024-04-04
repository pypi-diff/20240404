# Comparing `tmp/PyTOUGH-1.6.1.tar.gz` & `tmp/PyTOUGH-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTOUGH-1.6.1.tar", last modified: Sun Feb 25 22:35:23 2024, max compression
+gzip compressed data, was "PyTOUGH-1.6.2.tar", last modified: Thu Apr  4 04:09:22 2024, max compression
```

## Comparing `PyTOUGH-1.6.1.tar` & `PyTOUGH-1.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 22:35:23.464090 PyTOUGH-1.6.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)    19449 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/IAPWS97.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-02-25 22:35:23.464090 PyTOUGH-1.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 22:35:23.464090 PyTOUGH-1.6.1/PyTOUGH.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-02-25 22:35:23.000000 PyTOUGH-1.6.1/PyTOUGH.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-25 22:35:23.000000 PyTOUGH-1.6.1/PyTOUGH.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 22:35:23.000000 PyTOUGH-1.6.1/PyTOUGH.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 22:35:23.000000 PyTOUGH-1.6.1/PyTOUGH.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 22:35:23.000000 PyTOUGH-1.6.1/PyTOUGH.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/fixed_format_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13903 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   206242 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/mulgrids.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 22:35:23.464090 PyTOUGH-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   133291 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/t2data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    60732 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/t2grids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13547 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/t2incons.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    86115 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/t2listing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/t2thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 22:35:23.464090 PyTOUGH-1.6.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2433 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_IAPWS97.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20838 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_mulgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    93713 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_t2data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10546 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_t2grid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8999 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_t2incon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32245 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_t2listing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-02-25 22:35:12.000000 PyTOUGH-1.6.1/tests/test_t2thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:09:22.515880 PyTOUGH-1.6.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19449 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/IAPWS97.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-04 04:09:22.515880 PyTOUGH-1.6.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:09:22.511880 PyTOUGH-1.6.2/PyTOUGH.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-04 04:09:22.000000 PyTOUGH-1.6.2/PyTOUGH.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-04 04:09:22.000000 PyTOUGH-1.6.2/PyTOUGH.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:09:22.000000 PyTOUGH-1.6.2/PyTOUGH.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 04:09:22.000000 PyTOUGH-1.6.2/PyTOUGH.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 04:09:22.000000 PyTOUGH-1.6.2/PyTOUGH.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/fixed_format_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15223 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   202596 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/mulgrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:09:22.515880 PyTOUGH-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   133291 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/t2data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60732 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/t2grids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13696 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/t2incons.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86115 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/t2listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/t2thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:09:22.511880 PyTOUGH-1.6.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2433 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_IAPWS97.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24448 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_mulgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93713 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_t2data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10546 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_t2grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8999 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_t2incon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32245 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_t2listing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-04 04:09:18.000000 PyTOUGH-1.6.2/tests/test_t2thermo.py
```

### Comparing `PyTOUGH-1.6.1/IAPWS97.py` & `PyTOUGH-1.6.2/IAPWS97.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/LICENSE` & `PyTOUGH-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/PKG-INFO` & `PyTOUGH-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTOUGH
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python scripting library for TOUGH2 simulation
 Author-email: Adrian Croucher <a.croucher@auckland.ac.nz>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -211,20 +211,12 @@
 
 # More information:
 
 For more detailed information on PyTOUGH, consult the [user guide](https://pytough.readthedocs.io) (html, or you can download PDF or Epub versions) and the PyTOUGH [wiki](https://github.com/acroucher/PyTOUGH/wiki/), which has links to published articles on PyTOUGH.
 
 # What's new in PyTOUGH?
 
-The latest stable version is 1.6.1, which has:
+The latest stable version is 1.6.2, which has:
 
-* updated user guide theming using [Furo](https://github.com/pradyunsg/furo) Sphinx theme
+* a new `mulgrid` naming convention 3, with 3 characters for columns and 2 characters for layers
 
-* other user guide enhancements including a new "command reference" page
-
-as well as the changes introduced in version 1.6.0:
-
-* easy installation via `pip`
-
-* online user guide at [Read the Docs](https://pytough.readthedocs.io)
-
-* updated Python packaging using a `pyproject.toml` file
+* the `mulgrid` `column_track()` method has been re-written with a different algorithm, enabling it (and the `slice_plot()` method) to handle non-contiguous slices, e.g. if the slice passes out of the mesh and back in
```

### Comparing `PyTOUGH-1.6.1/PyTOUGH.egg-info/PKG-INFO` & `PyTOUGH-1.6.2/PyTOUGH.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTOUGH
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python scripting library for TOUGH2 simulation
 Author-email: Adrian Croucher <a.croucher@auckland.ac.nz>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -211,20 +211,12 @@
 
 # More information:
 
 For more detailed information on PyTOUGH, consult the [user guide](https://pytough.readthedocs.io) (html, or you can download PDF or Epub versions) and the PyTOUGH [wiki](https://github.com/acroucher/PyTOUGH/wiki/), which has links to published articles on PyTOUGH.
 
 # What's new in PyTOUGH?
 
-The latest stable version is 1.6.1, which has:
+The latest stable version is 1.6.2, which has:
 
-* updated user guide theming using [Furo](https://github.com/pradyunsg/furo) Sphinx theme
+* a new `mulgrid` naming convention 3, with 3 characters for columns and 2 characters for layers
 
-* other user guide enhancements including a new "command reference" page
-
-as well as the changes introduced in version 1.6.0:
-
-* easy installation via `pip`
-
-* online user guide at [Read the Docs](https://pytough.readthedocs.io)
-
-* updated Python packaging using a `pyproject.toml` file
+* the `mulgrid` `column_track()` method has been re-written with a different algorithm, enabling it (and the `slice_plot()` method) to handle non-contiguous slices, e.g. if the slice passes out of the mesh and back in
```

### Comparing `PyTOUGH-1.6.1/README.md` & `PyTOUGH-1.6.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,20 +28,12 @@
 
 # More information:
 
 For more detailed information on PyTOUGH, consult the [user guide](https://pytough.readthedocs.io) (html, or you can download PDF or Epub versions) and the PyTOUGH [wiki](https://github.com/acroucher/PyTOUGH/wiki/), which has links to published articles on PyTOUGH.
 
 # What's new in PyTOUGH?
 
-The latest stable version is 1.6.1, which has:
+The latest stable version is 1.6.2, which has:
 
-* updated user guide theming using [Furo](https://github.com/pradyunsg/furo) Sphinx theme
+* a new `mulgrid` naming convention 3, with 3 characters for columns and 2 characters for layers
 
-* other user guide enhancements including a new "command reference" page
-
-as well as the changes introduced in version 1.6.0:
-
-* easy installation via `pip`
-
-* online user guide at [Read the Docs](https://pytough.readthedocs.io)
-
-* updated Python packaging using a `pyproject.toml` file
+* the `mulgrid` `column_track()` method has been re-written with a different algorithm, enabling it (and the `slice_plot()` method) to handle non-contiguous slices, e.g. if the slice passes out of the mesh and back in
```

### Comparing `PyTOUGH-1.6.1/fixed_format_file.py` & `PyTOUGH-1.6.2/fixed_format_file.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/geometry.py` & `PyTOUGH-1.6.2/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,26 +111,24 @@
             p2 = polygon[(j+1) % n]
             t = p1[0] * p2[1] - p2[0] * p1[1]
             area += t
             c += (p1 + p2) * t
         area *= 0.5
         return c / (6. * area) + shift
 
-def line_polygon_intersections(polygon, line, bound_line = (True,True),
-                               indices = False):
+def line_polygon_intersections(polygon, line, bound_line = (True,True)):
     """Returns a list of the intersection points at which a line crosses a
     polygon.  The list is sorted by distance from the start of the
     line.  The parameter bound_line controls whether to limit
-    intersections between the line's start and end points.  If indices
-    is True, also return polygon side indices of intersections.
+    intersections between the line's start and end points.
     """
     crossings = []
     ref = polygon[0]
     l1, l2 = line[0] - ref, line[1] - ref
-    tol = 1.e-12
+    tol = 1.e-9
     ind = {}
     def in_unit(x): return -tol <= x <= 1.0 + tol
     for i, p in enumerate(polygon):
         p1 = p - ref
         p2 = polygon[(i+1)%len(polygon)] - ref
         dp = p2 - p1
         A, b = np.column_stack((dp, l1 - l2)), l1 - p1
@@ -140,30 +138,84 @@
             if bound_line[0]: inline = inline and (-tol <= xi[1])
             if bound_line[1]: inline = inline and (xi[1] <= 1.0 + tol)
             if in_unit(xi[0]) and inline :
                 c = tuple(ref + p1 + xi[0] * dp)
                 ind[c] = i
         except LinAlgError: continue
     crossings = [np.array(c) for c, i in ind.items()]
-    # Sort by distance from start of line:
-    sortindex = np.argsort([norm(c - line[0]) for c in crossings])
-    if indices: return [crossings[i] for i in sortindex], \
-       [ind[tuple(crossings[i])] for i in sortindex]
-    else: return [crossings[i] for i in sortindex]
+    # Remove duplicates and sort by distance from start of line:
+    d = np.array([norm(c - line[0]) for c in crossings])
+    if len(d) > 0: d = d / max(d[-1], 1) # non-dimensionalise
+    d = d.round(decimals = 3)
+    d_unique, i_unique = np.unique(d, return_index = True)
+    sortindex = np.argsort(d_unique)
+    return [crossings[i_unique[i]] for i in sortindex]
 
 def polyline_polygon_intersections(polygon, polyline):
     """Returns a list of intersection points at which a polyline (list of
     2-D points) crosses a polygon."""
     N = len(polyline)
     intersections = [
         line_polygon_intersections(polygon, [pt, polyline[(i+1) % N]])
         for i, pt in enumerate(polyline)]
     from itertools import chain # flatten list of lists
     return list(chain.from_iterable(intersections))
 
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
 def simplify_polygon(polygon, tolerance = 1.e-6):
     """Simplifies a polygon by deleting colinear points.  The tolerance
     for detecting colinearity of points can optionally be
     specified.
     """
     s = []
     N = len(polygon)
```

### Comparing `PyTOUGH-1.6.1/mulgrids.py` & `PyTOUGH-1.6.2/mulgrids.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     treating names as (a3, i2)"""
     if name[2].isdigit() and name[4].isdigit() and name[3] == ' ':
         return '0'.join((name[0:3], name[4:5]))
     else: return name
 
 def unfix_blockname(name):
     """The inverse of fix_blockname()."""
-    return "%3s%2d" % (name[0:3], int(name[3:5]))
+    return "%3s%2d" % (name[0:3], int(name[3:5])) if name[3:5].isdigit() else name
 
 def fix_block_mapping(blockmap):
     """Fixes block names in specified block mapping."""
     keys_to_fix = {}
     for k, v in blockmap.items():
         fixedk = fix_blockname(k)
         if k != fixedk: keys_to_fix[k] = fixedk
@@ -562,14 +562,15 @@
                  block_order = None):
         self.filename = filename
         self.type = type  # geometry type- only GENER supported
         self._convention = convention  # naming convention:
         # 0: 3-char column + 2-digit layer
         # 1: 3-char layer + 2-digit column
         # 2: 2-char layer + 3-digit column
+        # 3: 3-char column + 2-char layer
         self._atmosphere_type = atmos_type  # atmosphere type:
         # 0: single atmosphere block
         # 1: one atmosphere block per column
         # else: no atmosphere blocks
         self.set_secondary_variables()
         self.atmosphere_volume = atmos_volume
         self.atmosphere_connection = atmos_connection
@@ -583,17 +584,17 @@
         self.empty()
         if self.filename: self.read(filename)
         if block_order is not None: self.block_order = block_order.lower()
 
     def set_secondary_variables(self):
         """Sets variables dependent on naming convention and atmosphere type"""
         if self.atmosphere_type == 0:
-            self.atmosphere_column_name = ['ATM', ' 0', '  0'][self.convention]
-        self.colname_length = [3, 2, 3][self.convention]
-        self.layername_length = [2, 3, 2][self.convention]
+            self.atmosphere_column_name = ['ATM', ' 0', '  0', 'ATM'][self.convention]
+        self.colname_length = [3, 2, 3, 3][self.convention]
+        self.layername_length = [2, 3, 2, 2][self.convention]
 
     def get_convention(self):
         """Get naming convention"""
         return self._convention
     def set_convention(self, convention):
         """Set naming convention"""
         self._convention = convention
@@ -728,15 +729,16 @@
         self.block_connection_name_list = []
         self.block_connection_name_index = {}
 
     def __repr__(self):
         conventionstr = [
             '3 characters for column, 2 digits for layer',
             '3 characters for layer, 2 digits for column',
-            '2 characters for layer, 3 digits for column'][self.convention]
+            '2 characters for layer, 3 digits for column',
+            '3 characters for column, 2 characters for layer'][self.convention]
         atmstr = [
             'single atmosphere block',
             'one atmosphere block over each column',
             'no atmosphere blocks'][self.atmosphere_type]
         return str(self.num_nodes) + ' nodes; ' + \
             str(self.num_columns) + ' columns; ' + \
             str(self.num_layers) + ' layers; ' + \
@@ -863,27 +865,29 @@
             [(con, i) for i, con in enumerate(self.block_connection_name_list)])
 
     def column_name(self, blockname):
         """Returns column name of block name."""
         if self.convention == 0: return blockname[0: 3]
         elif self.convention == 1: return blockname[3: 5]
         elif self.convention == 2: return blockname[2: 5]
+        elif self.convention == 3: return blockname[0: 3]
         else: return None
 
     def layer_name(self, blockname):
         """Returns layer name of block name."""
         if self.convention == 0: return blockname[3: 5]
         elif self.convention == 1: return blockname[0: 3]
         elif self.convention == 2: return blockname[0: 2]
+        elif self.convention == 3: return blockname[3: 5]
         else: return None
 
     def node_col_name_from_number(self, num, justfn = str.rjust,
                                   chars = ascii_lowercase, spaces = True):
         """Returns node or column name from number."""
-        if self.convention == 0:
+        if self.convention in [0, 3]:
             name = justfn(int_to_chars(num, chars = chars, spaces = spaces,
                                        length = self.colname_length), self.colname_length)
         else: name = str.rjust(str(num), self.colname_length)
         return name
 
     def column_name_from_number(self, num, justfn = str.rjust,
                                 chars = ascii_lowercase, spaces = True):
@@ -1437,15 +1441,15 @@
             return [dist, area]
         else: return [[0.0, 0.0], 0.0] # no connection
 
     def block_name(self, layername, colname, blockmap = {}):
         """Returns block name from layer and column names, depending on the
         naming convention.  An optional block mapping can be applied.
         """
-        if self.convention == 0: name = colname[0:3] + layername[0:2]
+        if self.convention in [0, 3]: name = colname[0:3] + layername[0:2]
         elif self.convention == 1: name = layername[0:3] + colname[0:2]
         else: name = layername[0:2] + colname[0:3]
         blkname = fix_blockname(name)
         if blkname in blockmap: blkname = blockmap[blkname]
         return blkname
 
     def write(self, filename = ''):
@@ -1598,15 +1602,15 @@
                    chars  =  ascii_lowercase, spaces = True):
         """Adds layers of specified thicknesses and top elevation."""
         justfn = [str.rjust, str.ljust][justify == 'l']
         chars = uniqstring(chars)
         num = 0
         self.clear_layers()
         z = top_elevation
-        surfacelayername = [' 0', 'atm', 'at'][self.convention]
+        surfacelayername = [' 0', 'atm', 'at', ' 0'][self.convention]
         self.add_layer(layer(surfacelayername, z, z))
         for thickness in thicknesses:
             z -= thickness
             centre = z + 0.5 * thickness
             name = surfacelayername
             while name == surfacelayername:
                 # make sure layer name is different from surface layer name
@@ -1649,15 +1653,15 @@
                 element_type = int(items[1])
                 if element_type in [2, 3]: # triangle or quadrilateral
                     name = items[0]
                     name = self.column_name_from_number(int(name), justfn, chars, spaces)
                     ntags = int(items[2])
                     colnodenumbers = [int(item) for item in items[3 + ntags:]]
                     colnodenames = [[self.node_name_from_number(nodeno, justfn, chars, spaces),
-                                     nodeno][convention > 0] for nodeno in colnodenumbers]
+                                     nodeno][convention in [1, 2]] for nodeno in colnodenumbers]
                     colnodes = [grid.node[v] for v in colnodenames]
                     grid.add_column(column(name, colnodes))
 
         def read_msh_4_1():
             line = ''
             while not '$Nodes' in line: line = gmsh.readline()
             items = gmsh.readline().strip().split(' ')
@@ -1685,15 +1689,15 @@
                 if element_type in [2, 3]: # triangle or quadrilateral
                     for ielt in range(num_block_elements):
                         items = gmsh.readline().strip().split(' ')
                         tag = items[0]
                         name = self.column_name_from_number(int(tag), justfn, chars, spaces)
                         colnodenumbers = [int(item) for item in items[1:]]
                         colnodenames = [[self.node_name_from_number(nodeno, justfn, chars, spaces),
-                                         nodeno][convention > 0] for nodeno in colnodenumbers]
+                                         nodeno][convention in [1, 2]] for nodeno in colnodenumbers]
                         colnodes = [grid.node[v] for v in colnodenames]
                         grid.add_column(column(name, colnodes))
                 else:
                     for ielt in range(num_block_elements): gmsh.readline()
 
         if filetype == '2.2': read_msh_2_2()
         elif filetype == '4.1': read_msh_4_1()
@@ -1995,125 +1999,50 @@
         """Returns a list of tuples of (column,entrypoint,exitpoint)
         representing the horizontal track traversed by the specified
         line through the grid.  Line is a tuple of two 2D arrays.  The
         resulting list is ordered by distance from the start of the
         line.
         """
 
-        def furthest_intersection(poly, line):
-            """Returns furthest intersection point between line and poly."""
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
-            """Finds starting point for track- an arbitrary point on the line that is inside
-            the grid.  If the start point of the line is inside the grid, that is used;
-            otherwise, a recursive bisection technique is used to find a point."""
-            col, start_type = None, None
-            for endpt, name in zip(line, ['start', 'end']):
-                pos, col, start_type = endpt, self.column_containing_point(endpt), name
-                if col: break
-            if not col: # line ends are both outside the grid:
-                start_type = 'mid'
-                max_levels = 7
-
-                def find_start(line, level = 0):
-                    midpt = 0.5 * (line[0] + line[1])
-                    col = self.column_containing_point(midpt)
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
-            """If the line has hit a node, determine a new column containing that node,
-            not already visited."""
-            node_tol = 1.e-12
-            nextcol = None
-            nearnodes = [n for n in col.node if np.linalg.norm(n.pos - pos) < node_tol]
-            if nearnodes: # hit a node
-                nearnode = nearnodes[0]
-                nearcols = nearnode.column - cols
-                if nearcols: nextcol = nearcols.pop()
-                else: more = False
-            return nextcol, more
+        tol = 1e-3
+        def track_dist(p): return norm(p - line[0])
+        dl = track_dist(line[1])
+        tol_dl = tol * dl
 
-        def next_neighbour_column(col, more, cols):
-            """Determine a new neighbour column not already visited."""
-            nbrs = col.neighbour - cols
-            if nbrs: return nbrs.pop(), more
-            else: return None, False
-
-        def find_track_segment(linesegment, pos, col):
-            """Finds track segment starting from the specified position and column."""
-            track = []
-            cols, more, inpos = set(), True, pos
-            colnbr, nextcol = col.neighbourlist, None
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
+        track, dist = [], []
+        start_col, end_col = None, None
+        for col in self.columnlist:
+            bbox = col.bounding_box
+            if line_intersects_rectangle(bbox, line):
+                if start_col is None:
+                    if col.contains_point(line[0]):
+                        start_col = col
+                if end_col is None:
+                    if col.contains_point(line[1]):
+                        end_col = col
+                if col == start_col == end_col:
+                    track.append((col, line[0], line[1]))
+                    dist.append(0)
+                    break
                 else:
-                    nextcol, more = next_neighbour_column(nbr_base_col, more, cols)
-                col = nextcol
-                if col: colnbr = col.neighbourlist
-                else: more = False
-
-            return track
-
-        def reverse_track(track): return [tuple([tk[0], tk[2], tk[1]]) for tk in track][::-1]
-
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
 
     def layer_plot_wells(self, plt, ax, layer, wells, well_names,
                          hide_wells_outside, wellcolour, welllinewidth, wellname_bottom):
         """Draws wells on a layer plot, given the plot and axes.  For
         documentation of the parameters, see layer_plot()."""
         if wells is True: wells = self.welllist
         elif wells is False or wells is None: wells = []
```

### Comparing `PyTOUGH-1.6.1/pyproject.toml` & `PyTOUGH-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyTOUGH"
-version = "1.6.1"
+version = "1.6.2"
 description = "Python scripting library for TOUGH2 simulation"
 readme = "README.md"
 authors = [
   {name = "Adrian Croucher", email = "a.croucher@auckland.ac.nz"}
 ]
 license = {file = "LICENSE"}
 requires-python = ">=2.7"
```

### Comparing `PyTOUGH-1.6.1/t2data.py` & `PyTOUGH-1.6.2/t2data.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/t2grids.py` & `PyTOUGH-1.6.2/t2grids.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/t2incons.py` & `PyTOUGH-1.6.2/t2incons.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,19 +53,20 @@
         if self.nseq is not None:
             result += ' (' + str(self.nseq) + ', ' + str(self.nadd) + ')'
         return result
 
 class t2incon(object):
     """Class for a set of initial conditions over a TOUGH2 grid."""
     def __init__(self, filename = '',
-                 read_function = fortran_read_function, num_variables = None):
+                 read_function = fortran_read_function, num_variables = None,
+                 check_blocknames = True):
         self.simulator = 'TOUGH2'
         self.read_function = read_function
         self.empty()
-        if filename: self.read(filename, num_variables)
+        if filename: self.read(filename, num_variables, check_blocknames)
 
     def __getitem__(self, key):
         if isinstance(key, (int, slice)): return self._blocklist[key]
         elif isinstance(key, str): return self._block[key]
         else: return None
     def __setitem__(self, key, value):
         if isinstance(value,(list,tuple)):
@@ -157,15 +158,15 @@
     def delete_incon(self, block):
         """Deletes a t2blockincon."""
         if block in self._block:
             incon = self._block[block]
             del self._block[block]
             self._blocklist.remove(incon)
 
-    def read(self, filename, num_variables = None):
+    def read(self, filename, num_variables = None, check_blocknames = True):
         """Reads initial conditions from file."""
         self.empty()
         mode = 'r' if sys.version_info > (3,) else 'rU'
         infile = t2incon_parser(filename, mode, read_function = self.read_function)
         infile.readline() # skip header
         finished = False
         timing = False
@@ -175,15 +176,16 @@
                 if line.startswith('+++'):
                     finished = True
                     timing = True
                 else:
                     line = padstring(line)
                     [blkname, nseq, nadd, porosity, k1, k2, k3] = \
                         infile.parse_string(line, 'incon1_toughreact')
-                    if valid_blockname(blkname):
+                    valid = valid_blockname(blkname) if check_blocknames else True
+                    if valid:
                         blkname = fix_blockname(blkname)
                         if (k1 is None or k2 is None or k3 is None): permeability = None
                         else:
                             permeability = np.array([k1, k2, k3])
                             self.simulator = 'TOUGHREACT'
                         vals, more = [], True
                         while more:
```

### Comparing `PyTOUGH-1.6.1/t2listing.py` & `PyTOUGH-1.6.2/t2listing.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/t2thermo.py` & `PyTOUGH-1.6.2/t2thermo.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/tests/test_IAPWS97.py` & `PyTOUGH-1.6.2/tests/test_IAPWS97.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/tests/test_geometry.py` & `PyTOUGH-1.6.2/tests/test_geometry.py`

 * *Files 14% similar despite different names*

```diff
@@ -187,14 +187,34 @@
         a = np.array([2., 1.])
         p, xi = line_projection(a, line, True)
         self.assertTrue(np.allclose(np.array([1.5, 1.5]), p))
         self.assertAlmostEqual(1.5, xi)
         d = point_line_distance(a, line)
         self.assertAlmostEqual(sqrt(0.5), d)
 
+    def test_line_intersects_rectangle(self):
+        """line_intersects_rectangle()"""
+        r = [np.array([1., 1.]), np.array([5., 3.])]
+        line = [np.array([0., 0.]), np.array([1., 1.])]
+        self.assertTrue(line_intersects_rectangle(r, line))
+        line = r
+        self.assertTrue(line_intersects_rectangle(r, line))
+        line = r[::-1]
+        self.assertTrue(line_intersects_rectangle(r, line))
+        line = [np.array([1., 1.]), np.array([5., 1.])]
+        self.assertTrue(line_intersects_rectangle(r, line))
+        line = [np.array([3., 1.]), np.array([4., 3.])]
+        self.assertTrue(line_intersects_rectangle(r, line))
+        line = [np.array([3., 0.]), np.array([4., 6.])]
+        self.assertTrue(line_intersects_rectangle(r, line))
+        line = [np.array([2., 2.]), np.array([4., 2.5])]
+        self.assertTrue(line_intersects_rectangle(r, line))
+        line = [np.array([6., 6.]), np.array([8., 0.])]
+        self.assertFalse(line_intersects_rectangle(r, line))
+
     def test_vector_heading(self):
         """vector_heading()"""
         from math import atan
         p = np.array([0., 10.])
         h = vector_heading(p)
         self.assertAlmostEqual(0., h)
```

### Comparing `PyTOUGH-1.6.1/tests/test_mulgrid.py` & `PyTOUGH-1.6.2/tests/test_mulgrid.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,14 +64,17 @@
         blk = 'AA1 6'
         fblk = fix_blockname(blk)
         self.assertNotEqual(fblk[-2], ' ')
         blk2 = unfix_blockname(fblk)
         self.assertEqual(blk, blk2)
         blk = 'A 200'
         self.assertEqual(blk, fix_blockname(blk))
+        blk = 'abcde'
+        self.assertEqual(blk, fix_blockname(blk))
+        self.assertEqual(blk, unfix_blockname(blk))
 
     def test_valid_blockname(self):
         """valid_blockname() function"""
         self.assertTrue(valid_blockname('AA123'))
         self.assertFalse(valid_blockname('AA12a'))
         self.assertTrue(valid_blockname('A   1'))
         self.assertTrue(valid_blockname('A? 21'))
@@ -254,14 +257,101 @@
             t = geo.column_track(geo.bounds)
             found_names = [ts[0].name for ts in t]
             err = False
             self.assertEqual(found_names, names)
         except: err = True
         self.assertFalse(err)
 
+        # track through grid with a corner removed:
+        geo = mulgrid().rectangular([100]*2, [100]*2, [10])
+        geo.translate([1e7, 1e7, 0])
+        geo.delete_column(geo.columnlist[0].name)
+        geo.rotate(30)
+        line = [geo.columnlist[0].centre, geo.columnlist[1].centre]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 2)
+        if len(t) > 1:
+            self.assertEqual(t[0][0].name, geo.columnlist[0].name)
+            self.assertEqual(t[1][0].name, geo.columnlist[1].name)
+
+        # M-grid:
+        geo = mulgrid().rectangular([100]*5, [100]*3, [10])
+        names = [geo.columnlist[i].name for i in [1,3,6,8]]
+        for name in names: geo.delete_column(name)
+        line = [np.array([0, 50]), np.array([500, 50])]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 3)
+        if (len(t) == 3):
+            self.assertEqual(t[0][0].name, geo.columnlist[0].name)
+            self.assertEqual(t[1][0].name, geo.columnlist[1].name)
+            self.assertEqual(t[2][0].name, geo.columnlist[2].name)
+
+        line = line[::-1]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 3)
+        if (len(t) == 3):
+            self.assertEqual(t[0][0].name, geo.columnlist[2].name)
+            self.assertEqual(t[1][0].name, geo.columnlist[1].name)
+            self.assertEqual(t[2][0].name, geo.columnlist[0].name)
+
+        # track within a single column:
+        col = geo.columnlist[-1]
+        p = col.centre
+        d = np.ones(2) * 25
+        line = [p - d, p + d]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 1)
+        if (len(t) == 1):
+            self.assertEqual(t[0][0].name, col.name)
+
+        # track outside grid:
+        line = [np.array([-10, -10]), np.array([600, -200])]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 0)
+
+        # track entirely within grid:
+        line = [np.array([380, 270]), np.array([490, 90])]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 4)
+        self.assertTrue(np.allclose(t[0][1], line[0]))
+        self.assertTrue(np.allclose(t[-1][2], line[1]))
+        if (len(t) == 4):
+            names = [ti[0].name for ti in t]
+            col_ind = [9, 10, 5, 2]
+            expected_names = [geo.columnlist[i].name for i in col_ind]
+            self.assertEqual(names, expected_names)
+
+        # track leaving grid:
+        line = [np.array([250, 50]), np.array([300, -100])]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 1)
+        if (len(t) == 1):
+            self.assertEqual(t[0][0].name, geo.columnlist[1].name)
+            self.assertTrue(np.allclose(t[0][1], line[0]))
+
+        # track entering grid:
+        line = [np.array([270, -50]), np.array([230, 270])]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 3)
+        if (len(t) == 3):
+            names = [ti[0].name for ti in t]
+            col_ind = [1, 4, 8]
+            expected_names = [geo.columnlist[i].name for i in col_ind]
+            self.assertEqual(names, expected_names)
+            self.assertTrue(np.allclose(t[-1][2], line[1]))
+
+        # 5x5 grid:
+        geo = mulgrid().rectangular([100]*5, [100]*5, [10])
+        line = [np.array([100, 100]), np.array([400, 400])]
+        t = geo.column_track(line)
+        self.assertEqual(len(t), 3)
+        if (len(t) == 3):
+            self.assertTrue(np.allclose(t[0][1], line[0]))
+            self.assertTrue(np.allclose(t[-1][2], line[1]))
+
     def test_grid3d(self):
         """3D grid"""
 
         def get_bounding_box(nodes):
             large = 1.e99
             box = []
             for i in range(3): box.append([large, -large])
```

### Comparing `PyTOUGH-1.6.1/tests/test_t2data.py` & `PyTOUGH-1.6.2/tests/test_t2data.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/tests/test_t2grid.py` & `PyTOUGH-1.6.2/tests/test_t2grid.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/tests/test_t2incon.py` & `PyTOUGH-1.6.2/tests/test_t2incon.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/tests/test_t2listing.py` & `PyTOUGH-1.6.2/tests/test_t2listing.py`

 * *Files identical despite different names*

### Comparing `PyTOUGH-1.6.1/tests/test_t2thermo.py` & `PyTOUGH-1.6.2/tests/test_t2thermo.py`

 * *Files identical despite different names*

