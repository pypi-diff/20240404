# Comparing `tmp/ions-0.3.0.tar.gz` & `tmp/ions-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ions-0.3.0.tar", last modified: Mon Apr  1 16:21:49 2024, max compression
+gzip compressed data, was "ions-0.3.1.tar", last modified: Thu Apr  4 14:44:25 2024, max compression
```

## Comparing `ions-0.3.0.tar` & `ions-0.3.1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:21:49.361981 ions-0.3.0/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.3.0/LICENSE
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.3.0/MANIFEST.in
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 16:21:49.361771 ions-0.3.0/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10819 2024-03-05 07:10:45.000000 ions-0.3.0/README.md
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:21:49.340077 ions-0.3.0/ions/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.3.0/ions/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7322 2023-12-29 14:18:01.000000 ions-0.3.0/ions/calculators.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:21:49.359420 ions-0.3.0/ions/data/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.3.0/ions/data/Li2O_mp-1960.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.3.0/ions/data/bvparam_1991.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/bvparams2020-average.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/bvparams2020-average.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/bvparams_averaged2020.csv
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.3.0/ions/data/bvparm2020.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.3.0/ions/data/bvparm2020_edit.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/bvse_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/bvse_data.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.3.0/ions/data/elneg_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.3.0/ions/data/icsd_bv.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.3.0/ions/data/icsd_bv_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.3.0/ions/data/quantum_n.pkl
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/shannon-data-crystal.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/shannon-data-crystal.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/shannon-data-ionic.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/shannon-data-ionic.pickle
--rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.3.0/ions/data/shannon-radii.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.3.0/ions/data/shannon-radii.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.3.0/ions/data.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2023-12-28 12:26:57.000000 ions-0.3.0/ions/decorator.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:21:49.359974 ions-0.3.0/ions/featurizers/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       44 2024-04-01 14:09:37.000000 ions-0.3.0/ions/featurizers/__init__.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:21:49.360503 ions-0.3.0/ions/geom/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       22 2024-04-01 10:11:35.000000 ions-0.3.0/ions/geom/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     9060 2024-04-01 16:18:51.000000 ions-0.3.0/ions/geom/edge.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2023-12-29 18:07:12.000000 ions-0.3.0/ions/potential.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:21:49.361309 ions-0.3.0/ions/tools/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       86 2024-04-01 14:11:28.000000 ions-0.3.0/ions/tools/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    19592 2024-04-01 14:15:22.000000 ions-0.3.0/ions/tools/path_finder.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7061 2024-03-04 19:36:00.000000 ions-0.3.0/ions/tools/saddle_finder.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4230 2024-04-01 12:24:32.000000 ions-0.3.0/ions/utils.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:21:49.341115 ions-0.3.0/ions.egg-info/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 16:21:49.000000 ions-0.3.0/ions.egg-info/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1000 2024-04-01 16:21:49.000000 ions-0.3.0/ions.egg-info/SOURCES.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-04-01 16:21:49.000000 ions-0.3.0/ions.egg-info/dependency_links.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       49 2024-04-01 16:21:49.000000 ions-0.3.0/ions.egg-info/requires.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-04-01 16:21:49.000000 ions-0.3.0/ions.egg-info/top_level.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-04-01 16:21:49.362039 ions-0.3.0/setup.cfg
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1537 2024-04-01 16:19:04.000000 ions-0.3.0/setup.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-04 14:44:25.234592 ions-0.3.1/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.3.1/LICENSE
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.3.1/MANIFEST.in
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    12151 2024-04-04 14:44:25.234394 ions-0.3.1/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11435 2024-04-04 13:33:19.000000 ions-0.3.1/README.md
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-04 14:44:25.228133 ions-0.3.1/ions/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.3.1/ions/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7429 2024-04-04 13:13:20.000000 ions-0.3.1/ions/calculators.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-04 14:44:25.232726 ions-0.3.1/ions/data/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.3.1/ions/data/Li2O_mp-1960.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.3.1/ions/data/bvparam_1991.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/bvparams2020-average.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/bvparams2020-average.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/bvparams_averaged2020.csv
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.3.1/ions/data/bvparm2020.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.3.1/ions/data/bvparm2020_edit.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/bvse_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/bvse_data.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.3.1/ions/data/elneg_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.3.1/ions/data/icsd_bv.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.3.1/ions/data/icsd_bv_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.3.1/ions/data/quantum_n.pkl
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/shannon-data-crystal.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/shannon-data-crystal.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/shannon-data-ionic.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/shannon-data-ionic.pickle
+-rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.3.1/ions/data/shannon-radii.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.3.1/ions/data/shannon-radii.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.3.1/ions/data.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2024-04-04 13:35:35.000000 ions-0.3.1/ions/decorator.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-04 14:44:25.232911 ions-0.3.1/ions/featurizers/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       44 2024-04-01 14:09:37.000000 ions-0.3.1/ions/featurizers/__init__.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-04 14:44:25.233394 ions-0.3.1/ions/geom/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       43 2024-04-03 14:03:20.000000 ions-0.3.1/ions/geom/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     2326 2024-04-04 13:03:40.000000 ions-0.3.1/ions/geom/box.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4267 2024-04-04 14:32:28.000000 ions-0.3.1/ions/geom/edge.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2023-12-29 18:07:12.000000 ions-0.3.1/ions/potential.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-04 14:44:25.234140 ions-0.3.1/ions/tools/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      120 2024-04-04 10:15:21.000000 ions-0.3.1/ions/tools/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    19639 2024-04-04 08:40:31.000000 ions-0.3.1/ions/tools/path_finder.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    15102 2024-04-04 13:01:13.000000 ions-0.3.1/ions/tools/percolator.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3161 2024-04-04 13:04:00.000000 ions-0.3.1/ions/tools/saddle_finder.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4742 2024-04-04 06:53:48.000000 ions-0.3.1/ions/utils.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-04 14:44:25.228841 ions-0.3.1/ions.egg-info/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    12151 2024-04-04 14:44:25.000000 ions-0.3.1/ions.egg-info/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1042 2024-04-04 14:44:25.000000 ions-0.3.1/ions.egg-info/SOURCES.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-04-04 14:44:25.000000 ions-0.3.1/ions.egg-info/dependency_links.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       49 2024-04-04 14:44:25.000000 ions-0.3.1/ions.egg-info/requires.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-04-04 14:44:25.000000 ions-0.3.1/ions.egg-info/top_level.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-04-04 14:44:25.234659 ions-0.3.1/setup.cfg
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1537 2024-04-04 13:14:44.000000 ions-0.3.1/setup.py
```

### Comparing `ions-0.3.0/LICENSE` & `ions-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/PKG-INFO` & `ions-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -49,113 +49,100 @@
 ```pip install ions```
 
 #### Maximum percolation dimensionality and minimum required jump distance
 
 
 ```python
 from ase.io import read, write
-from ions.tools import PathFinder
+from ions.tools import Percolator
 
 file = '/Users/artemdembitskiy/Downloads/LiFePO4.cif'
 atoms = read(file)  
 
 specie = 3
-pf = PathFinder(atoms, specie, 10.0)
+pr = Percolator(atoms, specie, 10.0)
 
 tr = 0.5 # Minimum allowed distance between the edge and the framework
-cutoff, max_dim = pf.mincut_maxdim(tr)
+cutoff, dim = pr.mincut_maxdim(tr)
 
-print(f'Maximum percolation dimensionality: {max_dim}')
+print(f'Maximum percolation dimensionality: {dim}')
 print(f'Jump distance cutoff: {cutoff} angstrom')
 ```
 
     Maximum percolation dimensionality: 3
     Jump distance cutoff: 5.7421875 angstrom
 
 
 
 ```python
-pf.percolation_threshold(1), pf.percolation_threshold(2), pf.percolation_threshold(3)
+pr.percolation_threshold(1), pr.percolation_threshold(2), pr.percolation_threshold(3)
 ```
 
 
 
 
     (1.582, 1.4551, 0.9668)
 
 
 
-#### Save percolating network
-
-
-```python
-traj = pf.create_percotraj(cutoff, tr)
-write('perolating_sublattice.cif', traj) # jumps between nearest neighbors are linearly interpolated within 2x2x2 supercell
-```
-
 #### Inequivalent ionic hops forming percolating netwrok
 
 
 ```python
-edges, features = pf.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
-edges, features
+edges, features = pr.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
+edges
 ```
 
 
 
 
-    (array([[2, 3, 0, 0, 0],
-            [0, 1, 1, 0, 0],
-            [0, 3, 1, 0, 0],
-            [0, 3, 1, 1, 0],
-            [2, 1, 0, 1, 0],
-            [0, 0, 1, 0, 0]]),
-     array([[0.   , 0.   , 0.589, 5.736],
-            [0.   , 0.   , 0.66 , 5.736],
-            [0.   , 0.   , 0.695, 5.639],
-            [0.   , 0.   , 0.696, 5.639],
-            [0.   , 0.   , 1.461, 3.045],
-            [0.   , 0.   , 1.587, 4.746]]))
+    [Edge(0,1,[0 0 0], d=5.74, wrapped_target=1'),
+     Edge(0,3,[1 0 0], d=5.64, wrapped_target=3'),
+     Edge(0,3,[0 0 0], d=3.05, wrapped_target=3'),
+     Edge(0,0,[1 0 0], d=4.75, wrapped_target=0')]
 
 
 
 #### Find saddle point for each ionic hop using bond valence force field potential
 
 
 ```python
 import numpy as np
 from ase.io import read, write
 from ase.optimize import FIRE
 
 from ions.tools import SaddleFinder
 from ions.decorator import Decorator
+from ions.utils import collect_bvse_params
 
 
 Decorator().decorate(atoms) # oxidation states are required for this method
+collect_bvse_params(atoms, 'Li', +1, self_interaction=True) # do not omit Li-Li interaction
+pr = Percolator(atoms, specie, 10.0)
+edges, _ = pr.unique_edges(cutoff, tr)
 
-sf = SaddleFinder(self_interaction=True) # do not omit Li-Li interaction
 traj = []
 for i, edge in enumerate(edges):
-    source, target = edge[:2]
-    offset = edge[2:]
-    images, atoms_mod, offset = sf.interpolate(atoms, source, target, offset, min_sep_dist = 6.0, spacing = .75, abc = True)
+    superedge = edge.superedge(10.0, center = True) # put centroid of the edge in the center of the box
+    images = superedge.interpolate(spacing = 0.75)
+    sf = SaddleFinder()
+    neb = sf.bvse_neb(images)
+    optim = FIRE(neb,
+                    logfile = 'log'
+                    )
     traj.append(images)
-    neb = sf.bvse_neb(images, k = 2.0, gm = True) # Note that images are linked to the neb object and will be changed after optimization
-    optimizer = FIRE(neb, logfile = 'log')
-    optimizer.run(fmax =.1, steps = 100)
+    optim.run(fmax = 0.1, steps = 100)
     print(f'Unique jump #{i}: Fmax {neb.get_forces().max().round(2)} eV/angstrom |',
          f'Activation barrier {sf.get_barrier(images).round(2)} eV')
 ```
 
-    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.15 eV
-    Unique jump #1: Fmax 1.0 eV/angstrom | Activation barrier 4.14 eV
-    Unique jump #2: Fmax 0.08 eV/angstrom | Activation barrier 3.45 eV
-    Unique jump #3: Fmax 0.42 eV/angstrom | Activation barrier 4.89 eV
-    Unique jump #4: Fmax 0.09 eV/angstrom | Activation barrier 0.38 eV
-    Unique jump #5: Fmax 0.06 eV/angstrom | Activation barrier 3.28 eV
+    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.26 eV
+    Unique jump #1: Fmax 0.05 eV/angstrom | Activation barrier 3.56 eV
+    Unique jump #2: Fmax 0.09 eV/angstrom | Activation barrier 0.33 eV
+    Unique jump #3: Fmax 0.05 eV/angstrom | Activation barrier 3.3 eV
 
 
 #### Plot profile
 
 
 ```python
 import matplotlib.pyplot as plt
@@ -179,81 +166,116 @@
     ax.legend(frameon = False)
 axes[0].set_ylabel('Energy, eV')
 plt.tight_layout()
 ```
 
 
     
-![png](example_files/example_13_0.png)
+![png](example_files/example_11_0.png)
     
 
 
 #### Percolation dimensionality study (I found some inconsistency, don't use until update)
 
 
 ```python
 emins = []
 emaxs = []
 for images in traj:
+    
     emins.append(sf.get_profile(images).min())
     emaxs.append(sf.get_profile(images).max())
 
-for i, dim in enumerate(np.arange(1, max_dim + 1)):
-    e_a, tr_min, tr_max = pf.propagate_barriers(cutoff, tr, emins, emaxs, dim)
-    print(f'Activation barrier of {i + 1}D percolation: {round(e_a, 2)} eV')
+for d in range(1, dim + 1):
+   ea, tr_min, tr_max = pr.propagate_barriers(cutoff, tr, emins, emaxs, d)
+   print(f'{d}D percolations barrier: {round(ea, 3)}')
+
 ```
 
-    Activation barrier of 1D percolation: 3.28 eV
-    Activation barrier of 2D percolation: 3.45 eV
-    Activation barrier of 3D percolation: 3.45 eV
+    1D percolations barrier: 0.331
+    2D percolations barrier: 3.258
+    3D percolations barrier: 3.313
 
 
 #### Put all together
 
 
 ```python
+import numpy as np
 from ase.io import read, write
-from ions.tools import PathFinder, SaddleFinder
+from ase.optimize import FIRE
+from ions.tools import SaddleFinder
+from ions.decorator import Decorator
+from ions.utils import collect_bvse_params
+import matplotlib.pyplot as plt
+from scipy.interpolate import pchip_interpolate
 
-file = '/Users/artemdembitskiy/Downloads/LiFePO4.cif'
-atoms = read(file)  
-Decorator().decorate(atoms) # oxidation states are required for this method
+plt.rcParams.update({'font.size': 8})
+plt.rcParams.update({'font.family': 'Arial'})
 
-specie = 3
-pf = PathFinder(atoms, specie, 10.0)
 
-tr = 0.5 # Minimum allowed distance between the edge and the framework
-cutoff, max_dim = pf.mincut_maxdim(tr)
-edges, features = pf.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
 
-sf = SaddleFinder(self_interaction=True) # do not omit Li-Li interaction
+Decorator().decorate(atoms) # oxidation states are required for this method
+collect_bvse_params(atoms, 'Li', +1, self_interaction=True) # do not omit Li-Li interaction
+pr = Percolator(atoms, specie, 10.0)
+edges, _ = pr.unique_edges(cutoff, tr)
+
 traj = []
 emins = []
 emaxs = []
-for edge in edges:
-    source, target = edge[:2]
-    offset = edge[2:]
-    images, atoms_mod, offset = sf.interpolate(atoms, source, target, offset, min_sep_dist = 10.0, spacing = 0.5)
+for i, edge in enumerate(edges):
+    superedge = edge.superedge(10.0, center = True) # put centroid of the edge in the center of the box
+    images = superedge.interpolate(spacing = 0.75)
+    sf = SaddleFinder()
+    neb = sf.bvse_neb(images)
+    optim = FIRE(neb,
+                    logfile = 'log'
+                    )
+    
+    optim.run(fmax = 0.1, steps = 100)
+    print(f'Unique jump #{i}: Fmax {neb.get_forces().max().round(2)} eV/angstrom |',
+         f'Activation barrier {sf.get_barrier(images).round(2)} eV')
     traj.append(images)
-    neb = sf.bvse_neb(images, k = 5.0, gm = True) # Note that images are linked to the neb object and will be changed after optimization
-    optimizer = FIRE(neb, logfile = 'log')
-    optimizer.run(fmax =.1, steps = 100)
     emins.append(sf.get_profile(images).min())
     emaxs.append(sf.get_profile(images).max())
 
+for d in range(1, dim + 1):
+   ea, tr_min, tr_max = pr.propagate_barriers(cutoff, tr, emins, emaxs, d)
+   print(f'{d}D percolations barrier: {round(ea, 3)}')
 
-for dim in np.arange(1, max_dim + 1):
-    e_a, tr_min, tr_max = pf.propagate_barriers(cutoff, tr, emins, emaxs, dim)
-    print(f'Activation barrier of {dim}D percolation: {round(e_a, 2)} eV')
 
+
+fig, axes = plt.subplots(dpi = 600, figsize = (12, 2.5), ncols = len(traj), sharey  = True)
+for ax, images in zip(axes, traj):
+    profile = sf.get_profile(images)
+    x = np.arange(0, len(images))
+    x_fit = np.linspace(0, len(images), 100)
+    y_fit = pchip_interpolate(x, profile, x_fit)
+    ax.plot(x, profile, 'o', label = 'calculated')
+    ax.plot(x_fit, y_fit, zorder = 1, label = 'pchip fit', color = 'darkred')
+    ax.set_xlabel('Reaction coordinate')
+    ax.set_xlim(x.min(), x.max())
+    ax.legend(frameon = False)
+axes[0].set_ylabel('Energy, eV')
+plt.tight_layout()
 ```
 
-    Activation barrier of 1D percolation: 3.29 eV
-    Activation barrier of 2D percolation: 3.56 eV
-    Activation barrier of 3D percolation: 3.56 eV
+    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.26 eV
+    Unique jump #1: Fmax 0.05 eV/angstrom | Activation barrier 3.56 eV
+    Unique jump #2: Fmax 0.09 eV/angstrom | Activation barrier 0.33 eV
+    Unique jump #3: Fmax 0.05 eV/angstrom | Activation barrier 3.3 eV
+    1D percolations barrier: 0.331
+    2D percolations barrier: 3.258
+    3D percolations barrier: 3.313
+
+
+
+    
+![png](example_files/example_15_1.png)
+    
 
 
 #### Compare with BVSE meshgrid approach (i.e. empty lattice)
 
 
 ```python
 from bvlain import Lain
@@ -406,7 +428,17 @@
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
 
 
 
+```python
+!jupyter nbconvert --to markdown example.ipynb
+```
+
+    [NbConvertApp] Converting notebook example.ipynb to markdown
+    [NbConvertApp] Support files will be in example_files/
+    [NbConvertApp] Writing 10819 bytes to example.md
+
+
+
```

### Comparing `ions-0.3.0/README.md` & `ions-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -29,113 +29,100 @@
 ```pip install ions```
 
 #### Maximum percolation dimensionality and minimum required jump distance
 
 
 ```python
 from ase.io import read, write
-from ions.tools import PathFinder
+from ions.tools import Percolator
 
 file = '/Users/artemdembitskiy/Downloads/LiFePO4.cif'
 atoms = read(file)  
 
 specie = 3
-pf = PathFinder(atoms, specie, 10.0)
+pr = Percolator(atoms, specie, 10.0)
 
 tr = 0.5 # Minimum allowed distance between the edge and the framework
-cutoff, max_dim = pf.mincut_maxdim(tr)
+cutoff, dim = pr.mincut_maxdim(tr)
 
-print(f'Maximum percolation dimensionality: {max_dim}')
+print(f'Maximum percolation dimensionality: {dim}')
 print(f'Jump distance cutoff: {cutoff} angstrom')
 ```
 
     Maximum percolation dimensionality: 3
     Jump distance cutoff: 5.7421875 angstrom
 
 
 
 ```python
-pf.percolation_threshold(1), pf.percolation_threshold(2), pf.percolation_threshold(3)
+pr.percolation_threshold(1), pr.percolation_threshold(2), pr.percolation_threshold(3)
 ```
 
 
 
 
     (1.582, 1.4551, 0.9668)
 
 
 
-#### Save percolating network
-
-
-```python
-traj = pf.create_percotraj(cutoff, tr)
-write('perolating_sublattice.cif', traj) # jumps between nearest neighbors are linearly interpolated within 2x2x2 supercell
-```
-
 #### Inequivalent ionic hops forming percolating netwrok
 
 
 ```python
-edges, features = pf.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
-edges, features
+edges, features = pr.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
+edges
 ```
 
 
 
 
-    (array([[2, 3, 0, 0, 0],
-            [0, 1, 1, 0, 0],
-            [0, 3, 1, 0, 0],
-            [0, 3, 1, 1, 0],
-            [2, 1, 0, 1, 0],
-            [0, 0, 1, 0, 0]]),
-     array([[0.   , 0.   , 0.589, 5.736],
-            [0.   , 0.   , 0.66 , 5.736],
-            [0.   , 0.   , 0.695, 5.639],
-            [0.   , 0.   , 0.696, 5.639],
-            [0.   , 0.   , 1.461, 3.045],
-            [0.   , 0.   , 1.587, 4.746]]))
+    [Edge(0,1,[0 0 0], d=5.74, wrapped_target=1'),
+     Edge(0,3,[1 0 0], d=5.64, wrapped_target=3'),
+     Edge(0,3,[0 0 0], d=3.05, wrapped_target=3'),
+     Edge(0,0,[1 0 0], d=4.75, wrapped_target=0')]
 
 
 
 #### Find saddle point for each ionic hop using bond valence force field potential
 
 
 ```python
 import numpy as np
 from ase.io import read, write
 from ase.optimize import FIRE
 
 from ions.tools import SaddleFinder
 from ions.decorator import Decorator
+from ions.utils import collect_bvse_params
 
 
 Decorator().decorate(atoms) # oxidation states are required for this method
+collect_bvse_params(atoms, 'Li', +1, self_interaction=True) # do not omit Li-Li interaction
+pr = Percolator(atoms, specie, 10.0)
+edges, _ = pr.unique_edges(cutoff, tr)
 
-sf = SaddleFinder(self_interaction=True) # do not omit Li-Li interaction
 traj = []
 for i, edge in enumerate(edges):
-    source, target = edge[:2]
-    offset = edge[2:]
-    images, atoms_mod, offset = sf.interpolate(atoms, source, target, offset, min_sep_dist = 6.0, spacing = .75, abc = True)
+    superedge = edge.superedge(10.0, center = True) # put centroid of the edge in the center of the box
+    images = superedge.interpolate(spacing = 0.75)
+    sf = SaddleFinder()
+    neb = sf.bvse_neb(images)
+    optim = FIRE(neb,
+                    logfile = 'log'
+                    )
     traj.append(images)
-    neb = sf.bvse_neb(images, k = 2.0, gm = True) # Note that images are linked to the neb object and will be changed after optimization
-    optimizer = FIRE(neb, logfile = 'log')
-    optimizer.run(fmax =.1, steps = 100)
+    optim.run(fmax = 0.1, steps = 100)
     print(f'Unique jump #{i}: Fmax {neb.get_forces().max().round(2)} eV/angstrom |',
          f'Activation barrier {sf.get_barrier(images).round(2)} eV')
 ```
 
-    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.15 eV
-    Unique jump #1: Fmax 1.0 eV/angstrom | Activation barrier 4.14 eV
-    Unique jump #2: Fmax 0.08 eV/angstrom | Activation barrier 3.45 eV
-    Unique jump #3: Fmax 0.42 eV/angstrom | Activation barrier 4.89 eV
-    Unique jump #4: Fmax 0.09 eV/angstrom | Activation barrier 0.38 eV
-    Unique jump #5: Fmax 0.06 eV/angstrom | Activation barrier 3.28 eV
+    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.26 eV
+    Unique jump #1: Fmax 0.05 eV/angstrom | Activation barrier 3.56 eV
+    Unique jump #2: Fmax 0.09 eV/angstrom | Activation barrier 0.33 eV
+    Unique jump #3: Fmax 0.05 eV/angstrom | Activation barrier 3.3 eV
 
 
 #### Plot profile
 
 
 ```python
 import matplotlib.pyplot as plt
@@ -159,81 +146,116 @@
     ax.legend(frameon = False)
 axes[0].set_ylabel('Energy, eV')
 plt.tight_layout()
 ```
 
 
     
-![png](example_files/example_13_0.png)
+![png](example_files/example_11_0.png)
     
 
 
 #### Percolation dimensionality study (I found some inconsistency, don't use until update)
 
 
 ```python
 emins = []
 emaxs = []
 for images in traj:
+    
     emins.append(sf.get_profile(images).min())
     emaxs.append(sf.get_profile(images).max())
 
-for i, dim in enumerate(np.arange(1, max_dim + 1)):
-    e_a, tr_min, tr_max = pf.propagate_barriers(cutoff, tr, emins, emaxs, dim)
-    print(f'Activation barrier of {i + 1}D percolation: {round(e_a, 2)} eV')
+for d in range(1, dim + 1):
+   ea, tr_min, tr_max = pr.propagate_barriers(cutoff, tr, emins, emaxs, d)
+   print(f'{d}D percolations barrier: {round(ea, 3)}')
+
 ```
 
-    Activation barrier of 1D percolation: 3.28 eV
-    Activation barrier of 2D percolation: 3.45 eV
-    Activation barrier of 3D percolation: 3.45 eV
+    1D percolations barrier: 0.331
+    2D percolations barrier: 3.258
+    3D percolations barrier: 3.313
 
 
 #### Put all together
 
 
 ```python
+import numpy as np
 from ase.io import read, write
-from ions.tools import PathFinder, SaddleFinder
+from ase.optimize import FIRE
+from ions.tools import SaddleFinder
+from ions.decorator import Decorator
+from ions.utils import collect_bvse_params
+import matplotlib.pyplot as plt
+from scipy.interpolate import pchip_interpolate
 
-file = '/Users/artemdembitskiy/Downloads/LiFePO4.cif'
-atoms = read(file)  
-Decorator().decorate(atoms) # oxidation states are required for this method
+plt.rcParams.update({'font.size': 8})
+plt.rcParams.update({'font.family': 'Arial'})
 
-specie = 3
-pf = PathFinder(atoms, specie, 10.0)
 
-tr = 0.5 # Minimum allowed distance between the edge and the framework
-cutoff, max_dim = pf.mincut_maxdim(tr)
-edges, features = pf.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
 
-sf = SaddleFinder(self_interaction=True) # do not omit Li-Li interaction
+Decorator().decorate(atoms) # oxidation states are required for this method
+collect_bvse_params(atoms, 'Li', +1, self_interaction=True) # do not omit Li-Li interaction
+pr = Percolator(atoms, specie, 10.0)
+edges, _ = pr.unique_edges(cutoff, tr)
+
 traj = []
 emins = []
 emaxs = []
-for edge in edges:
-    source, target = edge[:2]
-    offset = edge[2:]
-    images, atoms_mod, offset = sf.interpolate(atoms, source, target, offset, min_sep_dist = 10.0, spacing = 0.5)
+for i, edge in enumerate(edges):
+    superedge = edge.superedge(10.0, center = True) # put centroid of the edge in the center of the box
+    images = superedge.interpolate(spacing = 0.75)
+    sf = SaddleFinder()
+    neb = sf.bvse_neb(images)
+    optim = FIRE(neb,
+                    logfile = 'log'
+                    )
+    
+    optim.run(fmax = 0.1, steps = 100)
+    print(f'Unique jump #{i}: Fmax {neb.get_forces().max().round(2)} eV/angstrom |',
+         f'Activation barrier {sf.get_barrier(images).round(2)} eV')
     traj.append(images)
-    neb = sf.bvse_neb(images, k = 5.0, gm = True) # Note that images are linked to the neb object and will be changed after optimization
-    optimizer = FIRE(neb, logfile = 'log')
-    optimizer.run(fmax =.1, steps = 100)
     emins.append(sf.get_profile(images).min())
     emaxs.append(sf.get_profile(images).max())
 
+for d in range(1, dim + 1):
+   ea, tr_min, tr_max = pr.propagate_barriers(cutoff, tr, emins, emaxs, d)
+   print(f'{d}D percolations barrier: {round(ea, 3)}')
 
-for dim in np.arange(1, max_dim + 1):
-    e_a, tr_min, tr_max = pf.propagate_barriers(cutoff, tr, emins, emaxs, dim)
-    print(f'Activation barrier of {dim}D percolation: {round(e_a, 2)} eV')
 
+
+fig, axes = plt.subplots(dpi = 600, figsize = (12, 2.5), ncols = len(traj), sharey  = True)
+for ax, images in zip(axes, traj):
+    profile = sf.get_profile(images)
+    x = np.arange(0, len(images))
+    x_fit = np.linspace(0, len(images), 100)
+    y_fit = pchip_interpolate(x, profile, x_fit)
+    ax.plot(x, profile, 'o', label = 'calculated')
+    ax.plot(x_fit, y_fit, zorder = 1, label = 'pchip fit', color = 'darkred')
+    ax.set_xlabel('Reaction coordinate')
+    ax.set_xlim(x.min(), x.max())
+    ax.legend(frameon = False)
+axes[0].set_ylabel('Energy, eV')
+plt.tight_layout()
 ```
 
-    Activation barrier of 1D percolation: 3.29 eV
-    Activation barrier of 2D percolation: 3.56 eV
-    Activation barrier of 3D percolation: 3.56 eV
+    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.26 eV
+    Unique jump #1: Fmax 0.05 eV/angstrom | Activation barrier 3.56 eV
+    Unique jump #2: Fmax 0.09 eV/angstrom | Activation barrier 0.33 eV
+    Unique jump #3: Fmax 0.05 eV/angstrom | Activation barrier 3.3 eV
+    1D percolations barrier: 0.331
+    2D percolations barrier: 3.258
+    3D percolations barrier: 3.313
+
+
+
+    
+![png](example_files/example_15_1.png)
+    
 
 
 #### Compare with BVSE meshgrid approach (i.e. empty lattice)
 
 
 ```python
 from bvlain import Lain
@@ -384,7 +406,17 @@
     Bond valence sum for Fe is 1.8394
     Bond valence sum for Fe is 1.8394
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
 
+
+
+```python
+!jupyter nbconvert --to markdown example.ipynb
+```
+
+    [NbConvertApp] Converting notebook example.ipynb to markdown
+    [NbConvertApp] Support files will be in example_files/
+    [NbConvertApp] Writing 10819 bytes to example.md
+
```

### Comparing `ions-0.3.0/ions/calculators.py` & `ions-0.3.1/ions/calculators.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,17 @@
         self.nl.update(self.atoms)
 
         energies = np.zeros(natoms)
         forces = np.zeros((natoms, 3))
         positions = self.atoms.positions
         cell = self.atoms.cell
         neighbors, offsets = self.nl.get_neighbors(self.site)
-        cells = np.dot(offsets, cell)
-        r = self.atoms.positions[self.site] - (atoms.positions[neighbors] + np.dot(atoms.cell.T, offsets.T).T)
+        #cells = np.dot(offsets, cell)
+        #r = self.atoms.positions[self.site] - (atoms.positions[neighbors] + np.dot(atoms.cell.T, offsets.T).T)
+        r = self.atoms.positions[self.site] - (atoms.positions[neighbors] + np.dot(offsets, atoms.cell))
         r2 = np.linalg.norm(r, axis = 1)
 
         q1 = self.atoms.get_array('oxi_states')[self.site]
         s1 = self.atoms.symbols[self.site]
         z1 = self.atoms.numbers[self.site]
         n1 = principle_number[z1]
         rc1 = covalent_radii[z1]
```

### Comparing `ions-0.3.0/ions/data/Li2O_mp-1960.cif` & `ions-0.3.1/ions/data/Li2O_mp-1960.cif`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvparam_1991.yaml` & `ions-0.3.1/ions/data/bvparam_1991.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvparams2020-average.json` & `ions-0.3.1/ions/data/bvparams2020-average.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvparams2020-average.pickle` & `ions-0.3.1/ions/data/bvparams2020-average.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvparams_averaged2020.csv` & `ions-0.3.1/ions/data/bvparams_averaged2020.csv`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvparm2020.cif` & `ions-0.3.1/ions/data/bvparm2020.cif`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvparm2020_edit.txt` & `ions-0.3.1/ions/data/bvparm2020_edit.txt`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvse_data.json` & `ions-0.3.1/ions/data/bvse_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/bvse_data.pickle` & `ions-0.3.1/ions/data/bvse_data.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/elneg_data.json` & `ions-0.3.1/ions/data/elneg_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/icsd_bv.yaml` & `ions-0.3.1/ions/data/icsd_bv.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/quantum_n.pkl` & `ions-0.3.1/ions/data/quantum_n.pkl`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/shannon-data-crystal.json` & `ions-0.3.1/ions/data/shannon-data-crystal.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/shannon-data-crystal.pickle` & `ions-0.3.1/ions/data/shannon-data-crystal.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/shannon-data-ionic.json` & `ions-0.3.1/ions/data/shannon-data-ionic.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/shannon-data-ionic.pickle` & `ions-0.3.1/ions/data/shannon-data-ionic.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/shannon-radii.json` & `ions-0.3.1/ions/data/shannon-radii.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data/shannon-radii.pickle` & `ions-0.3.1/ions/data/shannon-radii.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/data.py` & `ions-0.3.1/ions/data.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/decorator.py` & `ions-0.3.1/ions/decorator.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/potential.py` & `ions-0.3.1/ions/potential.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.0/ions/tools/path_finder.py` & `ions-0.3.1/ions/tools/path_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,23 +130,24 @@
             [2, 0, 0],
             [0, 2, 0],
             [0, 0, 2]
         ]
         #print('collecting nn')
         supercell = make_supercell(mobile_atoms.copy(), scale) 
         supercell.pbc = False # we are interested in the percolation within the supercell -< it was a mistsake-< check it twice
-        shifts = np.where((supercell.get_scaled_positions() * 2.0).round(4) >= 1.0, 1, 0)
+        shifts = np.where((supercell.get_scaled_positions() * 2.0).round(4) >= 1.0, 1, 0) # check this line!
         supercell.set_array('shift', shifts)
         self.mobile_supercell = supercell
         i, j, d = neighbor_list('ijd', supercell, self.upper_bound)
         ij = np.array(list(zip(i, j)))
         if len(ij) == 0:
             raise
-        ij.sort(axis = 1) # (source, target)  == (target, source)
-        pairs, idx = np.unique(ij, axis = 0, return_index=True) # remove duplicates
+        ij.sort(axis = 1) # (source, target)  == (target, source) <-probably, was a bad idea
+        print('check')
+        pairs, idx = np.unique(ij, axis = 0, return_index=True) # remove duplicates, check this line!
         offsets = np.squeeze(np.diff(supercell.get_array('shift')[pairs], axis = 1))
         self.pairs = pairs
         self.offsets = offsets
         unwrapped_edges = np.hstack([pairs, offsets])
         #wrapped_edges = np.hstack([pairs - n_vertices * (pairs // n_vertices), offsets])
 
         wrapped_pairs = np.take(self.mobile_atoms.get_array('unitcell_idx'), pairs - n_vertices * (pairs // n_vertices))
@@ -161,18 +162,16 @@
         
         u, w, jump_distances = self._collect_edges_within_supercell()
         unique_edges, ue_idx, inverse = np.unique(w, axis = 0, return_index = True, return_inverse = True)
         #unitcell_idx = self.mobile_atoms.get_array('unitcell_idx')
         distances = []
         for edge  in w[ue_idx]:
             offset = edge[2:]
-            #source = unitcell_idx[int(edge[0])]
             source = edge[0]
             target = edge[1]
-            #target = unitcell_idx[int(edge[1])]
             shift = np.where(offset < 0, 1, 0)
             p1 = self.atoms.positions[source] + np.dot(shift, self.atoms.cell)
             p2 = self.atoms.positions[target] + np.dot(offset + shift, self.atoms.cell)
             base = self.atoms[[i for i in range(len(self.atoms)) if i not in [source, target]]]
             translations = np.array(list(itertools.product(
                                             [0, 1, -1], # should be [0, 1, -1, 2, -2] ideally
                                             [0, 1, -1],
@@ -189,14 +188,15 @@
             if self.oxi_states:
                 d_min = dd.min() - max(base.get_array('r_i')[ii[dd == dd.min()]])
             distances.append(d_min)
         self.distances = np.take(distances, inverse)
         self.jump_distances = jump_distances
         self.u = u
         self.w = w
+        return u, w, self.distances, self.jump_distances
 
 
     def _filter_edges(self, tr = 0.75, cutoff = 100.0):
 
         accept = []
         for i, (u, jump, dist) in enumerate(zip(self.u, self.jump_distances, self.distances)):
             if (jump > cutoff) or (dist < tr):
@@ -477,14 +477,15 @@
         else:
             print('Unexpected behavior')
             raise
         
         return abs(tr2 - tr), tr2, tr
 
 
+
     def interpolate(self, atoms, source, target, offset, min_sep_dist = 10.0, spacing = 0.5, n_max = 9):
         
         """
         Linearly interpolates trajectory between source and target ions. 
         Uses min_sep_dist to create supercell. 
 
         Parameters
```

### Comparing `ions-0.3.0/ions/utils.py` & `ions-0.3.1/ions/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,8 +122,23 @@
     z = X[:, 2]
     x0 = center.copy().positions[source]
     def dist_func(x0):
         return sum(((np.full(len(x),x0[0])-x)**2+(np.full(len(x),x0[1])-y)**2+(np.full(len(x),x0[2])-z)**2)**(1/2))
     
     bounds = ((x0[0] - 0.25, x0[0] + 0.25),(x0[1] - 0.25, x0[1] + 0.25), (x0[2] - 0.25, x0[2] + 0.25))
     res = minimize(dist_func, x0, method='nelder-mead', options={'disp': False}, bounds=bounds)
-    return res.x, x0
+    return res.x, x0
+
+def lineseg_dists(p, a, b):
+    
+    # source:    https://stackoverflow.com/questions/54442057/
+    # calculate-the-euclidian-distance-between-an-array-of-points-to-a-line-segment-in/
+    # 54442561#54442561 
+    
+    if np.all(a == b):
+        return np.linalg.norm(p - a, axis=1)
+    d = np.divide(b - a, np.linalg.norm(b - a))
+    s = np.dot(a - p, d)
+    t = np.dot(p - b, d)
+    h = np.maximum.reduce([s, t, np.zeros(len(p))])
+    c = np.cross(p - a, d)
+    return np.hypot(h, np.linalg.norm(c, axis = 1))
```

### Comparing `ions-0.3.0/ions.egg-info/PKG-INFO` & `ions-0.3.1/ions.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.3.0
+Version: 0.3.1
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
@@ -49,113 +49,100 @@
 ```pip install ions```
 
 #### Maximum percolation dimensionality and minimum required jump distance
 
 
 ```python
 from ase.io import read, write
-from ions.tools import PathFinder
+from ions.tools import Percolator
 
 file = '/Users/artemdembitskiy/Downloads/LiFePO4.cif'
 atoms = read(file)  
 
 specie = 3
-pf = PathFinder(atoms, specie, 10.0)
+pr = Percolator(atoms, specie, 10.0)
 
 tr = 0.5 # Minimum allowed distance between the edge and the framework
-cutoff, max_dim = pf.mincut_maxdim(tr)
+cutoff, dim = pr.mincut_maxdim(tr)
 
-print(f'Maximum percolation dimensionality: {max_dim}')
+print(f'Maximum percolation dimensionality: {dim}')
 print(f'Jump distance cutoff: {cutoff} angstrom')
 ```
 
     Maximum percolation dimensionality: 3
     Jump distance cutoff: 5.7421875 angstrom
 
 
 
 ```python
-pf.percolation_threshold(1), pf.percolation_threshold(2), pf.percolation_threshold(3)
+pr.percolation_threshold(1), pr.percolation_threshold(2), pr.percolation_threshold(3)
 ```
 
 
 
 
     (1.582, 1.4551, 0.9668)
 
 
 
-#### Save percolating network
-
-
-```python
-traj = pf.create_percotraj(cutoff, tr)
-write('perolating_sublattice.cif', traj) # jumps between nearest neighbors are linearly interpolated within 2x2x2 supercell
-```
-
 #### Inequivalent ionic hops forming percolating netwrok
 
 
 ```python
-edges, features = pf.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
-edges, features
+edges, features = pr.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
+edges
 ```
 
 
 
 
-    (array([[2, 3, 0, 0, 0],
-            [0, 1, 1, 0, 0],
-            [0, 3, 1, 0, 0],
-            [0, 3, 1, 1, 0],
-            [2, 1, 0, 1, 0],
-            [0, 0, 1, 0, 0]]),
-     array([[0.   , 0.   , 0.589, 5.736],
-            [0.   , 0.   , 0.66 , 5.736],
-            [0.   , 0.   , 0.695, 5.639],
-            [0.   , 0.   , 0.696, 5.639],
-            [0.   , 0.   , 1.461, 3.045],
-            [0.   , 0.   , 1.587, 4.746]]))
+    [Edge(0,1,[0 0 0], d=5.74, wrapped_target=1'),
+     Edge(0,3,[1 0 0], d=5.64, wrapped_target=3'),
+     Edge(0,3,[0 0 0], d=3.05, wrapped_target=3'),
+     Edge(0,0,[1 0 0], d=4.75, wrapped_target=0')]
 
 
 
 #### Find saddle point for each ionic hop using bond valence force field potential
 
 
 ```python
 import numpy as np
 from ase.io import read, write
 from ase.optimize import FIRE
 
 from ions.tools import SaddleFinder
 from ions.decorator import Decorator
+from ions.utils import collect_bvse_params
 
 
 Decorator().decorate(atoms) # oxidation states are required for this method
+collect_bvse_params(atoms, 'Li', +1, self_interaction=True) # do not omit Li-Li interaction
+pr = Percolator(atoms, specie, 10.0)
+edges, _ = pr.unique_edges(cutoff, tr)
 
-sf = SaddleFinder(self_interaction=True) # do not omit Li-Li interaction
 traj = []
 for i, edge in enumerate(edges):
-    source, target = edge[:2]
-    offset = edge[2:]
-    images, atoms_mod, offset = sf.interpolate(atoms, source, target, offset, min_sep_dist = 6.0, spacing = .75, abc = True)
+    superedge = edge.superedge(10.0, center = True) # put centroid of the edge in the center of the box
+    images = superedge.interpolate(spacing = 0.75)
+    sf = SaddleFinder()
+    neb = sf.bvse_neb(images)
+    optim = FIRE(neb,
+                    logfile = 'log'
+                    )
     traj.append(images)
-    neb = sf.bvse_neb(images, k = 2.0, gm = True) # Note that images are linked to the neb object and will be changed after optimization
-    optimizer = FIRE(neb, logfile = 'log')
-    optimizer.run(fmax =.1, steps = 100)
+    optim.run(fmax = 0.1, steps = 100)
     print(f'Unique jump #{i}: Fmax {neb.get_forces().max().round(2)} eV/angstrom |',
          f'Activation barrier {sf.get_barrier(images).round(2)} eV')
 ```
 
-    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.15 eV
-    Unique jump #1: Fmax 1.0 eV/angstrom | Activation barrier 4.14 eV
-    Unique jump #2: Fmax 0.08 eV/angstrom | Activation barrier 3.45 eV
-    Unique jump #3: Fmax 0.42 eV/angstrom | Activation barrier 4.89 eV
-    Unique jump #4: Fmax 0.09 eV/angstrom | Activation barrier 0.38 eV
-    Unique jump #5: Fmax 0.06 eV/angstrom | Activation barrier 3.28 eV
+    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.26 eV
+    Unique jump #1: Fmax 0.05 eV/angstrom | Activation barrier 3.56 eV
+    Unique jump #2: Fmax 0.09 eV/angstrom | Activation barrier 0.33 eV
+    Unique jump #3: Fmax 0.05 eV/angstrom | Activation barrier 3.3 eV
 
 
 #### Plot profile
 
 
 ```python
 import matplotlib.pyplot as plt
@@ -179,81 +166,116 @@
     ax.legend(frameon = False)
 axes[0].set_ylabel('Energy, eV')
 plt.tight_layout()
 ```
 
 
     
-![png](example_files/example_13_0.png)
+![png](example_files/example_11_0.png)
     
 
 
 #### Percolation dimensionality study (I found some inconsistency, don't use until update)
 
 
 ```python
 emins = []
 emaxs = []
 for images in traj:
+    
     emins.append(sf.get_profile(images).min())
     emaxs.append(sf.get_profile(images).max())
 
-for i, dim in enumerate(np.arange(1, max_dim + 1)):
-    e_a, tr_min, tr_max = pf.propagate_barriers(cutoff, tr, emins, emaxs, dim)
-    print(f'Activation barrier of {i + 1}D percolation: {round(e_a, 2)} eV')
+for d in range(1, dim + 1):
+   ea, tr_min, tr_max = pr.propagate_barriers(cutoff, tr, emins, emaxs, d)
+   print(f'{d}D percolations barrier: {round(ea, 3)}')
+
 ```
 
-    Activation barrier of 1D percolation: 3.28 eV
-    Activation barrier of 2D percolation: 3.45 eV
-    Activation barrier of 3D percolation: 3.45 eV
+    1D percolations barrier: 0.331
+    2D percolations barrier: 3.258
+    3D percolations barrier: 3.313
 
 
 #### Put all together
 
 
 ```python
+import numpy as np
 from ase.io import read, write
-from ions.tools import PathFinder, SaddleFinder
+from ase.optimize import FIRE
+from ions.tools import SaddleFinder
+from ions.decorator import Decorator
+from ions.utils import collect_bvse_params
+import matplotlib.pyplot as plt
+from scipy.interpolate import pchip_interpolate
 
-file = '/Users/artemdembitskiy/Downloads/LiFePO4.cif'
-atoms = read(file)  
-Decorator().decorate(atoms) # oxidation states are required for this method
+plt.rcParams.update({'font.size': 8})
+plt.rcParams.update({'font.family': 'Arial'})
 
-specie = 3
-pf = PathFinder(atoms, specie, 10.0)
 
-tr = 0.5 # Minimum allowed distance between the edge and the framework
-cutoff, max_dim = pf.mincut_maxdim(tr)
-edges, features = pf.unique_edges(cutoff, tr) # list of (source, target, offset_x, offset_y, offset_z)
 
-sf = SaddleFinder(self_interaction=True) # do not omit Li-Li interaction
+Decorator().decorate(atoms) # oxidation states are required for this method
+collect_bvse_params(atoms, 'Li', +1, self_interaction=True) # do not omit Li-Li interaction
+pr = Percolator(atoms, specie, 10.0)
+edges, _ = pr.unique_edges(cutoff, tr)
+
 traj = []
 emins = []
 emaxs = []
-for edge in edges:
-    source, target = edge[:2]
-    offset = edge[2:]
-    images, atoms_mod, offset = sf.interpolate(atoms, source, target, offset, min_sep_dist = 10.0, spacing = 0.5)
+for i, edge in enumerate(edges):
+    superedge = edge.superedge(10.0, center = True) # put centroid of the edge in the center of the box
+    images = superedge.interpolate(spacing = 0.75)
+    sf = SaddleFinder()
+    neb = sf.bvse_neb(images)
+    optim = FIRE(neb,
+                    logfile = 'log'
+                    )
+    
+    optim.run(fmax = 0.1, steps = 100)
+    print(f'Unique jump #{i}: Fmax {neb.get_forces().max().round(2)} eV/angstrom |',
+         f'Activation barrier {sf.get_barrier(images).round(2)} eV')
     traj.append(images)
-    neb = sf.bvse_neb(images, k = 5.0, gm = True) # Note that images are linked to the neb object and will be changed after optimization
-    optimizer = FIRE(neb, logfile = 'log')
-    optimizer.run(fmax =.1, steps = 100)
     emins.append(sf.get_profile(images).min())
     emaxs.append(sf.get_profile(images).max())
 
+for d in range(1, dim + 1):
+   ea, tr_min, tr_max = pr.propagate_barriers(cutoff, tr, emins, emaxs, d)
+   print(f'{d}D percolations barrier: {round(ea, 3)}')
 
-for dim in np.arange(1, max_dim + 1):
-    e_a, tr_min, tr_max = pf.propagate_barriers(cutoff, tr, emins, emaxs, dim)
-    print(f'Activation barrier of {dim}D percolation: {round(e_a, 2)} eV')
 
+
+fig, axes = plt.subplots(dpi = 600, figsize = (12, 2.5), ncols = len(traj), sharey  = True)
+for ax, images in zip(axes, traj):
+    profile = sf.get_profile(images)
+    x = np.arange(0, len(images))
+    x_fit = np.linspace(0, len(images), 100)
+    y_fit = pchip_interpolate(x, profile, x_fit)
+    ax.plot(x, profile, 'o', label = 'calculated')
+    ax.plot(x_fit, y_fit, zorder = 1, label = 'pchip fit', color = 'darkred')
+    ax.set_xlabel('Reaction coordinate')
+    ax.set_xlim(x.min(), x.max())
+    ax.legend(frameon = False)
+axes[0].set_ylabel('Energy, eV')
+plt.tight_layout()
 ```
 
-    Activation barrier of 1D percolation: 3.29 eV
-    Activation barrier of 2D percolation: 3.56 eV
-    Activation barrier of 3D percolation: 3.56 eV
+    Unique jump #0: Fmax 0.07 eV/angstrom | Activation barrier 3.26 eV
+    Unique jump #1: Fmax 0.05 eV/angstrom | Activation barrier 3.56 eV
+    Unique jump #2: Fmax 0.09 eV/angstrom | Activation barrier 0.33 eV
+    Unique jump #3: Fmax 0.05 eV/angstrom | Activation barrier 3.3 eV
+    1D percolations barrier: 0.331
+    2D percolations barrier: 3.258
+    3D percolations barrier: 3.313
+
+
+
+    
+![png](example_files/example_15_1.png)
+    
 
 
 #### Compare with BVSE meshgrid approach (i.e. empty lattice)
 
 
 ```python
 from bvlain import Lain
@@ -406,7 +428,17 @@
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
     Bond valence sum for P is 4.6745
 
 
 
+```python
+!jupyter nbconvert --to markdown example.ipynb
+```
+
+    [NbConvertApp] Converting notebook example.ipynb to markdown
+    [NbConvertApp] Support files will be in example_files/
+    [NbConvertApp] Writing 10819 bytes to example.md
+
+
+
```

### Comparing `ions-0.3.0/ions.egg-info/SOURCES.txt` & `ions-0.3.1/ions.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -30,11 +30,13 @@
 ions/data/shannon-data-crystal.pickle
 ions/data/shannon-data-ionic.json
 ions/data/shannon-data-ionic.pickle
 ions/data/shannon-radii.json
 ions/data/shannon-radii.pickle
 ions/featurizers/__init__.py
 ions/geom/__init__.py
+ions/geom/box.py
 ions/geom/edge.py
 ions/tools/__init__.py
 ions/tools/path_finder.py
+ions/tools/percolator.py
 ions/tools/saddle_finder.py
```

### Comparing `ions-0.3.0/setup.py` & `ions-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='ions',  
-     version='0.3.0',
+     version='0.3.1',
      py_modules = ["ions"],
      install_requires = [
                          "ase>=3.22.1",
                          "numpy",
 			             "spglib",
                          "networkx",
                          "scipy",
```

