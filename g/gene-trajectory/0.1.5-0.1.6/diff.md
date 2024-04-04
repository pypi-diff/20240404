# Comparing `tmp/gene_trajectory-0.1.5.tar.gz` & `tmp/gene_trajectory-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene_trajectory-0.1.5.tar", last modified: Thu Apr  4 10:03:42 2024, max compression
+gzip compressed data, was "gene_trajectory-0.1.6.tar", last modified: Thu Apr  4 10:54:28 2024, max compression
```

## Comparing `gene_trajectory-0.1.5.tar` & `gene_trajectory-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1070 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/LICENSE
--rw-r--r--   0        0        0      797 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/__init__.py
--rw-r--r--   0        0        0     1861 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/add_gene_bin_score.py
--rw-r--r--   0        0        0     4642 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/coarse_grain.py
--rw-r--r--   0        0        0     2846 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2337 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/diffusion_map.py
--rw-r--r--   0        0        0     5578 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/extract_gene_trajectory.py
--rw-r--r--   0        0        0     3845 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/gene_distance_shared.py
--rw-r--r--   0        0        0     1497 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/get_graph_distance.py
--rw-r--r--   0        0        0        0 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/plot/__init__.py
--rw-r--r--   0        0        0     2806 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/plot/gene_trajectory_plots.py
--rw-r--r--   0        0        0     1593 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/run_dm.py
--rw-r--r--   0        0        0        0 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/util/__init__.py
--rw-r--r--   0        0        0     3053 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/util/shared_array.py
--rw-r--r--   0        0        0     1295 2024-04-04 10:03:42.058318 gene_trajectory-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1988 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/example_data.py
--rw-r--r--   0        0        0      828 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_add_gene_bin_score.py
--rw-r--r--   0        0        0     3615 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_coarse_grain.py
--rw-r--r--   0        0        0     1770 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2446 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_diffusion_map.py
--rw-r--r--   0        0        0     3356 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_extract_gene_trajectory.py
--rw-r--r--   0        0        0     1124 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_gene_distance_shared.py
--rw-r--r--   0        0        0      519 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_get_graph_distance.py
--rw-r--r--   0        0        0      411 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_run_dm.py
--rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 gene_trajectory-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 10:54:22.810063 gene_trajectory-0.1.6/LICENSE
+-rw-r--r--   0        0        0      797 2024-04-04 10:54:22.810063 gene_trajectory-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 10:54:22.810063 gene_trajectory-0.1.6/gene_trajectory/__init__.py
+-rw-r--r--   0        0        0     1861 2024-04-04 10:54:22.810063 gene_trajectory-0.1.6/gene_trajectory/add_gene_bin_score.py
+-rw-r--r--   0        0        0     4642 2024-04-04 10:54:22.810063 gene_trajectory-0.1.6/gene_trajectory/coarse_grain.py
+-rw-r--r--   0        0        0     2846 2024-04-04 10:54:22.810063 gene_trajectory-0.1.6/gene_trajectory/compute_gene_distance_cmd.py
+-rw-r--r--   0        0        0     2337 2024-04-04 10:54:22.810063 gene_trajectory-0.1.6/gene_trajectory/diffusion_map.py
+-rw-r--r--   0        0        0     5578 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/extract_gene_trajectory.py
+-rw-r--r--   0        0        0     3845 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/gene_distance_shared.py
+-rw-r--r--   0        0        0     1497 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/get_graph_distance.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/plot/__init__.py
+-rw-r--r--   0        0        0     2806 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/plot/gene_trajectory_plots.py
+-rw-r--r--   0        0        0     1593 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/run_dm.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/util/__init__.py
+-rw-r--r--   0        0        0     3053 2024-04-04 10:54:22.814063 gene_trajectory-0.1.6/gene_trajectory/util/shared_array.py
+-rw-r--r--   0        0        0     1295 2024-04-04 10:54:28.490103 gene_trajectory-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1988 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/example_data.py
+-rw-r--r--   0        0        0      828 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_add_gene_bin_score.py
+-rw-r--r--   0        0        0     3615 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_coarse_grain.py
+-rw-r--r--   0        0        0     1770 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_compute_gene_distance_cmd.py
+-rw-r--r--   0        0        0     2446 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_diffusion_map.py
+-rw-r--r--   0        0        0     3356 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_extract_gene_trajectory.py
+-rw-r--r--   0        0        0     1124 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_gene_distance_shared.py
+-rw-r--r--   0        0        0      519 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_get_graph_distance.py
+-rw-r--r--   0        0        0      411 2024-04-04 10:54:22.842063 gene_trajectory-0.1.6/tests/test_run_dm.py
+-rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 gene_trajectory-0.1.6/PKG-INFO
```

### Comparing `gene_trajectory-0.1.5/LICENSE` & `gene_trajectory-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/README.md` & `gene_trajectory-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/add_gene_bin_score.py` & `gene_trajectory-0.1.6/gene_trajectory/add_gene_bin_score.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/coarse_grain.py` & `gene_trajectory-0.1.6/gene_trajectory/coarse_grain.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/compute_gene_distance_cmd.py` & `gene_trajectory-0.1.6/gene_trajectory/compute_gene_distance_cmd.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/diffusion_map.py` & `gene_trajectory-0.1.6/gene_trajectory/diffusion_map.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/extract_gene_trajectory.py` & `gene_trajectory-0.1.6/gene_trajectory/extract_gene_trajectory.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/gene_distance_shared.py` & `gene_trajectory-0.1.6/gene_trajectory/gene_distance_shared.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/get_graph_distance.py` & `gene_trajectory-0.1.6/gene_trajectory/get_graph_distance.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/plot/gene_trajectory_plots.py` & `gene_trajectory-0.1.6/gene_trajectory/plot/gene_trajectory_plots.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/run_dm.py` & `gene_trajectory-0.1.6/gene_trajectory/run_dm.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/gene_trajectory/util/shared_array.py` & `gene_trajectory-0.1.6/gene_trajectory/util/shared_array.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/pyproject.toml` & `gene_trajectory-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "gene-trajectory"
-version = "0.1.5"
+version = "0.1.6"
 description = "Compute gene trajectories"
 readme = "README.md"
 authors = [
     { name = "Francesco Strino", email = "francesco.strino@pcmgf.com" },
     { name = "Rihao Qu", email = "rihao.qu@yale.edu" },
 ]
 maintainers = [
```

### Comparing `gene_trajectory-0.1.5/tests/example_data.py` & `gene_trajectory-0.1.6/tests/example_data.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/tests/test_add_gene_bin_score.py` & `gene_trajectory-0.1.6/tests/test_add_gene_bin_score.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/tests/test_coarse_grain.py` & `gene_trajectory-0.1.6/tests/test_coarse_grain.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/tests/test_compute_gene_distance_cmd.py` & `gene_trajectory-0.1.6/tests/test_compute_gene_distance_cmd.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/tests/test_diffusion_map.py` & `gene_trajectory-0.1.6/tests/test_diffusion_map.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/tests/test_extract_gene_trajectory.py` & `gene_trajectory-0.1.6/tests/test_extract_gene_trajectory.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/tests/test_gene_distance_shared.py` & `gene_trajectory-0.1.6/tests/test_gene_distance_shared.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/tests/test_get_graph_distance.py` & `gene_trajectory-0.1.6/tests/test_get_graph_distance.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.5/PKG-INFO` & `gene_trajectory-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-trajectory
-Version: 0.1.5
+Version: 0.1.6
 Summary: Compute gene trajectories
 Keywords: Gene trajectory scRNA-seq
 Author-Email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
 Maintainer-Email: Francesco Strino <francesco.strino@pcmgf.com>
 License: MIT License
         
         Copyright (c) 2024 PCMGF-Limited
```

