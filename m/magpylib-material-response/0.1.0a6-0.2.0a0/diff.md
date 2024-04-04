# Comparing `tmp/magpylib-material-response-0.1.0a6.tar.gz` & `tmp/magpylib-material-response-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/magpylib-material-response-0.1.0a6.tar", last modified: Tue Nov 14 14:44:39 2023, max compression
+gzip compressed data, was "magpylib-material-response-0.2.0a0.tar", last modified: Thu Apr  4 11:31:55 2024, max compression
```

## Comparing `magpylib-material-response-0.1.0a6.tar` & `magpylib-material-response-0.2.0a0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:44:39.000000 magpylib-material-response-0.1.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-11-14 14:44:39.000000 magpylib-material-response-0.1.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:44:39.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:44:39.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/data/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/demag.py
--rw-r--r--   0 runner    (1001) docker     (127)    15995 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/meshing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/meshing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/polyline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/magpylib_material_response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 14:44:39.000000 magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-11-14 14:44:38.000000 magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-11-14 14:44:39.000000 magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 14:44:38.000000 magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-14 14:44:38.000000 magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-14 14:44:38.000000 magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 14:44:39.000000 magpylib-material-response-0.1.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-11-14 14:44:36.000000 magpylib-material-response-0.1.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.752461 magpylib-material-response-0.2.0a0/magpylib_material_response/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/magpylib_material_response/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/demag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/meshing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/magpylib_material_response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 11:31:55.000000 magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:31:55.756461 magpylib-material-response-0.2.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-04 11:31:53.000000 magpylib-material-response-0.2.0a0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `magpylib-material-response-0.1.0a6/PKG-INFO` & `magpylib-material-response-0.2.0a0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 Metadata-Version: 2.1
 Name: magpylib-material-response
-Version: 0.1.0a6
+Version: 0.2.0a0
 Summary: An extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets.
 Home-page: https://github.com/magpylib/magpylib-material-response
 Author: Alexandre Boisselet
 Author-email: magpylib@gmail.com
 License: MIT
-Description: # magpylib-material-response
-        
-        [![Code style: black][black-badge]][black-link]
-        
-        > **Warning**
-        > **This package is experimental and in a very dynamic development phase. Breaking API changes may happen at any time.**
-        
-        Magpylib-Material-Response is an extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets. Leveraging the Method of Moments, it calculates magnetic material response by meshing sources in an arbitrary number of unit elements.
-        
-        ## Installation
-        
-        Install from PyPi
-        
-        ```console
-        $ pip install magpylib-material-response
-        ```
-        
-        or locally:
-        
-        ```
-        $ pip install -e .[code_style,testing]
-        ```
-        
-        ## Testing
-        
-        Enter created folder then run tests:
-        
-        ```
-        $ flake8 .
-        $ black .
-        $ pytest
-        ```
-        
-        To use pre-commit:
-        
-        ```
-        $ git add *
-        # to apply to staged files
-        $ pre-commit run
-        # restage if changes
-        $ git add *
-        # to run on commits
-        $ pre-commit install
-        $ git commit -m 'Initial commit'
-        ```
-        
-        [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-        [black-link]: https://github.com/ambv/black
-        
-        (package originally created by [python-pkg-cookiecutter](https://github.com/executablebooks/python-pkg-cookiecutter))
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: code_style
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+# magpylib-material-response
+
+[![Code style: black][black-badge]][black-link]
+
+> **Warning**
+> **This package is experimental and in a very dynamic development phase. Breaking API changes may happen at any time.**
+
+Magpylib-Material-Response is an extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets. Leveraging the Method of Moments, it calculates magnetic material response by meshing sources in an arbitrary number of unit elements.
+
+## Installation
+
+Install from PyPi
+
+```console
+$ pip install magpylib-material-response
+```
+
+or locally:
+
+```
+$ pip install -e .[code_style,testing]
+```
+
+## Testing
+
+Enter created folder then run tests:
+
+```
+$ flake8 .
+$ black .
+$ pytest
+```
+
+To use pre-commit:
+
+```
+$ git add *
+# to apply to staged files
+$ pre-commit run
+# restage if changes
+$ git add *
+# to run on commits
+$ pre-commit install
+$ git commit -m 'Initial commit'
+```
+
+[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black-link]: https://github.com/ambv/black
+
+(package originally created by [python-pkg-cookiecutter](https://github.com/executablebooks/python-pkg-cookiecutter))
+
+
```

### Comparing `magpylib-material-response-0.1.0a6/README.md` & `magpylib-material-response-0.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a6/magpylib_material_response/demag.py` & `magpylib-material-response-0.2.0a0/magpylib_material_response/demag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """demag_functions"""
+
 # +
 # pylint: disable=invalid-name, redefined-outer-name, protected-access
 import sys
 from collections import Counter
 
 import magpylib as magpy
 import numpy as np
 from loguru import logger
-from magpylib._src.obj_classes.class_BaseExcitations import BaseCurrent
-from magpylib._src.obj_classes.class_BaseExcitations import BaseMagnet
+from magpylib._src.obj_classes.class_BaseExcitations import BaseCurrent, BaseMagnet
 from magpylib.magnet import Cuboid
 from scipy.spatial.transform import Rotation as R
 
 from magpylib_material_response.utils import timelog
 
 config = {
     "handlers": [
@@ -27,31 +27,29 @@
             ),
         ),
     ],
 }
 logger.configure(**config)
 
 
-def get_xis(*sources, xi=None):
-    """Return a list of length (len(sources)) with xi values
+def get_susceptibilities(*sources, susceptibility=None):
+    """Return a list of length (len(sources)) with susceptibility values
     Priority is given at the source level, hovever if value is not found, it is searched
     up the parent tree, if available. Raises an error if no value is found when reached
     the top level of the tree."""
-    xis = []
+    susceptibilities = []
     for src in sources:
-        xi = getattr(src, "xi", None)
-        if xi is None:
+        susceptibility = getattr(src, "susceptibility", None)
+        if susceptibility is None:
             if src.parent is None:
-                raise ValueError(
-                    "No susceptibility `xi` defined in any parent collection"
-                )
-            xis.extend(get_xis(src.parent))
+                raise ValueError("No susceptibility defined in any parent collection")
+            susceptibilities.extend(get_susceptibilities(src.parent))
         else:
-            xis.append(xi)
-    return xis
+            susceptibilities.append(susceptibility)
+    return susceptibilities
 
 
 def demag_tensor(
     src_list,
     pairs_matching=False,
     split=False,
     max_dist=0,
@@ -101,52 +99,52 @@
         getH_params, mask_inds, unique_inv_inds, pos0, rot0 = match_pairs(src_list)
     else:
         pos0 = np.array([getattr(src, "barycenter", src.position) for src in src_list])
         rotQ0 = [src.orientation.as_quat() for src in src_list]
         rot0 = R.from_quat(rotQ0)
 
     H_point = []
-    for unit_mag in [(1, 0, 0), (0, 1, 0), (0, 0, 1)]:
-        mag_all = rot0.inv().apply(unit_mag)
+    for unit_pol in [(1, 0, 0), (0, 1, 0), (0, 0, 1)]:
+        pol_all = rot0.inv().apply(unit_pol)
         # point matching field and demag tensor
-        with timelog(f"getH with unit_mag={unit_mag}", min_log_time=min_log_time):
+        with timelog(f"getH with unit_pol={unit_pol}", min_log_time=min_log_time):
             if pairs_matching or max_dist != 0:
-                magnetization = np.repeat(mag_all, len(src_list), axis=0)[mask_inds]
+                polarization = np.repeat(pol_all, len(src_list), axis=0)[mask_inds]
                 H_unique = magpy.getH(
-                    "Cuboid", magnetization=magnetization, **getH_params
+                    "Cuboid", polarization=polarization, **getH_params
                 )
                 if max_dist != 0:
                     H_temp = np.zeros((len(src_list) ** 2, 3))
                     H_temp[mask_inds] = H_unique
-                    H_unit_mag = H_temp
+                    H_unit_pol = H_temp
                 else:
-                    H_unit_mag = H_unique[unique_inv_inds]
+                    H_unit_pol = H_unique[unique_inv_inds]
             else:
-                for src, mag in zip(src_list, mag_all):
-                    src.magnetization = mag
+                for src, pol in zip(src_list, pol_all):
+                    src.polarization = pol
                 if split > 1:
                     src_list_split = np.array_split(src_list, split)
                     with logger.contextualize(
                         task="Splitting field calculation", split=split
                     ):
-                        H_unit_mag = []
+                        H_unit_pol = []
                         for split_ind, src_list_subset in enumerate(src_list_split):
                             logger.info(
                                 f"Sources subset {split_ind+1}/{len(src_list_split)}"
                             )
                             if src_list_subset.size > 0:
-                                H_unit_mag.append(
+                                H_unit_pol.append(
                                     magpy.getH(src_list_subset.tolist(), pos0)
                                 )
-                        H_unit_mag = np.concatenate(H_unit_mag, axis=0)
+                        H_unit_pol = np.concatenate(H_unit_pol, axis=0)
                 else:
-                    H_unit_mag = magpy.getH(src_list, pos0)
-            H_point.append(H_unit_mag)  # shape (n_cells, n_pos, 3_xyz)
+                    H_unit_pol = magpy.getH(src_list, pos0)
+            H_point.append(H_unit_pol)  # shape (n_cells, n_pos, 3_xyz)
 
-    # shape (3_unit_mag, n_cells, n_pos, 3_xyz)
+    # shape (3_unit_pol, n_cells, n_pos, 3_xyz)
     T = np.array(H_point).reshape((3, nof_src, nof_src, 3))
 
     return T
 
 
 def filter_distance(
     src_list,
@@ -241,32 +239,32 @@
             dimension=np.repeat(dim0, len(src_list), axis=0)[unique_inds],
         )
     return params, unique_inds, unique_inv_inds, pos0, rot0
 
 
 def apply_demag(
     collection,
-    xi=None,
+    susceptibility=None,
     inplace=False,
     pairs_matching=False,
     max_dist=0,
     split=1,
     min_log_time=1,
     style=None,
 ):
     """
     Computes the interaction between all collection magnets and fixes their
-    magnetization.
+    polarization.
 
     Parameters
     ----------
     collection: magpylib.Collection object with n magnet sources
         Each magnet source in collection is treated as a magnetic cell.
 
-    xi: array_like, shape (n,)
+    susceptibility: array_like, shape (n,)
         Vector of n magnetic susceptibilities of the cells. If not defined, values are
         searched at object level or parent level if needed.
 
     inplace: bool
         If False, applies demagnetization on a copy of the input collection and returns
         the demagnetized collection
 
@@ -328,62 +326,62 @@
     coll_str = str(collection) if not lbl else lbl
     demag_msg = (
         f"Demagnetization{inplace_str} of <blue>{coll_str}</blue>"
         f" with {n} cells - {counts}"
     )
     with timelog(demag_msg, min_log_time=min_log_time):
         # set up mr
-        mag_magnets = [
-            src.orientation.apply(src.magnetization) for src in magnets_list
+        pol_magnets = [
+            src.orientation.apply(src.polarization) for src in magnets_list
         ]  # ROTATION CHECK
-        mag_magnets = np.reshape(
-            mag_magnets, (3 * n, 1), order="F"
+        pol_magnets = np.reshape(
+            pol_magnets, (3 * n, 1), order="F"
         )  # shape ii = x1, ... xn, y1, ... yn, z1, ... zn
 
         # set up S
-        if xi is None:
-            xi = get_xis(*magnets_list)
-        xi = np.array(xi)
-        if len(xi) != n:
+        if susceptibility is None:
+            susceptibility = get_susceptibilities(*magnets_list)
+        susceptibility = np.array(susceptibility)
+        if len(susceptibility) != n:
             raise ValueError(
-                "Apply_demag input collection and xi must have same length."
+                "Apply_demag input collection and susceptibility must have same length."
             )
-        S = np.diag(np.tile(xi, 3))  # shape ii, jj
+        S = np.diag(np.tile(susceptibility, 3))  # shape ii, jj
 
-        # set up T (3 mag unit, n cells, n positions, 3 Bxyz)
+        # set up T (3 pol unit, n cells, n positions, 3 Bxyz)
         with timelog("Demagnetization tensor calculation", min_log_time=min_log_time):
             T = demag_tensor(
                 magnets_list,
                 split=split,
                 pairs_matching=pairs_matching,
                 max_dist=max_dist,
             )
 
-            T *= 4 * np.pi / 10
+            T *= magpy.mu_0
             T = T.swapaxes(2, 3).reshape((3 * n, 3 * n)).T  # shape ii, jj
 
-        mag_tolal = mag_magnets
+        pol_tolal = pol_magnets
 
         if currents_list:
             with timelog(
                 "Add current sources contributions", min_log_time=min_log_time
             ):
                 pos = np.array([src.position for src in magnets_list])
-                mag_currents = magpy.getB(currents_list, pos, sumup=True)
-                mag_currents = np.reshape(mag_currents, (3 * n, 1), order="F")
-                mag_tolal += np.matmul(S, mag_currents)
+                pol_currents = magpy.getB(currents_list, pos, sumup=True)
+                pol_currents = np.reshape(pol_currents, (3 * n, 1), order="F")
+                pol_tolal += np.matmul(S, pol_currents)
 
         # set up Q
         Q = np.eye(3 * n) - np.matmul(S, T)
 
-        # determine new magnetization vectors
+        # determine new polarization vectors
         with timelog("Solving of linear system", min_log_time=1):
-            mag_new = np.linalg.solve(Q, mag_tolal)
+            pol_new = np.linalg.solve(Q, pol_tolal)
 
-        mag_new = np.reshape(mag_new, (n, 3), order="F")
-        # mag_new *= .4*np.pi
+        pol_new = np.reshape(pol_new, (n, 3), order="F")
+        # pol_new *= .4*np.pi
 
-        for s, mag in zip(collection.sources_all, mag_new):
-            s.magnetization = s.orientation.inv().apply(mag)  # ROTATION CHECK
+        for s, pol in zip(collection.sources_all, pol_new):
+            s.polarization = s.orientation.inv().apply(pol)  # ROTATION CHECK
 
     if not inplace:
         return collection
```

### Comparing `magpylib-material-response-0.1.0a6/magpylib_material_response/meshing.py` & `magpylib-material-response-0.2.0a0/magpylib_material_response/meshing.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 import magpylib as magpy
 import numpy as np
 from loguru import logger
 from magpylib._src.obj_classes.class_BaseExcitations import BaseCurrent
 from scipy.spatial.transform import Rotation as R
 
-from magpylib_material_response.meshing_utils import cells_from_dimension
-from magpylib_material_response.meshing_utils import get_volume
-from magpylib_material_response.meshing_utils import mask_inside
+from magpylib_material_response.meshing_utils import (
+    cells_from_dimension,
+    get_volume,
+    mask_inside,
+)
 
 
 def _collection_from_obj_and_cells(obj, cells, **style_kwargs):
-    xi = getattr(obj, "xi", None)
-    if xi is not None:
+    susceptibility = getattr(obj, "susceptibility", None)
+    if susceptibility is not None:
         for cell in cells:
-            cell.xi = xi
+            cell.susceptibility = susceptibility
     coll = magpy.Collection(cells)
     coll.style.update(obj.style.as_dict(), _match_properties=False)
     coll.style.update(coll._process_style_kwargs(**style_kwargs))
     coll.position = obj.position
     coll.orientation = obj.orientation
     return coll
 
@@ -49,15 +51,15 @@
     """
     if not isinstance(cuboid, magpy.magnet.Cuboid):
         raise TypeError(
             "Object to be meshed must be a Cuboid, "
             f"received instead {cuboid.__class__.__name__!r}"
         )
     dim0 = cuboid.dimension
-    mag0 = cuboid.magnetization
+    pol0 = cuboid.polarization
 
     if np.isscalar(target_elems):
         nnn = cells_from_dimension(dim0, target_elems)
     else:
         nnn = target_elems
     elems = np.prod(nnn)
     if verbose:
@@ -78,15 +80,15 @@
         for d, n in zip(dim0, nnn)
     )
     grid = np.array([(x, y, z) for x in xs for y in ys for z in zs])
 
     # create cells as magpylib objects and return Collection
     cells = []
     for pp in grid:
-        cell = magpy.magnet.Cuboid(magnetization=mag0, dimension=new_dim, position=pp)
+        cell = magpy.magnet.Cuboid(polarization=pol0, dimension=new_dim, position=pp)
         cells.append(cell)
 
     return _collection_from_obj_and_cells(cuboid, cells, **kwargs)
 
 
 def mesh_Cylinder(cylinder, target_elems, verbose=False, **kwargs):
     """
@@ -124,15 +126,15 @@
             360,
         )
     else:
         raise TypeError("Input must be a Cylinder or CylinderSegment")
 
     al = (r2 + r1) * 3.14 * (phi2 - phi1) / 360  # arclen = D*pi*arcratio
     dim = al, r2 - r1, h
-    mag0 = cylinder.magnetization
+    pol0 = cylinder.polarization
     # "unroll" the cylinder and distribute the target number of elemens along the
     # circumference, radius and height.
     if np.isscalar(target_elems):
         nphi, nr, nh = cells_from_dimension(dim, target_elems)
     else:
         nphi, nr, nh = target_elems
     elems = np.prod([nphi, nr, nh])
@@ -151,30 +153,30 @@
         for h_ind in range(nh):
             pos_h = dh * h_ind - h / 2 + dh / 2
             # use a cylinder for the innermost cells if there are at least 3 layers and
             # if it is closed, use cylinder segments otherwise
             if nr >= 3 and r[r_ind] == 0 and phi2 - phi1 == 360:
                 dimension = r[r_ind + 1] * 2, dh
                 cell = magpy.magnet.Cylinder(
-                    magnetization=mag0,
+                    polarization=pol0,
                     dimension=dimension,
                     position=(0, 0, pos_h),
                 )
                 cells.append(cell)
             else:
                 for phi_ind in range(nphi_r):
                     dimension = (
                         r[r_ind],
                         r[r_ind + 1],
                         dh,
                         phi[phi_ind],
                         phi[phi_ind + 1],
                     )
                     cell = magpy.magnet.CylinderSegment(
-                        magnetization=mag0,
+                        polarization=pol0,
                         dimension=dimension,
                         position=(0, 0, pos_h),
                     )
                     cells.append(cell)
     return _collection_from_obj_and_cells(cylinder, cells, **kwargs)
 
 
@@ -204,15 +206,15 @@
     Returns
     -------
     discretization: magpylib.Collection
         Collection of Cuboid cells
     """
 
     r1, r2, h, phi1, phi2 = cyl_seg.dimension
-    mag0 = cyl_seg.magnetization
+    pol0 = cyl_seg.polarization
     if ratio_limit > r2 / (r2 - r1):
         raise ValueError(
             "This meshing function is intended for thin-walled CylinderSegment objects"
             f" of radii-ratio r2/(r2-r1)>{ratio_limit}, r1 being the inner radius."
             f"\nInstead r2/(r2-r1)={r2 / (r2 - r1)}"
         )
     # distribute elements -> targeting thin close-to-square surface cells
@@ -234,15 +236,15 @@
     )
     poss = np.array([x0 * np.cos(phi_vec), x0 * np.sin(phi_vec), np.zeros(nphi)]).T
     rots = R.from_euler("z", phi_vec)
     cells = []
     for z in np.linspace(-h / 2 + dh / 2, h / 2 - dh / 2, nh):
         for pos, orient in zip(poss, rots):
             child = magpy.magnet.Cuboid(
-                magnetization=orient.inv().apply(mag0),
+                polarization=orient.inv().apply(pol0),
                 dimension=dim,
                 position=pos + np.array([0, 0, z]),
                 orientation=orient,
             )
             cells.append(child)
     return _collection_from_obj_and_cells(cyl_seg, cells, **kwargs)
 
@@ -278,27 +280,27 @@
         raise TypeError(
             "Object to be sliced must be a Cuboid, "
             f"received instead {cuboid.__class__.__name__!r}"
         )
     if not 0 < shift < 1:
         raise ValueError("Shift must be between 0 and 1 (exclusive)")
     dim0 = cuboid.dimension
-    mag0 = cuboid.magnetization
+    pol0 = cuboid.polarization
     ind = "xyz".index(axis)
     dim_k = cuboid.dimension[ind]
     dims_k = dim_k * (1 - shift), dim_k * (shift)
     shift_k = (dim_k - dims_k[0]) / 2, -(dim_k - dims_k[1]) / 2
     cells = []
     for d, s in zip(dims_k, shift_k):
         dimension = dim0.copy()
         dimension[ind] = d
         position = np.array([0, 0, 0], dtype=float)
         position[ind] = s
         cell = magpy.magnet.Cuboid(
-            magnetization=mag0,
+            polarization=pol0,
             dimension=dimension,
             position=position,
         )
         cells.append(cell)
     return _collection_from_obj_and_cells(cuboid, cells[::-1], **kwargs)
 
 
@@ -317,15 +319,15 @@
     strict inside: bool
         If True, also filters out the cells with vertices outside the object boundaries
 
     Returns
     -------
     discretization: magpylib.Collection
         Collection of Cylinder and CylinderSegment cells"""
-    mag0 = obj.magnetization
+    pol0 = obj.polarization
     vol, containing_cube_edge = get_volume(obj, return_containing_cube_edge=True)
     vol_ratio = (containing_cube_edge**3) / vol
 
     grid_elems = [int((vol_ratio * target_elems) ** (1 / 3))] * 3
     grid_dim = [containing_cube_edge] * 3
 
     slices = [slice(-d / 2, d / 2, N * 1j) for d, N in zip(grid_dim, grid_elems)]
@@ -344,15 +346,15 @@
         grid = grid[pos_inside_strict_mask]
         if grid.size == 0:
             raise ValueError("No cuboids left with strict-inside method")
 
     cells = []
     for pos in grid:
         cell = magpy.magnet.Cuboid(
-            magnetization=mag0,
+            polarization=pol0,
             dimension=cube_cell_dim,
             position=pos,
         )
         cells.append(cell)
     return _collection_from_obj_and_cells(obj, cells, **kwargs)
```

### Comparing `magpylib-material-response-0.1.0a6/magpylib_material_response/meshing_utils.py` & `magpylib-material-response-0.2.0a0/magpylib_material_response/meshing_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a6/magpylib_material_response/polyline.py` & `magpylib-material-response-0.2.0a0/magpylib_material_response/polyline.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     dot_babc = np.dot(ba_unit, bc_unit)
     if dot_babc == -1:  # angle is 180°
         return None
     theta = np.arccos(dot_babc) / 2
     tan_theta = np.tan(theta)
     d = r / tan_theta
     if d > norm_bc * max_ratio or d > norm_ab * max_ratio:
-        rold, dold = r, d
+        # rold, dold = r, d
         print("r, d, norm_ab, norm_bc: ", r, d, norm_ab, norm_bc)
         d = min(norm_bc * max_ratio, norm_ab * max_ratio)
         r = d * tan_theta if theta > 0 else 0
         # warnings.warn(f"Radius {rold:.4g} is too big and has been reduced to {r:.4g}")
     ta = b + ba_unit * d
     tb = b + bc_unit * d
 
@@ -141,16 +141,18 @@
             points[i],
             points[i + 1],
         )
         if closed and i == n - 2:
             c = filleted_points[1]
         try:
             filleted_points.extend(_create_fillet_segment(a, b, c, radius, N))
-        except ValueError:
-            raise ValueError(f"The radius {radius} on position vertex {i} is too large")
+        except ValueError as exc:
+            raise ValueError(
+                f"The radius {radius} on position vertex {i} is too large"
+            ) from exc
     if closed:
         filleted_points[0] = filleted_points[-1]
     else:
         filleted_points = np.append(filleted_points, points[-1:], axis=0)
     return np.array(filleted_points)
 
 
@@ -204,15 +206,15 @@
     Returns
     -------
     intersection_points : numpy.ndarray
         A 2D array of shape (N, 3) representing the intersection points of the lines and the plane.
     """
     # Calculate the plane equation coefficients A, B, C, and D
     A, B, C = plane_normal
-    x0, y0, z0 = plane_point
+    # x0, y0, z0 = plane_point
     D = -np.dot(plane_normal, plane_point)
 
     # Calculate the parameter t
     t = -(A * line_points[:, 0] + B * line_points[:, 1] + C * line_points[:, 2] + D) / (
         A * line_directions[:, 0]
         + B * line_directions[:, 1]
         + C * line_directions[:, 2]
```

### Comparing `magpylib-material-response-0.1.0a6/magpylib_material_response/utils.py` & `magpylib-material-response-0.2.0a0/magpylib_material_response/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 logger.opt(colors=True).info(f"Start {self.msg}")
                 self._msg_displayed = True
             # include a delay here so the thread doesn't uselessly thrash the CPU
             time.sleep(max(0.01, self.min_log_time / 5))
 
 
 @contextmanager
-def timelog(msg, min_log_time=1) -> float:
+def timelog(msg, min_log_time=1):
     """ "Measure and log time with loguru as context manager."""
     start = time.perf_counter()
     end = None
     thread_timer = ElapsedTimeThread(msg=msg, min_log_time=min_log_time)
     thread_timer.start()
     try:
         yield
@@ -65,38 +65,46 @@
         )
 
 
 def serialize_recursive(obj, parent="warn"):
     dd = {
         "id": id(obj),
         "type": obj.__class__.__name__,
-        "position": {"value": obj.position.tolist(), "unit": "mm"},
+        "position": {"value": obj.position.tolist(), "unit": "m"},
         "orientation": {
             "value": obj.orientation.as_matrix().tolist(),
             "type": "matrix",
         },
     }
     if getattr(obj, "_style", None) is not None or obj._style_kwargs:
         dd["style"] = obj.style.as_dict()
     if parent == "warn" and obj.parent is not None:
         warnings.warn(f"object parent ({obj.parent}) not included in serialization")
     if isinstance(obj, BaseMagnet):
-        dd["magnetization"] = {"value": obj.magnetization.tolist(), "unit": "mT"}
-        xi = getattr(obj, "susceptibility", None)
-        xi = getattr(obj, "xi", None) if xi is None else xi
-        if xi is not None:
-            dd["susceptibility"] = {"value": xi}
+        dd["polarization"] = {"value": obj.polarization.tolist(), "unit": "T"}
+        susceptibility = getattr(obj, "susceptibility", None)
+        susceptibility = (
+            getattr(obj, "susceptibility", None)
+            if susceptibility is None
+            else susceptibility
+        )
+        if susceptibility is not None:
+            dd["susceptibility"] = {"value": susceptibility}
     if isinstance(obj, magpy.magnet.Cuboid):
-        dd["dimension"] = {"value": obj.dimension.tolist(), "unit": "mm"}
-        xi = getattr(obj, "susceptibility", None)
-        xi = getattr(obj, "xi", None) if xi is None else xi
-        if xi is not None:
-            dd["susceptibility"] = {"value": xi}
+        dd["dimension"] = {"value": obj.dimension.tolist(), "unit": "m"}
+        susceptibility = getattr(obj, "susceptibility", None)
+        susceptibility = (
+            getattr(obj, "susceptibility", None)
+            if susceptibility is None
+            else susceptibility
+        )
+        if susceptibility is not None:
+            dd["susceptibility"] = {"value": susceptibility}
     elif isinstance(obj, magpy.Sensor):
-        dd["pixel"] = {"value": obj.pixel.tolist(), "unit": "mm"}
+        dd["pixel"] = {"value": obj.pixel.tolist(), "unit": "m"}
     elif isinstance(obj, magpy.Collection):
         dd["children"] = [
             serialize_recursive(child, parent="ignore") for child in obj.children
         ]
     else:
         raise TypeError("Only Cuboid supported")
     return dd
@@ -115,16 +123,16 @@
         constr = magpy.Sensor
     elif getattr(magpy.magnet, typ, None) is not None:
         constr = getattr(magpy.magnet, typ)
     kw = {}
     # position
     kw["position"] = inp["position"]["value"]
     pos_unit = inp["position"]["unit"]
-    if pos_unit != "mm":
-        raise ValueError(f"Position unit must be `mm`, got {pos_unit!r}")
+    if pos_unit != "m":
+        raise ValueError(f"Position unit must be `m`, got {pos_unit!r}")
 
     # orientation
     orient = inp["orientation"]["value"]
     orient_typ = inp["orientation"]["type"]
     if orient_typ != "matrix":
         raise ValueError(f"Orientation type must be `matrix`, got {orient_typ!r}")
     kw["orientation"] = Rotation.from_matrix(orient)
@@ -133,36 +141,34 @@
     if style is not None:
         kw["style"] = style
 
     if inp.get("parent", None) is not None:
         warnings.warn(f"object parent ({inp['parent']}) ignored")
 
     if issubclass(constr, BaseMagnet):
-        # magnetization
-        kw["magnetization"] = inp["magnetization"]["value"]
-        mag_unit = inp["magnetization"]["unit"]
-        if mag_unit != "mT":
-            raise ValueError(f"Magnetization unit must be `mT`, got {mag_unit!r}")
+        kw["polarization"] = inp["polarization"]["value"]
+        pol_unit = inp["polarization"]["unit"]
+        if pol_unit != "T":
+            raise ValueError(f"Polarization unit must be `T`, got {pol_unit!r}")
     if issubclass(constr, magpy.magnet.Cuboid):
-        # dimension
         kw["dimension"] = inp["dimension"]["value"]
         dim_unit = inp["dimension"]["unit"]
-        if dim_unit != "mm":
-            raise ValueError(f"Dimension unit must be `mm`, got {dim_unit!r}")
+        if dim_unit != "m":
+            raise ValueError(f"Dimension unit must be `m`, got {dim_unit!r}")
     elif issubclass(constr, magpy.Sensor):
         kw["pixel"] = inp["pixel"]["value"]
         pix_unit = inp["pixel"]["unit"]
-        if pix_unit != "mm":
-            raise ValueError(f"Pixel unit must be `mm`, got {pix_unit!r}")
+        if pix_unit != "m":
+            raise ValueError(f"Pixel unit must be `m`, got {pix_unit!r}")
     elif not is_coll:
         raise TypeError("Only Collection, Cuboid, Sensor supported")
     obj = constr(**kw)
     ids[inp["id"]] = obj
     if inp.get("susceptibility", None) is not None:
-        obj.xi = inp["susceptibility"]["value"]
+        obj.susceptibility = inp["susceptibility"]["value"]
     if is_coll:
         obj.add(*[deserialize_recursive(child, ids)[0] for child in inp["children"]])
     return obj, ids
 
 
 def serialize_setup(*objs):
     res = []
```

### Comparing `magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/PKG-INFO` & `magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 Metadata-Version: 2.1
 Name: magpylib-material-response
-Version: 0.1.0a6
+Version: 0.2.0a0
 Summary: An extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets.
 Home-page: https://github.com/magpylib/magpylib-material-response
 Author: Alexandre Boisselet
 Author-email: magpylib@gmail.com
 License: MIT
-Description: # magpylib-material-response
-        
-        [![Code style: black][black-badge]][black-link]
-        
-        > **Warning**
-        > **This package is experimental and in a very dynamic development phase. Breaking API changes may happen at any time.**
-        
-        Magpylib-Material-Response is an extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets. Leveraging the Method of Moments, it calculates magnetic material response by meshing sources in an arbitrary number of unit elements.
-        
-        ## Installation
-        
-        Install from PyPi
-        
-        ```console
-        $ pip install magpylib-material-response
-        ```
-        
-        or locally:
-        
-        ```
-        $ pip install -e .[code_style,testing]
-        ```
-        
-        ## Testing
-        
-        Enter created folder then run tests:
-        
-        ```
-        $ flake8 .
-        $ black .
-        $ pytest
-        ```
-        
-        To use pre-commit:
-        
-        ```
-        $ git add *
-        # to apply to staged files
-        $ pre-commit run
-        # restage if changes
-        $ git add *
-        # to run on commits
-        $ pre-commit install
-        $ git commit -m 'Initial commit'
-        ```
-        
-        [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-        [black-link]: https://github.com/ambv/black
-        
-        (package originally created by [python-pkg-cookiecutter](https://github.com/executablebooks/python-pkg-cookiecutter))
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: code_style
 Provides-Extra: testing
 Provides-Extra: docs
+License-File: LICENSE
+
+# magpylib-material-response
+
+[![Code style: black][black-badge]][black-link]
+
+> **Warning**
+> **This package is experimental and in a very dynamic development phase. Breaking API changes may happen at any time.**
+
+Magpylib-Material-Response is an extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets. Leveraging the Method of Moments, it calculates magnetic material response by meshing sources in an arbitrary number of unit elements.
+
+## Installation
+
+Install from PyPi
+
+```console
+$ pip install magpylib-material-response
+```
+
+or locally:
+
+```
+$ pip install -e .[code_style,testing]
+```
+
+## Testing
+
+Enter created folder then run tests:
+
+```
+$ flake8 .
+$ black .
+$ pytest
+```
+
+To use pre-commit:
+
+```
+$ git add *
+# to apply to staged files
+$ pre-commit run
+# restage if changes
+$ git add *
+# to run on commits
+$ pre-commit install
+$ git commit -m 'Initial commit'
+```
+
+[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black-link]: https://github.com/ambv/black
+
+(package originally created by [python-pkg-cookiecutter](https://github.com/executablebooks/python-pkg-cookiecutter))
+
+
```

### Comparing `magpylib-material-response-0.1.0a6/magpylib_material_response.egg-info/SOURCES.txt` & `magpylib-material-response-0.2.0a0/magpylib_material_response.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 magpylib_material_response/__init__.py
 magpylib_material_response/demag.py
 magpylib_material_response/meshing.py
 magpylib_material_response/meshing_utils.py
```

### Comparing `magpylib-material-response-0.1.0a6/setup.py` & `magpylib-material-response-0.2.0a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 """The setup script."""
-from setuptools import find_packages
-from setuptools import setup
+from setuptools import find_packages, setup
 
 with open("magpylib_material_response/__init__.py") as handle:
     for line in handle:
         if "__version__" in line:
             version = line.split(" = ")[-1].replace('"', "")
             break
```

