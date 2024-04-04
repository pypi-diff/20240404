# Comparing `tmp/utrc-0.0.2.tar.gz` & `tmp/utrc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utrc-0.0.2.tar", last modified: Sun Mar 24 19:53:20 2024, max compression
+gzip compressed data, was "utrc-0.0.3.tar", last modified: Thu Apr  4 12:39:58 2024, max compression
```

## Comparing `utrc-0.0.2.tar` & `utrc-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-24 19:53:20.099711 utrc-0.0.2/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.2/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.2/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3821 2024-03-24 19:53:20.099478 utrc-0.0.2/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.2/README.md
--rw-r--r--   0 solst      (501) staff       (20)      915 2024-03-24 17:52:32.000000 utrc-0.0.2/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-24 19:53:20.099791 utrc-0.0.2/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.2/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-24 19:53:20.097878 utrc-0.0.2/utrc/
--rw-r--r--   0 solst      (501) staff       (20)      936 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    20373 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2561 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/attr.py
--rw-r--r--   0 solst      (501) staff       (20)     7771 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)     3481 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/bend.py
--rw-r--r--   0 solst      (501) staff       (20)     1360 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     1384 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)     8477 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/diff.py
--rw-r--r--   0 solst      (501) staff       (20)    13575 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/dims.py
--rw-r--r--   0 solst      (501) staff       (20)     7586 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/init.py
--rw-r--r--   0 solst      (501) staff       (20)    32638 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/kwds.py
--rw-r--r--   0 solst      (501) staff       (20)     1226 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/logs.py
--rw-r--r--   0 solst      (501) staff       (20)     6563 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/loss.py
--rw-r--r--   0 solst      (501) staff       (20)     3593 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/misc.py
--rw-r--r--   0 solst      (501) staff       (20)     6391 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/perc.py
--rw-r--r--   0 solst      (501) staff       (20)     3327 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/seed.py
--rw-r--r--   0 solst      (501) staff       (20)     5313 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/smpl.py
--rw-r--r--   0 solst      (501) staff       (20)     1084 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/strs.py
--rw-r--r--   0 solst      (501) staff       (20)     9168 2024-03-24 19:52:38.000000 utrc-0.0.2/utrc/tens.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-24 19:53:20.098869 utrc-0.0.2/utrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3821 2024-03-24 19:53:20.000000 utrc-0.0.2/utrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      502 2024-03-24 19:53:20.000000 utrc-0.0.2/utrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 19:53:20.000000 utrc-0.0.2/utrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-24 19:53:20.000000 utrc-0.0.2/utrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.2/utrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      132 2024-03-24 19:53:20.000000 utrc-0.0.2/utrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-24 19:53:20.000000 utrc-0.0.2/utrc.egg-info/top_level.txt
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:39:58.181978 utrc-0.0.3/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.3/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.3/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3841 2024-04-04 12:39:58.181769 utrc-0.0.3/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.3/README.md
+-rw-r--r--   0 solst      (501) staff       (20)      920 2024-04-02 17:48:34.000000 utrc-0.0.3/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-04 12:39:58.182012 utrc-0.0.3/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.3/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:39:58.179904 utrc-0.0.3/utrc/
+-rw-r--r--   0 solst      (501) staff       (20)      936 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    20577 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2561 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/attr.py
+-rw-r--r--   0 solst      (501) staff       (20)     7771 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/bend.py
+-rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     1384 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/diff.py
+-rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/dims.py
+-rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/init.py
+-rw-r--r--   0 solst      (501) staff       (20)    32638 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/kwds.py
+-rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/logs.py
+-rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/loss.py
+-rw-r--r--   0 solst      (501) staff       (20)     5409 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/misc.py
+-rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/perc.py
+-rw-r--r--   0 solst      (501) staff       (20)     3327 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/seed.py
+-rw-r--r--   0 solst      (501) staff       (20)     5313 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/smpl.py
+-rw-r--r--   0 solst      (501) staff       (20)     1084 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/strs.py
+-rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-04 12:39:47.000000 utrc-0.0.3/utrc/tens.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:39:58.181281 utrc-0.0.3/utrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3841 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      502 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.3/utrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      137 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-04 12:39:58.000000 utrc-0.0.3/utrc.egg-info/top_level.txt
```

### Comparing `utrc-0.0.2/LICENSE` & `utrc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/PKG-INFO` & `utrc-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.2
+Version: 0.0.3
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
@@ -24,14 +24,15 @@
 Requires-Dist: nlit
 Requires-Dist: quac
 Requires-Dist: uscr
 Requires-Dist: etrc
 Requires-Dist: slcs
 Requires-Dist: lmsg
 Requires-Dist: dtyp
+Requires-Dist: zipr
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

### Comparing `utrc-0.0.2/README.md` & `utrc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/settings.ini` & `utrc-0.0.3/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utrc
 lib_name = utrc
-version = 0.0.2
+version = 0.0.3
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = utrc
 nbs_path = nbs
 recursive = True
@@ -29,10 +29,10 @@
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-requirements = astr atup chck dref lull nchr nlit quac uscr etrc slcs lmsg dtyp
+requirements = astr atup chck dref lull nchr nlit quac uscr etrc slcs lmsg dtyp zipr
 dev_requirements = numpy pandas matplotlib torch pytorch_lightning torchvision
```

### Comparing `utrc-0.0.2/setup.py` & `utrc-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/__init__.py` & `utrc-0.0.3/utrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `utrc-0.0.2/utrc/_modidx.py` & `utrc-0.0.3/utrc/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,17 @@
                            'utrc.loss.MMDLoss.__init__': ('loss.html#mmdloss.__init__', 'utrc/loss.py'),
                            'utrc.loss.MMDLoss.forward': ('loss.html#mmdloss.forward', 'utrc/loss.py'),
                            'utrc.loss.MMDLoss.guassian_kernel': ('loss.html#mmdloss.guassian_kernel', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss': ('loss.html#optimaltransportloss', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss.__call__': ('loss.html#optimaltransportloss.__call__', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss.__init__': ('loss.html#optimaltransportloss.__init__', 'utrc/loss.py')},
             'utrc.misc': { 'utrc.misc.calcgrid': ('misc.html#calcgrid', 'utrc/misc.py'),
+                           'utrc.misc.generate_steps': ('misc.html#generate_steps', 'utrc/misc.py'),
                            'utrc.misc.grididx': ('misc.html#grididx', 'utrc/misc.py'),
+                           'utrc.misc.increment_pairs': ('misc.html#increment_pairs', 'utrc/misc.py'),
                            'utrc.misc.pad4grid': ('misc.html#pad4grid', 'utrc/misc.py'),
                            'utrc.misc.pair': ('misc.html#pair', 'utrc/misc.py'),
                            'utrc.misc.steps': ('misc.html#steps', 'utrc/misc.py'),
                            'utrc.misc.takekeys': ('misc.html#takekeys', 'utrc/misc.py')},
             'utrc.perc': { 'utrc.perc.accumulate_percents': ('perc.html#accumulate_percents', 'utrc/perc.py'),
                            'utrc.perc.apercents': ('perc.html#apercents', 'utrc/perc.py'),
                            'utrc.perc.idxstep': ('perc.html#idxstep', 'utrc/perc.py'),
```

### Comparing `utrc-0.0.2/utrc/attr.py` & `utrc-0.0.3/utrc/attr.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/atyp.py` & `utrc-0.0.3/utrc/atyp.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/bend.py` & `utrc-0.0.3/utrc/bend.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/cons.py` & `utrc-0.0.3/utrc/cons.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/data.py` & `utrc-0.0.3/utrc/data.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/diff.py` & `utrc-0.0.3/utrc/diff.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/dims.py` & `utrc-0.0.3/utrc/dims.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/init.py` & `utrc-0.0.3/utrc/init.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/kwds.py` & `utrc-0.0.3/utrc/kwds.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/logs.py` & `utrc-0.0.3/utrc/logs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/loss.py` & `utrc-0.0.3/utrc/loss.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/misc.py` & `utrc-0.0.3/utrc/misc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/10_misc.ipynb.
 
 # %% auto 0
-__all__ = ['pair', 'steps', 'calcgrid', 'grididx', 'pad4grid', 'takekeys']
+__all__ = ['pair', 'steps', 'increment_pairs', 'generate_steps', 'calcgrid', 'grididx', 'pad4grid', 'takekeys']
 
 # %% ../nbs/10_misc.ipynb 6
 import math
-from functools import wraps
+from functools import wraps, singledispatch
+from itertools import takewhile, count
 
 # %% ../nbs/10_misc.ipynb 8
-from typing import Iterable, overload
+from numbers import Number
+from typing import Generator, Iterator, Iterable, overload
 
 # %% ../nbs/10_misc.ipynb 11
 #| export
 
 # %% ../nbs/10_misc.ipynb 13
 #| export
 
@@ -23,16 +25,16 @@
 
 # %% ../nbs/10_misc.ipynb 17
 #| export
 
 
 # %% ../nbs/10_misc.ipynb 19
 from atup import fillnone
-from chck import isdict
 from quac import nums, rect, xypos
+from chck import isdict
 
 # %% ../nbs/10_misc.ipynb 21
 from .cons import WRAPS_ASSIGN_ANNDOCS
 
 # %% ../nbs/10_misc.ipynb 23
 def pair(a: nums, n: int = 2, i: int = 1) -> tuple[nums, ...]:
     '''Pair numbers in an array
@@ -72,15 +74,68 @@
     return tuple(zip(a, *(a[(i * _):] for _ in range(1, n))))
 
 @wraps(pair, assigned=WRAPS_ASSIGN_ANNDOCS)
 def steps(*args, **kwargs):
     '''Alias for `pair`.'''
     return pair(*args, **kwargs)
 
+@wraps(pair, assigned=WRAPS_ASSIGN_ANNDOCS)
+def increment_pairs(*args, **kwargs):
+    return pair(*args, **kwargs)
+
 # %% ../nbs/10_misc.ipynb 26
+def generate_steps(incr, step, stop):
+    '''
+    Generate a list of tuples representing step intervals from 0 up to stop,
+    incrementing by incr and ensuring each step interval does not exceed step.
+    
+    Parameters
+    ----------
+    incr : int
+        The increment between each start of the step intervals.
+    step : int
+        The maximum allowed difference between the start and end of each interval.
+    stop : int
+        The stopping point for the generation of intervals.
+    
+    Returns
+    -------
+    list of tuples
+        A list of tuples, where each tuple contains the start and end of each step interval.
+        
+    Examples
+    --------
+    >>> incr = 3
+    ... step = 2
+    ... stop = 10
+    ... vals = generate_steps(incr, step, stop)
+
+    ... firstvals = [v[0] for v in vals]
+    ... firstdiff = tuple(b - a for a, b in zip(firstvals, firstvals[1:]))
+
+    ... step_diff = tuple(b - a for a, b in vals)
+    ... good_step = all(e <= step for e in step_diff)
+
+    ... good_end = vals[-1][-1] == stop
+    ... good_inc = all(e == incr for e in firstdiff)
+
+    ... # each tuple increments by +incr, has a (a, b) diff of <= step and ends at stop
+    ... all_valid = good_inc and good_step and good_end
+    ... vals, all_valid
+
+    '''
+    # Use takewhile to generate values up to the stop condition
+    vals_gen = takewhile(lambda x: x < stop, count(0, incr))
+    
+    # Generate the list of tuples with the specified conditions
+    vals = [(i, min(i + step, stop)) for i in vals_gen]
+    
+    return vals
+
+# %% ../nbs/10_misc.ipynb 32
 def calcgrid(n: int) -> rect:
     '''
     Find the closest rectangle layout that accommodates n elements.
 
     Parameters
     ----------
     n : int
@@ -92,15 +147,15 @@
         A tuple representing the dimensions (rows, cols) of the grid.
     '''
     x = math.isqrt(n)
     while n % x != 0: x -= 1
     y = n // x
     return x, y
 
-# %% ../nbs/10_misc.ipynb 28
+# %% ../nbs/10_misc.ipynb 34
 def grididx(pos: xypos, grid: rect) -> int:
     '''
     Calculate the linear index of an element in a `grid` given its `(row, col)` position (`pos`).
 
     Parameters
     ----------
     pos : XYPos
@@ -113,15 +168,15 @@
     int
         The linear index of the element in the grid.
     '''
     nrows, ncols = grid
     cur_r, cur_c = pos
     return cur_r * ncols + cur_c
 
-# %% ../nbs/10_misc.ipynb 30
+# %% ../nbs/10_misc.ipynb 36
 @overload
 def pad4grid(arr: list, rows: int, cols: int) -> list: ...
 @overload
 def pad4grid(arr: list, n: int) -> list: ...
 def pad4grid(arr: list, *args) -> list:
     '''
     Pad the list of objects to the closest grid layout that accommodates a specified number of elements.
@@ -137,15 +192,15 @@
     -------
     list
         The padded list.
     '''
     rows, cols = args[0], (1 if len(args) <= 1 else args[1])
     return list(fillnone(arr, rows * cols))
 
-# %% ../nbs/10_misc.ipynb 32
+# %% ../nbs/10_misc.ipynb 38
 def takekeys(d: dict, keys: list | dict) -> dict:
     keys = keys or []
     if isdict(keys): keys = keys.keys()
     return {k: d.get(k, None) for k in keys if k in d}
 
-# %% ../nbs/10_misc.ipynb 34
+# %% ../nbs/10_misc.ipynb 40
 #| export
```

### Comparing `utrc-0.0.2/utrc/perc.py` & `utrc-0.0.3/utrc/perc.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/seed.py` & `utrc-0.0.3/utrc/seed.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/smpl.py` & `utrc-0.0.3/utrc/smpl.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/strs.py` & `utrc-0.0.3/utrc/strs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc/tens.py` & `utrc-0.0.3/utrc/tens.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.2/utrc.egg-info/PKG-INFO` & `utrc-0.0.3/utrc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.2
+Version: 0.0.3
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
@@ -24,14 +24,15 @@
 Requires-Dist: nlit
 Requires-Dist: quac
 Requires-Dist: uscr
 Requires-Dist: etrc
 Requires-Dist: slcs
 Requires-Dist: lmsg
 Requires-Dist: dtyp
+Requires-Dist: zipr
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

