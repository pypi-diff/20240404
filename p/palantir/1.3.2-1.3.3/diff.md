# Comparing `tmp/palantir-1.3.2.tar.gz` & `tmp/palantir-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palantir-1.3.2.tar", last modified: Wed Nov 29 00:29:13 2023, max compression
+gzip compressed data, was "palantir-1.3.3.tar", last modified: Thu Apr  4 21:45:41 2024, max compression
```

## Comparing `palantir-1.3.2.tar` & `palantir-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-11-29 00:29:13.530958 palantir-1.3.2/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    18047 2021-11-19 00:26:10.000000 palantir-1.3.2/LICENSE
--rw-r--r--   0 dotto    (71780) setty_m_grp (239268)     7805 2023-11-29 00:29:13.526850 palantir-1.3.2/PKG-INFO
--rwxrwx---   0 dotto    (71780) setty_m_grp (239268)     6710 2023-11-28 21:33:24.000000 palantir-1.3.2/README.md
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2023-11-29 00:29:13.532389 palantir-1.3.2/setup.cfg
--rwxrwx---   0 dotto    (71780) setty_m_grp (239268)     1493 2023-10-31 19:13:54.000000 palantir-1.3.2/setup.py
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-11-29 00:29:13.424226 palantir-1.3.2/src/
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-11-29 00:29:13.482445 palantir-1.3.2/src/palantir/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      306 2023-10-31 19:13:54.000000 palantir-1.3.2/src/palantir/__init__.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      595 2023-10-31 19:13:54.000000 palantir-1.3.2/src/palantir/config.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    21085 2023-11-27 21:33:17.000000 palantir-1.3.2/src/palantir/core.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3460 2023-11-28 03:03:37.000000 palantir-1.3.2/src/palantir/io.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    73351 2023-11-07 02:21:28.000000 palantir-1.3.2/src/palantir/plot.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1459 2023-10-31 19:13:54.000000 palantir-1.3.2/src/palantir/preprocess.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    20835 2023-11-27 21:48:16.000000 palantir-1.3.2/src/palantir/presults.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)    33474 2023-10-31 19:13:54.000000 palantir-1.3.2/src/palantir/utils.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     5570 2023-10-31 19:13:54.000000 palantir-1.3.2/src/palantir/validation.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      107 2023-10-31 19:13:54.000000 palantir-1.3.2/src/palantir/version.py
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-11-29 00:29:13.519980 palantir-1.3.2/src/palantir.egg-info/
--rw-r--r--   0 dotto    (71780) setty_m_grp (239268)     7805 2023-11-29 00:29:13.000000 palantir-1.3.2/src/palantir.egg-info/PKG-INFO
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      483 2023-11-29 00:29:13.000000 palantir-1.3.2/src/palantir.egg-info/SOURCES.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2023-11-29 00:29:13.000000 palantir-1.3.2/src/palantir.egg-info/dependency_links.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)      175 2023-11-29 00:29:13.000000 palantir-1.3.2/src/palantir.egg-info/requires.txt
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)        9 2023-11-29 00:29:13.000000 palantir-1.3.2/src/palantir.egg-info/top_level.txt
-drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2023-11-29 00:29:13.514491 palantir-1.3.2/tests/
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     4456 2023-11-28 03:46:05.000000 palantir-1.3.2/tests/test_io.py
--rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2354 2023-11-29 00:09:21.000000 palantir-1.3.2/tests/test_util_density.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2024-04-04 21:45:41.244291 palantir-1.3.3/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    18047 2021-11-19 00:26:10.000000 palantir-1.3.3/LICENSE
+-rw-r--r--   0 dotto    (71780) setty_m_grp (239268)     7994 2024-04-04 21:45:41.241255 palantir-1.3.3/PKG-INFO
+-rwxrwx---   0 dotto    (71780) setty_m_grp (239268)     6899 2024-04-04 21:44:22.000000 palantir-1.3.3/README.md
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)       38 2024-04-04 21:45:41.245348 palantir-1.3.3/setup.cfg
+-rwxrwx---   0 dotto    (71780) setty_m_grp (239268)     1493 2023-10-31 19:13:54.000000 palantir-1.3.3/setup.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2024-04-04 21:45:41.117695 palantir-1.3.3/src/
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2024-04-04 21:45:41.200630 palantir-1.3.3/src/palantir/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      306 2023-10-31 19:13:54.000000 palantir-1.3.3/src/palantir/__init__.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      595 2023-10-31 19:13:54.000000 palantir-1.3.3/src/palantir/config.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    21085 2023-11-27 21:33:17.000000 palantir-1.3.3/src/palantir/core.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     3460 2023-11-28 03:03:37.000000 palantir-1.3.3/src/palantir/io.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    73406 2024-04-04 21:34:02.000000 palantir-1.3.3/src/palantir/plot.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     1459 2023-10-31 19:13:54.000000 palantir-1.3.3/src/palantir/preprocess.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    20835 2023-11-27 21:48:16.000000 palantir-1.3.3/src/palantir/presults.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)    34144 2024-01-11 20:47:09.000000 palantir-1.3.3/src/palantir/utils.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     5570 2023-10-31 19:13:54.000000 palantir-1.3.3/src/palantir/validation.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      107 2024-04-04 21:45:22.000000 palantir-1.3.3/src/palantir/version.py
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2024-04-04 21:45:41.235333 palantir-1.3.3/src/palantir.egg-info/
+-rw-r--r--   0 dotto    (71780) setty_m_grp (239268)     7994 2024-04-04 21:45:41.000000 palantir-1.3.3/src/palantir.egg-info/PKG-INFO
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      483 2024-04-04 21:45:41.000000 palantir-1.3.3/src/palantir.egg-info/SOURCES.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        1 2024-04-04 21:45:41.000000 palantir-1.3.3/src/palantir.egg-info/dependency_links.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)      175 2024-04-04 21:45:41.000000 palantir-1.3.3/src/palantir.egg-info/requires.txt
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)        9 2024-04-04 21:45:41.000000 palantir-1.3.3/src/palantir.egg-info/top_level.txt
+drwxrws---   0 dotto    (71780) setty_m_grp (239268)        0 2024-04-04 21:45:41.230611 palantir-1.3.3/tests/
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     4456 2023-11-28 03:46:05.000000 palantir-1.3.3/tests/test_io.py
+-rw-rw----   0 dotto    (71780) setty_m_grp (239268)     2354 2023-11-29 00:09:21.000000 palantir-1.3.3/tests/test_util_density.py
```

### Comparing `palantir-1.3.2/LICENSE` & `palantir-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/PKG-INFO` & `palantir-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palantir
-Version: 1.3.2
+Version: 1.3.3
 Summary: Palantir for modeling continuous cell state and cell fate choices in single cell data
 Home-page: https://github.com/dpeerlab/palantir
 Author: Palantir development team
 Author-email: manu.talanki@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,14 +72,19 @@
                 url = {https://doi.org/10.1038/s41587-019-0068-4},
                 doi = {10.1038/s41587-019-0068-4}
         }
 ____
 
 Release Notes
 -------------
+ ### Version 1.3.3
+ * optional progress bar with `progress=True` in `palantir.utils.run_local_variability`
+ * avoid NaN in local variablility output
+ * compatibility with `scanpy>=1.10.0`
+
  ### Version 1.3.2
  * require `python>=3.8`
  * implement CI for testing
  * fixes for edge cases discoverd through extended testing
  * implement `plot_trajectory` function to show trajectory on the umap
  * scale pseudotime to unit intervall in anndata
```

### Comparing `palantir-1.3.2/README.md` & `palantir-1.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,19 @@
                 url = {https://doi.org/10.1038/s41587-019-0068-4},
                 doi = {10.1038/s41587-019-0068-4}
         }
 ____
 
 Release Notes
 -------------
+ ### Version 1.3.3
+ * optional progress bar with `progress=True` in `palantir.utils.run_local_variability`
+ * avoid NaN in local variablility output
+ * compatibility with `scanpy>=1.10.0`
+
  ### Version 1.3.2
  * require `python>=3.8`
  * implement CI for testing
  * fixes for edge cases discoverd through extended testing
  * implement `plot_trajectory` function to show trajectory on the umap
  * scale pseudotime to unit intervall in anndata
```

### Comparing `palantir-1.3.2/setup.py` & `palantir-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/src/palantir/config.py` & `palantir-1.3.3/src/palantir/config.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/src/palantir/core.py` & `palantir-1.3.3/src/palantir/core.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/src/palantir/io.py` & `palantir-1.3.3/src/palantir/io.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/src/palantir/plot.py` & `palantir-1.3.3/src/palantir/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         umap = data.copy()
     else:
         raise TypeError("'data' should be either sc.AnnData or pd.DataFrame.")
 
     if not isinstance(cells, (pd.Series, np.ndarray, pd.Index, list)):
         if isinstance(cells, str):
             if cells not in data.obs.columns:
-                raise KeyError(f"'{cells}' not found in .obs.")
+                raise KeyError(f"The column '{cells}' was not found in .obs.")
             mask = data.obs[cells].astype(bool).values
             cells = {cell: "" for cell in data.obs[mask].index}
         elif not isinstance(cells, dict):
             raise TypeError(
                 "'cells' should be either list, dict, pd.Series, pd.Index, string "
                 "(as column in .obs), or a boolean array-like."
             )
@@ -945,15 +945,15 @@
     -------
     Tuple
         Color vector and a flag indicating whether it's categorical
     """
 
     color_source_vector = _get_color_source_vector(ad, color, layer=layer)
     color_vector, categorical = _color_vector(
-        ad, color, color_source_vector, palette=palette, na_color=na_color
+        ad, color, values=color_source_vector, palette=palette, na_color=na_color
     )
     if mask is not None:
         color_vector = color_vector[mask]
 
     return color_source_vector, color_vector, categorical
 
 
@@ -1152,17 +1152,17 @@
     if isinstance(vmin, str) or not isinstance(vmin, cabc.Sequence):
         vmin = [vmin]
     if isinstance(vcenter, str) or not isinstance(vcenter, cabc.Sequence):
         vcenter = [vcenter]
     if isinstance(norm, Normalize) or not isinstance(norm, cabc.Sequence):
         norm = [norm]
 
-    if not categorical and color is not None:
+    if categorical == "cont":
         vmin_float, vmax_float, vcenter_float, norm_obj = _get_vboundnorm(
-            vmin, vmax, vcenter, norm, 0, color_vector
+            vmin, vmax, vcenter, norm=norm, index=0, colors=color_vector
         )
         normalize = check_colornorm(
             vmin_float,
             vmax_float,
             vcenter_float,
             norm_obj,
         )
@@ -1187,27 +1187,30 @@
     ax.set_zorder(0)
     ax.set_facecolor("none")
 
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=UserWarning)
         ax.locator_params(axis="both", nbins=nticks)
 
-    if categorical or color_vector.dtype == bool:
+    if color is None:
+        return fig, ax
+
+    if categorical == "cat" or color_vector.dtype == bool:
         _add_categorical_legend(
             ax,
             color_source_vector,
             palette=_get_palette(ad, color),
             legend_anchor=legend_anchor,
             legend_fontweight=legend_fontweight,
             legend_fontsize=legend_fontsize,
             legend_fontoutline=None,
             na_color=na_color,
             na_in_legend=True,
         )
-    elif color_bar_bounds is not None and color is not None:
+    elif color_bar_bounds is not None:
         cax = ax.inset_axes(color_bar_bounds)
         cb = plt.colorbar(points, cax=cax)
         cb.set_label(color)
 
     return fig, ax
 
 
@@ -1724,15 +1727,15 @@
         index=trends.index,
         columns=trends.columns.astype(float),
     )
 
     # Obtain unique clusters and prepare figure
     cluster_labels = (
         clusters.cat.categories
-        if pd.api.types.is_categorical_dtype(clusters)
+        if isinstance(clusters, pd.CategoricalDtype)
         else set(clusters)
     )
     n_rows = int(np.ceil(len(cluster_labels) / 3))
     fig = plt.figure(figsize=[5.5 * 3, 2.5 * n_rows])
 
     # Plot each cluster
     for i, c in enumerate(cluster_labels):
```

### Comparing `palantir-1.3.2/src/palantir/preprocess.py` & `palantir-1.3.3/src/palantir/preprocess.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/src/palantir/presults.py` & `palantir-1.3.3/src/palantir/presults.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/src/palantir/utils.py` & `palantir-1.3.3/src/palantir/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,15 +484,15 @@
     return res
 
 
 def _dot_helper_func(x, y):
     return x.dot(y)
 
 
-def _local_var_helper(expressions, distances):
+def _local_var_helper(expressions, distances, eps=1e-16):
     if hasattr(expressions, "todense"):
 
         def cast(x):
             return x.todense()
 
         issparse = True
     else:
@@ -506,23 +506,25 @@
         try:
             neighbor_expression = cast(expressions[neighbors, :])
             cell_expression = cast(expressions[cell, :])
             expr_deltas = np.array(neighbor_expression - cell_expression)
         except ValueError:
             raise ValueError(f"This cell caused the error: {cell}")
         expr_distance = np.sqrt(np.sum(expr_deltas**2, axis=1, keepdims=True))
-        change_rate = expr_deltas / expr_distance
+        change_rate = expr_deltas / (expr_distance + eps)
         yield np.max(change_rate**2, axis=0)
 
 
 def run_local_variability(
     ad: sc.AnnData,
     expression_key: str = "MAGIC_imputed_data",
     distances_key: str = "distances",
     localvar_key: str = "local_variability",
+    progress: bool = False,
+    eps: float = 1e-16,
 ) -> np.ndarray:
     """
     Compute local gene variability scores for each cell.
 
     This function calculates the variability in gene expression in a local neighbourhood for each cell.
     It adds the result to the layers of the given AnnData object under the specified key.
 
@@ -535,14 +537,18 @@
         If None, uses raw expression data in .X. Default is 'MAGIC_imputed_data'.
     distances_key : str, optional
         Key to access the distances matrix in the obsm of the AnnData object.
         Default is 'distances'.
     localvar_key : str, optional
         Key under which the computed local variability matrix is stored in the layers of the AnnData object.
         Default is 'local_variability'.
+    progress : bool
+        Show progress bar. Requires tqdm to be installed. Default is False.
+    eps : float
+        A small value preventing devision by 0. Defaults to 1e-16.
 
     Returns
     -------
     local_variability : np.ndarray
         A 2D numpy array of local variability scores for each gene in each cell.
     """
 
@@ -553,15 +559,25 @@
     else:
         X = ad.X
 
     if distances_key not in ad.obsp:
         raise KeyError(f"'{distances_key}' not found in .obsp.")
     X_dists = ad.obsp[distances_key]
 
-    local_variability = np.stack(list(_local_var_helper(X, X_dists)))
+    local_var_generator = _local_var_helper(X, X_dists, eps=eps)
+    if progress is True:
+        try:
+            from fastprogress.fastprogress import progress_bar
+        except ModuleNotFoundError:
+            raise Exception(
+                "Showing the progress bar requires the python module `fastprogress` to be installed."
+            )
+        local_var_generator = progress_bar(local_var_generator, total=X.shape[0])
+
+    local_variability = np.stack(list(local_var_generator))
 
     ad.layers[localvar_key] = local_variability
 
     return local_variability
 
 
 def run_magic_imputation(
```

### Comparing `palantir-1.3.2/src/palantir/validation.py` & `palantir-1.3.3/src/palantir/validation.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/src/palantir.egg-info/PKG-INFO` & `palantir-1.3.3/src/palantir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palantir
-Version: 1.3.2
+Version: 1.3.3
 Summary: Palantir for modeling continuous cell state and cell fate choices in single cell data
 Home-page: https://github.com/dpeerlab/palantir
 Author: Palantir development team
 Author-email: manu.talanki@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,14 +72,19 @@
                 url = {https://doi.org/10.1038/s41587-019-0068-4},
                 doi = {10.1038/s41587-019-0068-4}
         }
 ____
 
 Release Notes
 -------------
+ ### Version 1.3.3
+ * optional progress bar with `progress=True` in `palantir.utils.run_local_variability`
+ * avoid NaN in local variablility output
+ * compatibility with `scanpy>=1.10.0`
+
  ### Version 1.3.2
  * require `python>=3.8`
  * implement CI for testing
  * fixes for edge cases discoverd through extended testing
  * implement `plot_trajectory` function to show trajectory on the umap
  * scale pseudotime to unit intervall in anndata
```

### Comparing `palantir-1.3.2/tests/test_io.py` & `palantir-1.3.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `palantir-1.3.2/tests/test_util_density.py` & `palantir-1.3.3/tests/test_util_density.py`

 * *Files identical despite different names*

