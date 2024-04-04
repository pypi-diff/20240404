# Comparing `tmp/gene_trajectory-0.1.4.tar.gz` & `tmp/gene_trajectory-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene_trajectory-0.1.4.tar", last modified: Wed Apr  3 15:38:12 2024, max compression
+gzip compressed data, was "gene_trajectory-0.1.5.tar", last modified: Thu Apr  4 10:03:42 2024, max compression
```

## Comparing `gene_trajectory-0.1.4.tar` & `gene_trajectory-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1070 2024-04-02 19:05:46.814811 gene_trajectory-0.1.4/LICENSE
--rw-r--r--   0        0        0      797 2024-04-03 15:35:44.879769 gene_trajectory-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-03 13:57:55.079643 gene_trajectory-0.1.4/gene_trajectory/__init__.py
--rw-r--r--   0        0        0     1861 2024-04-03 13:57:55.079870 gene_trajectory-0.1.4/gene_trajectory/add_gene_bin_score.py
--rw-r--r--   0        0        0     4642 2024-04-03 13:57:55.080120 gene_trajectory-0.1.4/gene_trajectory/coarse_grain.py
--rw-r--r--   0        0        0     2587 2024-04-03 13:57:55.080644 gene_trajectory-0.1.4/gene_trajectory/compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2337 2024-04-03 13:57:55.080815 gene_trajectory-0.1.4/gene_trajectory/diffusion_map.py
--rw-r--r--   0        0        0     5578 2024-04-03 13:57:55.081416 gene_trajectory-0.1.4/gene_trajectory/extract_gene_trajectory.py
--rw-r--r--   0        0        0     3511 2024-04-03 13:57:55.081822 gene_trajectory-0.1.4/gene_trajectory/gene_distance_shared.py
--rw-r--r--   0        0        0     1497 2024-04-03 13:57:55.081950 gene_trajectory-0.1.4/gene_trajectory/get_graph_distance.py
--rw-r--r--   0        0        0        0 2024-04-03 13:57:55.082048 gene_trajectory-0.1.4/gene_trajectory/plot/__init__.py
--rw-r--r--   0        0        0     2806 2024-04-03 13:57:55.082234 gene_trajectory-0.1.4/gene_trajectory/plot/gene_trajectory_plots.py
--rw-r--r--   0        0        0     1593 2024-04-03 13:57:55.083330 gene_trajectory-0.1.4/gene_trajectory/run_dm.py
--rw-r--r--   0        0        0        0 2024-04-03 13:57:55.083479 gene_trajectory-0.1.4/gene_trajectory/util/__init__.py
--rw-r--r--   0        0        0     3053 2024-04-03 13:57:55.083631 gene_trajectory-0.1.4/gene_trajectory/util/shared_array.py
--rw-r--r--   0        0        0     1374 2024-04-03 15:38:12.916888 gene_trajectory-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 19:05:46.835286 gene_trajectory-0.1.4/test/__init__.py
--rw-r--r--   0        0        0     1988 2024-04-02 19:05:46.835414 gene_trajectory-0.1.4/test/example_data.py
--rw-r--r--   0        0        0      827 2024-04-02 20:03:55.999156 gene_trajectory-0.1.4/test/test_add_gene_bin_score.py
--rw-r--r--   0        0        0     3614 2024-04-02 20:03:56.033614 gene_trajectory-0.1.4/test/test_coarse_grain.py
--rw-r--r--   0        0        0     1102 2024-04-03 08:17:32.831447 gene_trajectory-0.1.4/test/test_compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2446 2024-04-02 20:03:56.002161 gene_trajectory-0.1.4/test/test_diffusion_map.py
--rw-r--r--   0        0        0     3355 2024-04-02 20:03:55.995656 gene_trajectory-0.1.4/test/test_extract_gene_trajectory.py
--rw-r--r--   0        0        0      746 2024-04-02 20:03:56.015847 gene_trajectory-0.1.4/test/test_gene_distance_shared.py
--rw-r--r--   0        0        0      518 2024-04-02 20:03:56.020042 gene_trajectory-0.1.4/test/test_get_graph_distance.py
--rw-r--r--   0        0        0      410 2024-04-02 20:03:56.027597 gene_trajectory-0.1.4/test/test_run_dm.py
--rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 gene_trajectory-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/LICENSE
+-rw-r--r--   0        0        0      797 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/__init__.py
+-rw-r--r--   0        0        0     1861 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/add_gene_bin_score.py
+-rw-r--r--   0        0        0     4642 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/coarse_grain.py
+-rw-r--r--   0        0        0     2846 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/compute_gene_distance_cmd.py
+-rw-r--r--   0        0        0     2337 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/diffusion_map.py
+-rw-r--r--   0        0        0     5578 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/extract_gene_trajectory.py
+-rw-r--r--   0        0        0     3845 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/gene_distance_shared.py
+-rw-r--r--   0        0        0     1497 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/get_graph_distance.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/plot/__init__.py
+-rw-r--r--   0        0        0     2806 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/plot/gene_trajectory_plots.py
+-rw-r--r--   0        0        0     1593 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/run_dm.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/util/__init__.py
+-rw-r--r--   0        0        0     3053 2024-04-04 10:03:39.466315 gene_trajectory-0.1.5/gene_trajectory/util/shared_array.py
+-rw-r--r--   0        0        0     1295 2024-04-04 10:03:42.058318 gene_trajectory-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1988 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/example_data.py
+-rw-r--r--   0        0        0      828 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_add_gene_bin_score.py
+-rw-r--r--   0        0        0     3615 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_coarse_grain.py
+-rw-r--r--   0        0        0     1770 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_compute_gene_distance_cmd.py
+-rw-r--r--   0        0        0     2446 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_diffusion_map.py
+-rw-r--r--   0        0        0     3356 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_extract_gene_trajectory.py
+-rw-r--r--   0        0        0     1124 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_gene_distance_shared.py
+-rw-r--r--   0        0        0      519 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_get_graph_distance.py
+-rw-r--r--   0        0        0      411 2024-04-04 10:03:39.498315 gene_trajectory-0.1.5/tests/test_run_dm.py
+-rw-r--r--   0        0        0     3232 1970-01-01 00:00:00.000000 gene_trajectory-0.1.5/PKG-INFO
```

### Comparing `gene_trajectory-0.1.4/LICENSE` & `gene_trajectory-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/README.md` & `gene_trajectory-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/add_gene_bin_score.py` & `gene_trajectory-0.1.5/gene_trajectory/add_gene_bin_score.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/coarse_grain.py` & `gene_trajectory-0.1.5/gene_trajectory/coarse_grain.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/compute_gene_distance_cmd.py` & `gene_trajectory-0.1.5/gene_trajectory/compute_gene_distance_cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,20 +34,23 @@
 
     :param path: path to the folder where the cost matrix (ot_cost.csv) and the gene expression matrix
                  (gene_expression.mtx) are saved
     :param num_iter_max: the max number of iterations when computing the distance (see ot.emd2)
     :param show_progress_bar: shows a progress bar while running the computation (default: True)
     :param processes:the number of processes to use (defaults to the number of CPUs available)
     """
-    ot_cost = np.loadtxt(path + "/ot_cost.csv", delimiter=",")
-    gene_expr = sio.mmread(path + "/gene_expression.mtx")
+    ot_cost = np.loadtxt(os.path.join(path, "ot_cost.csv"), delimiter=",")
+    gene_expr = sio.mmread(os.path.join(path,"gene_expression.mtx"))
     if issparse(gene_expr):
         gene_expr = gene_expr.todense()
+    gene_pairs_file = os.path.join(path, "gene_pairs.csv")
+    gene_pairs = np.loadtxt(gene_pairs_file, delimiter=",").astype(int) if os.path.isfile(gene_pairs_file) else None
 
-    emd_mat2 = cal_ot_mat_from_numpy(ot_cost=ot_cost, gene_expr=gene_expr, num_iter_max=num_iter_max,
+    emd_mat2 = cal_ot_mat_from_numpy(ot_cost=ot_cost, gene_expr=gene_expr,
+                                     gene_pairs=gene_pairs, num_iter_max=num_iter_max,
                                      show_progress_bar=show_progress_bar, processes=processes)
     np.savetxt(path + "/emd.csv", emd_mat2, delimiter=",")
 
 
 if __name__ == '__main__':
     args = parse_args()
```

### Comparing `gene_trajectory-0.1.4/gene_trajectory/diffusion_map.py` & `gene_trajectory-0.1.5/gene_trajectory/diffusion_map.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/extract_gene_trajectory.py` & `gene_trajectory-0.1.5/gene_trajectory/extract_gene_trajectory.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/gene_distance_shared.py` & `gene_trajectory-0.1.5/gene_trajectory/gene_distance_shared.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from concurrent.futures import ThreadPoolExecutor
 import os
 import time
 from multiprocessing.managers import SharedMemoryManager
+from typing import Optional, Sized
 
 import numpy as np
 import ot
 from tqdm import tqdm
 
 from gene_trajectory.util.shared_array import SharedArray, PartialStarApply
 
@@ -18,69 +19,70 @@
 # - Using ThreadPoolExecutor as ProcessPoolExecutor (which would make more sense) sometimes halts on Mac,
 #   even when changing multiprocessing.set_start_method('fork')
 
 
 def cal_ot_mat(
         ot_cost: np.array,
         gene_expr: np.array,
+        gene_pairs: Optional[Sized] = None,
         num_iter_max=_DEFAULT_NUMITERMAX,
         show_progress_bar=True,
-        processes: int = None,
+        processes: Optional[int] = None,
 ) -> np.array:
     """
     Calculate the earth mover distance matrix. Note that this step is computationally expensive
     and will be performed in parallel.
 
     :param ot_cost: the cost matrix
     :param gene_expr: the gene expression matrix
+    :param gene_pairs: only compute the distance for the given pairs (0-indexed) (default: None).
+           the distance entry for missing pairs will be set to 1000*max(computed_gene_distances)
     :param num_iter_max: the max number of iterations when computing the distance (see ot.emd2)
     :param show_progress_bar: shows a progress bar while running the computation (default: True)
     :param processes:the number of processes to use (defaults to the number of CPUs available)
     :return: the distance matrix
     """
     processes = int(processes) if isinstance(processes, float) else os.cpu_count()
+    n = gene_expr.shape[1]
     if show_progress_bar:
         logger.info(f'Computing emd distance..')
 
-    with SharedMemoryManager() as manager:
-        n = gene_expr.shape[1]
-
+    if gene_pairs is None:
+        pairs = ((i, j) for i in range(0, n - 1) for j in range(i + 1, n))
         npairs = (n * (n - 1)) // 2
+    else:
+        pairs = gene_pairs
+        npairs = len(gene_pairs)
+
+    emd_mat = np.full((n, n), fill_value=np.NaN)
 
+    with SharedMemoryManager() as manager:
         start_time = time.perf_counter()
         # create and configure the process pool
 
         with ThreadPoolExecutor(max_workers=processes) as pool:
             # prepare shared environment
             cost = SharedArray.copy(manager, np.asarray(ot_cost))
             gexp = SharedArray.copy(manager, np.asarray(gene_expr))
             f = PartialStarApply(_cal_ot, cost, gexp)
 
-            # prepare arguments
-            items = ((num_iter_max, i, j) for i in range(0, n - 1) for j in range(i + 1, n))
-
             # execute tasks and process results
-            result_generator = pool.map(f, items)
+            result_generator = pool.map(f,  ((num_iter_max, i, j) for i, j in pairs))
             if show_progress_bar:
                 result_generator = tqdm(result_generator, total=npairs, position=0, leave=True)
-            result = list(result_generator)
+            for d, i, j in result_generator:
+                emd_mat[i, j] = emd_mat[j, i] = d
         finish_time = time.perf_counter()
-
         if show_progress_bar:
             logger.info("Program finished in {} seconds - using multiprocessing".format(finish_time - start_time))
 
-        ind = 0
-        emd_mat = np.zeros((n, n))
-        for i in range(0, n - 1):
-            for j in range(i + 1, n):
-                emd_mat[i, j] = result[ind]
-                ind += 1
+        np.fill_diagonal(emd_mat, 0)
+        np.nan_to_num(emd_mat, nan=1000 * np.nanmax(emd_mat), copy=False)
 
-        emd_mat2 = emd_mat + np.transpose(emd_mat)
-        return emd_mat2
+        return emd_mat
 
 
 def _cal_ot(ot_cost_matrix: np.array, gene_expr_matrix: np.array, num_iter_max: int, i: int, j: int):
     """
     Computes the EMD between i and j
     """
     gene_i = np.array(gene_expr_matrix[:, i]).reshape(-1)
@@ -89,8 +91,8 @@
     gene_j = gene_j / sum(gene_j)
 
     emd_dist = ot.emd2(gene_i[np.nonzero(gene_i)],
                        gene_j[np.nonzero(gene_j)],
                        ot_cost_matrix[np.nonzero(gene_i)[0], :][:, np.nonzero(gene_j)[0]],
                        numItermax=num_iter_max)
     # return the generated value
-    return emd_dist
+    return emd_dist, i, j
```

### Comparing `gene_trajectory-0.1.4/gene_trajectory/get_graph_distance.py` & `gene_trajectory-0.1.5/gene_trajectory/get_graph_distance.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/plot/gene_trajectory_plots.py` & `gene_trajectory-0.1.5/gene_trajectory/plot/gene_trajectory_plots.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/run_dm.py` & `gene_trajectory-0.1.5/gene_trajectory/run_dm.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/gene_trajectory/util/shared_array.py` & `gene_trajectory-0.1.5/gene_trajectory/util/shared_array.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/pyproject.toml` & `gene_trajectory-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "gene-trajectory"
-version = "0.1.4"
+version = "0.1.5"
 description = "Compute gene trajectories"
 readme = "README.md"
 authors = [
     { name = "Francesco Strino", email = "francesco.strino@pcmgf.com" },
     { name = "Rihao Qu", email = "rihao.qu@yale.edu" },
 ]
 maintainers = [
@@ -51,13 +51,8 @@
 ]
 
 [project.urls]
 Documentation = "https://github.com/KlugerLab/GeneTrajectory-python.git"
 Repository = "https://github.com/KlugerLab/GeneTrajectory-python.git"
 "Bug Tracker" = "https://github.com/KlugerLab/GeneTrajectory-python/issues"
 
-[tool.hatch.build]
-exclude = [
-    "notebooks",
-    "test",
-    "requirements.txt",
-]
+[tool]
```

### Comparing `gene_trajectory-0.1.4/test/example_data.py` & `gene_trajectory-0.1.5/tests/example_data.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/test/test_add_gene_bin_score.py` & `gene_trajectory-0.1.5/tests/test_add_gene_bin_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import numpy as np
 
 from gene_trajectory.add_gene_bin_score import add_gene_bin_score
-from test.example_data import example_adata, diffusion_map, gene_trajectories, to_adata, gene_expression
+from tests.example_data import example_adata, diffusion_map, gene_trajectories, to_adata, gene_expression
 
 
 class AddGeneScoreTestCase(unittest.TestCase):
     def test_add_gene_bin_score(self):
 
         adata = to_adata(gene_expression.T, var_names=list(gene_trajectories.index.values))
```

### Comparing `gene_trajectory-0.1.4/test/test_coarse_grain.py` & `gene_trajectory-0.1.5/tests/test_coarse_grain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 import numpy as np
 from sklearn.metrics import pairwise_distances
 
 from gene_trajectory.coarse_grain import coarse_grain, select_top_genes
-from test.example_data import example_adata, random_adata
+from tests.example_data import example_adata, random_adata
 
 
 class CoarseGrainTestCase(unittest.TestCase):
     @staticmethod
     def test_cg():
         """
         Generated in R using
```

### Comparing `gene_trajectory-0.1.4/test/test_compute_gene_distance_cmd.py` & `gene_trajectory-0.1.5/tests/test_compute_gene_distance_cmd.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,20 +20,36 @@
         [.6, .2, .2]])
 
     expected_emd = np.array([
         [0.0, 0.8, 1.0],
         [0.8, 0.0, 0.9],
         [1.0, 0.9, 0.0]])
 
+    gene_pairs = np.array([[0, 1], [1, 1], [2, 1]], dtype=int)
+
     def test_compute_gene_distance_cmd(self):
         with TemporaryDirectory() as d:
             np.savetxt(os.path.join(d, 'ot_cost.csv'), self.gdm, delimiter=',')
             sio.mmwrite(os.path.join(d, 'gene_expression.mtx'), coo_matrix(self.gem.T))
 
             cal_ot_mat(d, show_progress_bar=False)
 
             res = np.loadtxt(d + "/emd.csv", delimiter=",")
             np.testing.assert_almost_equal(res, self.expected_emd, decimal=6)
 
+    def test_cal_ot_mat_gene_pairs(self):
+        exp = self.expected_emd.copy()
+        exp[0, 2] = exp[2, 0] = 900
+
+        with TemporaryDirectory() as d:
+            np.savetxt(os.path.join(d, 'ot_cost.csv'), self.gdm, delimiter=',')
+            sio.mmwrite(os.path.join(d, 'gene_expression.mtx'), coo_matrix(self.gem.T))
+            np.savetxt(os.path.join(d, 'gene_pairs.csv'), self.gene_pairs, fmt='%d', delimiter=',')
+
+            cal_ot_mat(d, show_progress_bar=False)
+
+            res = np.loadtxt(d + "/emd.csv", delimiter=",")
+            np.testing.assert_almost_equal(res, exp, decimal=6)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `gene_trajectory-0.1.4/test/test_diffusion_map.py` & `gene_trajectory-0.1.5/tests/test_diffusion_map.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.4/test/test_extract_gene_trajectory.py` & `gene_trajectory-0.1.5/tests/test_extract_gene_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import pandas as pd
 
 from gene_trajectory.extract_gene_trajectory import get_gene_embedding, get_randow_walk_matrix, get_gene_pseudoorder, \
     extract_gene_trajectory
-from test.example_data import gene_names, gene_trajectories
+from tests.example_data import gene_names, gene_trajectories
 
 
 class CoarseGrainTestCase(unittest.TestCase):
     gdm = np.array([
         [0.000000, 4.269544, 4.414329, 7.247308, 8.027305],
         [4.269544, 0.000000, 6.927429, 6.761171, 8.801408],
         [4.414329, 6.927429, 0.000000, 6.531824, 6.798761],
```

### Comparing `gene_trajectory-0.1.4/test/test_gene_distance_shared.py` & `gene_trajectory-0.1.5/tests/test_gene_distance_shared.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,25 @@
         [.6, .2, .2]])
 
     expected_emd = np.array([
         [0.0, 0.8, 1.0],
         [0.8, 0.0, 0.9],
         [1.0, 0.9, 0.0]])
 
+    gene_pairs = [(0, 1), (1, 1), (2, 1)]
+
     def test_gene_distance_shared(self):
         mt = cal_ot_mat(ot_cost=self.gdm, gene_expr=self.gem.T, show_progress_bar=False)
         np.testing.assert_almost_equal(self.expected_emd, mt, 6)
 
+    def test_cal_ot_mat_gene_pairs(self):
+        exp = self.expected_emd.copy()
+        exp[0, 2] = exp[2, 0] = 900
+
+        mt = cal_ot_mat(ot_cost=self.gdm, gene_expr=self.gem.T,
+                        gene_pairs=self.gene_pairs,
+                        show_progress_bar=False)
+        np.testing.assert_almost_equal(exp, mt, 6)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `gene_trajectory-0.1.4/test/test_get_graph_distance.py` & `gene_trajectory-0.1.5/tests/test_get_graph_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 import numpy as np
 
 from gene_trajectory.get_graph_distance import get_graph_distance
-from test.example_data import example_adata, diffusion_map, graph_distance
+from tests.example_data import example_adata, diffusion_map, graph_distance
 
 
 class CoarseGrainTestCase(unittest.TestCase):
     @staticmethod
     def test_get_graph_distance():
         adata = example_adata()
         adata.obsm['X_dm'] = diffusion_map
```

### Comparing `gene_trajectory-0.1.4/PKG-INFO` & `gene_trajectory-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-trajectory
-Version: 0.1.4
+Version: 0.1.5
 Summary: Compute gene trajectories
 Keywords: Gene trajectory scRNA-seq
 Author-Email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
 Maintainer-Email: Francesco Strino <francesco.strino@pcmgf.com>
 License: MIT License
         
         Copyright (c) 2024 PCMGF-Limited
```

