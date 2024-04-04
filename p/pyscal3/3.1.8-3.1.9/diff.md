# Comparing `tmp/pyscal3-3.1.8.tar.gz` & `tmp/pyscal3-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal3-3.1.8.tar", last modified: Wed Apr  3 08:58:22 2024, max compression
+gzip compressed data, was "pyscal3-3.1.9.tar", last modified: Thu Apr  4 15:34:22 2024, max compression
```

## Comparing `pyscal3-3.1.8.tar` & `pyscal3-3.1.9.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.742571 pyscal3-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 08:58:19.000000 pyscal3-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 08:58:19.000000 pyscal3-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-03 08:58:22.742571 pyscal3-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-03 08:58:19.000000 pyscal3-3.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.730571 pyscal3-3.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.730571 pyscal3-3.1.8/lib/voro++/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 08:58:19.000000 pyscal3-3.1.8/lib/voro++/voro++.cc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 08:58:19.000000 pyscal3-3.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:58:22.742571 pyscal3-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-03 08:58:19.000000 pyscal3-3.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.730571 pyscal3-3.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.734571 pyscal3-3.1.8/src/pyscal3/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/centrosymmetry.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/cna.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    20884 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/csl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.738571 pyscal3-3.1.8/src/pyscal3/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/data/annotations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/data/element_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/data/structure_data.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/entropy.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.738571 pyscal3-3.1.8/src/pyscal3/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/formats/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/formats/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/formats/mdtraj.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/formats/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/grain_boundary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    38915 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/neighbor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.738571 pyscal3-3.1.8/src/pyscal3/operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/centrosymmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/chemical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/cna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/identify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/neighbor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/operations/voronoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/routines.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/sh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/solids.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/structure_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/system_binding.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/traj_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-03 08:58:19.000000 pyscal3-3.1.8/src/pyscal3/voronoi.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.742571 pyscal3-3.1.8/src/pyscal3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-03 08:58:22.000000 pyscal3-3.1.8/src/pyscal3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-03 08:58:22.000000 pyscal3-3.1.8/src/pyscal3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:58:22.000000 pyscal3-3.1.8/src/pyscal3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:58:22.000000 pyscal3-3.1.8/src/pyscal3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 08:58:22.000000 pyscal3-3.1.8/src/pyscal3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 08:58:22.000000 pyscal3-3.1.8/src/pyscal3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:58:22.742571 pyscal3-3.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_angular.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_centro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_chiparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_cna.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_crystal_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_disorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_nucsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_q12.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_q3.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_q_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_read_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_sro.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_traj_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 08:58:19.000000 pyscal3-3.1.8/tests/test_voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.736783 pyscal3-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-04 15:34:18.000000 pyscal3-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 15:34:18.000000 pyscal3-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-04 15:34:22.736783 pyscal3-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-04 15:34:18.000000 pyscal3-3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.720783 pyscal3-3.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.724783 pyscal3-3.1.9/lib/voro++/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 15:34:18.000000 pyscal3-3.1.9/lib/voro++/voro++.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 15:34:18.000000 pyscal3-3.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:34:22.736783 pyscal3-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-04 15:34:18.000000 pyscal3-3.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.720783 pyscal3-3.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.728783 pyscal3-3.1.9/src/pyscal3/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/centrosymmetry.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/cna.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20884 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/csl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.728783 pyscal3-3.1.9/src/pyscal3/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/data/annotations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/data/element_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/data/structure_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/entropy.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.728783 pyscal3-3.1.9/src/pyscal3/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/formats/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/formats/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/formats/mdtraj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/formats/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/grain_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38915 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/neighbor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.732783 pyscal3-3.1.9/src/pyscal3/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/centrosymmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/chemical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/cna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/identify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/operations/voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/sh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/solids.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/structure_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/system_binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/traj_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-04 15:34:18.000000 pyscal3-3.1.9/src/pyscal3/voronoi.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.736783 pyscal3-3.1.9/src/pyscal3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-04 15:34:22.000000 pyscal3-3.1.9/src/pyscal3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-04 15:34:22.000000 pyscal3-3.1.9/src/pyscal3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:34:22.000000 pyscal3-3.1.9/src/pyscal3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:34:22.000000 pyscal3-3.1.9/src/pyscal3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 15:34:22.000000 pyscal3-3.1.9/src/pyscal3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 15:34:22.000000 pyscal3-3.1.9/src/pyscal3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:34:22.736783 pyscal3-3.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_angular.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_centro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_chiparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_cna.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_crystal_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_disorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_nucsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_q12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_q3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_q_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_read_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_sro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_traj_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-04 15:34:18.000000 pyscal3-3.1.9/tests/test_voronoi.py
```

### Comparing `pyscal3-3.1.8/LICENSE` & `pyscal3-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/PKG-INFO` & `pyscal3-3.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal3
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python library written in C++ for calculation of local atomic structural environment
 Home-page: https://pyscal.org
 Download-URL: https://anaconda.org/conda-forge/pyscal
 Author: Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal3-3.1.8/README.md` & `pyscal3-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/setup.py` & `pyscal3-3.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal3',
-    version='3.1.8',
+    version='3.1.9',
     author='Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Python library written in C++ for calculation of local atomic structural environment',
     long_description=readme,
     long_description_content_type = "text/markdown",
     # tell setuptools to look for any packages under 'src'
     packages=find_packages('src'),
```

### Comparing `pyscal3-3.1.8/src/pyscal3/atoms.py` & `pyscal3-3.1.9/src/pyscal3/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,21 +298,17 @@
             masks = self._validate_condition(condition)
         else:
             masks = self._generate_bool_list(ids=ids, indices=indices, condition=condition)
         masks = [not x for x in masks]
         self._apply_selection(masks)
 
     def delete(self, ids=None, indices=None, condition=None, selection=False):
-        #delete atoms
-        #reassign ids
-        #reassign indices
-        #reassign heads
         masks = self._generate_bool_list(ids=ids, indices=indices, condition=condition, selection=selection)
         delete_list = [masks[self["head"][x]] for x in range(self.ntotal)]
-        delete_ids = [x for x in range(self.ntotal) if masks[x]]
+        delete_ids = [x for x in range(self.ntotal) if delete_list[x]]
         self._delete_atoms(delete_ids)
     
     @property
     def _type_dict(self):
         sp = []
         types, typecounts = np.unique(self["types"][:self.nreal], return_counts=True)
         for t in types:
```

### Comparing `pyscal3-3.1.8/src/pyscal3/attributes.py` & `pyscal3-3.1.9/src/pyscal3/attributes.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/centrosymmetry.cpp` & `pyscal3-3.1.9/src/pyscal3/centrosymmetry.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/cna.cpp` & `pyscal3-3.1.9/src/pyscal3/cna.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/core.py` & `pyscal3-3.1.9/src/pyscal3/core.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/csl.py` & `pyscal3-3.1.9/src/pyscal3/csl.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/data/annotations.yaml` & `pyscal3-3.1.9/src/pyscal3/data/annotations.yaml`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/data/element_data.yaml` & `pyscal3-3.1.9/src/pyscal3/data/element_data.yaml`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/data/structure_data.yaml` & `pyscal3-3.1.9/src/pyscal3/data/structure_data.yaml`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/entropy.cpp` & `pyscal3-3.1.9/src/pyscal3/entropy.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/formats/ase.py` & `pyscal3-3.1.9/src/pyscal3/formats/ase.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/formats/lammps.py` & `pyscal3-3.1.9/src/pyscal3/formats/lammps.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/formats/mdtraj.py` & `pyscal3-3.1.9/src/pyscal3/formats/mdtraj.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/formats/vasp.py` & `pyscal3-3.1.9/src/pyscal3/formats/vasp.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/grain_boundary.py` & `pyscal3-3.1.9/src/pyscal3/grain_boundary.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/misc.py` & `pyscal3-3.1.9/src/pyscal3/misc.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/neighbor.cpp` & `pyscal3-3.1.9/src/pyscal3/neighbor.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/calculations.py` & `pyscal3-3.1.9/src/pyscal3/operations/calculations.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/centrosymmetry.py` & `pyscal3-3.1.9/src/pyscal3/operations/centrosymmetry.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/chemical.py` & `pyscal3-3.1.9/src/pyscal3/operations/chemical.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/cna.py` & `pyscal3-3.1.9/src/pyscal3/operations/cna.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/entropy.py` & `pyscal3-3.1.9/src/pyscal3/operations/entropy.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/identify.py` & `pyscal3-3.1.9/src/pyscal3/operations/identify.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/input.py` & `pyscal3-3.1.9/src/pyscal3/operations/input.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/neighbor.py` & `pyscal3-3.1.9/src/pyscal3/operations/neighbor.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/operations.py` & `pyscal3-3.1.9/src/pyscal3/operations/operations.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/serialize.py` & `pyscal3-3.1.9/src/pyscal3/operations/serialize.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/symmetry.py` & `pyscal3-3.1.9/src/pyscal3/operations/symmetry.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/visualize.py` & `pyscal3-3.1.9/src/pyscal3/operations/visualize.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/operations/voronoi.py` & `pyscal3-3.1.9/src/pyscal3/operations/voronoi.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/routines.py` & `pyscal3-3.1.9/src/pyscal3/routines.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/sh.cpp` & `pyscal3-3.1.9/src/pyscal3/sh.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/solids.cpp` & `pyscal3-3.1.9/src/pyscal3/solids.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/structure_creator.py` & `pyscal3-3.1.9/src/pyscal3/structure_creator.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/system_binding.cpp` & `pyscal3-3.1.9/src/pyscal3/system_binding.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/traj_process.py` & `pyscal3-3.1.9/src/pyscal3/traj_process.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/trajectory.py` & `pyscal3-3.1.9/src/pyscal3/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/visualization.py` & `pyscal3-3.1.9/src/pyscal3/visualization.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3/voronoi.cpp` & `pyscal3-3.1.9/src/pyscal3/voronoi.cpp`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/src/pyscal3.egg-info/PKG-INFO` & `pyscal3-3.1.9/src/pyscal3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscal3
-Version: 3.1.8
+Version: 3.1.9
 Summary: Python library written in C++ for calculation of local atomic structural environment
 Home-page: https://pyscal.org
 Download-URL: https://anaconda.org/conda-forge/pyscal
 Author: Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pyscal3-3.1.8/src/pyscal3.egg-info/SOURCES.txt` & `pyscal3-3.1.9/src/pyscal3.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 src/pyscal3/operations/visualize.py
 src/pyscal3/operations/voronoi.py
 tests/test_angular.py
 tests/test_centro.py
 tests/test_chiparams.py
 tests/test_cna.py
 tests/test_crystal_structures.py
+tests/test_delete.py
 tests/test_disorder.py
 tests/test_entropy.py
 tests/test_masking.py
 tests/test_neighbors.py
 tests/test_nucsize.py
 tests/test_q12.py
 tests/test_q3.py
```

### Comparing `pyscal3-3.1.8/tests/test_chiparams.py` & `pyscal3-3.1.9/tests/test_chiparams.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_cna.py` & `pyscal3-3.1.9/tests/test_cna.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_disorder.py` & `pyscal3-3.1.9/tests/test_disorder.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_masking.py` & `pyscal3-3.1.9/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_neighbors.py` & `pyscal3-3.1.9/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_nucsize.py` & `pyscal3-3.1.9/tests/test_nucsize.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_q12.py` & `pyscal3-3.1.9/tests/test_q12.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_q_system.py` & `pyscal3-3.1.9/tests/test_q_system.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_rdf.py` & `pyscal3-3.1.9/tests/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_read_file.py` & `pyscal3-3.1.9/tests/test_read_file.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_symmetry.py` & `pyscal3-3.1.9/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_system.py` & `pyscal3-3.1.9/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_traj_process.py` & `pyscal3-3.1.9/tests/test_traj_process.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_trajectory.py` & `pyscal3-3.1.9/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `pyscal3-3.1.8/tests/test_voronoi.py` & `pyscal3-3.1.9/tests/test_voronoi.py`

 * *Files identical despite different names*

