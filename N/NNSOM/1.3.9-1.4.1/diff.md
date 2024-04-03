# Comparing `tmp/nnsom-1.3.9.tar.gz` & `tmp/nnsom-1.4.1.tar.gz`

## Comparing `nnsom-1.3.9.tar` & `nnsom-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    55517 2020-02-02 00:00:00.000000 nnsom-1.3.9/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.3.9/src/NNSOM/som.py
--rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 nnsom-1.3.9/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.3.9/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.3.9/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.3.9/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0    59021 2020-02-02 00:00:00.000000 nnsom-1.4.1/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.1/src/NNSOM/som.py
+-rw-r--r--   0        0        0    20699 2020-02-02 00:00:00.000000 nnsom-1.4.1/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.1/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.1/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.1/PKG-INFO
```

### Comparing `nnsom-1.3.9/src/NNSOM/plots.py` & `nnsom-1.4.1/src/NNSOM/plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         if mouse_click and connect_pick_event:
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, patches, text
 
-    def gray_hist(self, x, perc, mouse_click=False, connect_pick_event=True, **kwargs):
+    def gray_hist(self, x, perc, mouse_click=False, **kwargs):
         # Make another hit histogram figure, and change the colors of the hexagons
         # to indicate the perc of pdb (or gb) ligands in each cluster. Lighter color
         # means more PDB ligands, darker color means more well-docked bad binders.
 
         numNeurons = self.numNeurons
 
         fig, ax, patches, text = self.hit_hist(x, False, mouse_click, **kwargs)
@@ -294,15 +294,15 @@
             patches[neuron][0]._facecolor = color
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
-    def color_hist(self, x, avg, mouse_click=False, connect_pick_event=True, **kwargs):
+    def color_hist(self, x, avg, mouse_click=False, **kwargs):
         # Plot an SOM figure where the size of the hexagons is related to
         # the number of elements in the clusters, and the color of the
         # inner hexagon is coded to the variable avg, which could be the
         # average number of a certain type of bond in the cluster
 
         # Find the maximum value of avg across all clusters
         dmax = np.amax(np.abs(avg))
@@ -344,17 +344,15 @@
         cbar.ax.set_yticklabels(ticktext)
 
         # Get rid of extra white space on sides
         fig.tight_layout()
 
         return fig, patches, text, cbar
 
-    # Need to be generalized
-    def cmplx_hit_hist(self, x, clust, perc, ind_missClass, ind21, ind12, mouse_click=False, connect_pick_event=True,
-                       **kwargs):
+    def cmplx_hit_hist(self, x, clust, perc, ind_missClass, ind21, ind12, mouse_click=False, **kwargs):
         """ Generates a complex hit histogram.
         It indicates what the majority class in each cluster is, and how many specific class occur in each cluster.
 
         Args:
             x: array-like
                 The input data to be clustered
             clust: list
@@ -402,14 +400,93 @@
             patches[neuron][0]._edgecolor = color
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
+    def custom_cmplx_hit_hist(self, x, face_labels, edge_labels, edge_width, mouse_click=False, **kwargs):
+        """ Generate cmplex hit hist
+        Users can specify the face color, edge width and edge color for each neuron.
+
+        x: array-like or sequence of vectors
+            The input data to be clustered
+        face_labels: array-like
+            class labels to determine the face color of the hexagons
+        edge_labels: array-like
+            class labels to determine the edge color of the hexagons
+        edge_width: array-like
+            A list of edge_width standerdised between (1 - 20).
+            You can call get_edge_width to get the standardised edge width in the utils function.
+            len(edge_width) must be equal to the number of neurons
+        mouse_click: bool
+            If true, the interactive plot and sub-clustering functionalities to be activated
+        kwargs: dict
+            Additional arguments to be passed to the onpick function
+            Possible keys include:
+            'data', 'clust', 'target', 'num1', 'num2',
+            'cat', 'align', 'height' and 'topn'
+
+        Returns:
+            fig, ax, patches, text
+        """
+        numNeurons = self.numNeurons
+
+        x = np.asarray(x, np.float32)
+        face_labels = np.asarray(face_labels, np.float32)
+        edge_labels = np.asarray(edge_labels, np.float32)
+        edge_width = np.asarray(edge_width, np.float32)
+
+        # Check if the input data is a sequence of vectors
+        if x.ndim != 2:
+            raise ValueError("x must be a 2D array")
+
+        # Check if the input data can be cdist with self.w
+        # the input data must be transposed
+        if x.shape[0] != self.w.shape[1]:
+            raise ValueError("The input data must have the same number of features as the SOM")
+
+        # Check if the face color, line width and edge color are 1D arrays
+        if face_labels.ndim != 1 or edge_width.ndim != 1 or edge_labels.ndim != 1:
+            raise ValueError("fcolor, lwidth and ecolor must be 1D arrays")
+
+        # Check if the length of fcolor, lwidth and ecolor are equal to the number of neurons
+        if len(face_labels) != numNeurons or len(edge_width) != numNeurons or len(edge_labels) != numNeurons:
+            raise ValueError("The length of x, fcolor, lwidth and ecolor must be equal to the number of neurons")
+
+        # Make hit histogram
+        fig, ax, patches, text = self.hit_hist(x, True, mouse_click, **kwargs)
+
+        # Exclude nan values for the unique color count
+        unique_fcolor = np.unique(face_labels[~np.isnan(face_labels)])
+        unique_ecolor = np.unique(edge_labels[~np.isnan(edge_labels)])
+
+        # Create the colormaps
+        cmap1 = plt.get_cmap('jet', len(unique_fcolor))
+        cmap2 = plt.get_cmap('cool', len(unique_ecolor))
+
+        for neuron in range(numNeurons):
+            if not np.isnan(face_labels[neuron]):
+                # Normalize the class label to the colormap index
+                color1_idx = np.argwhere(unique_fcolor == face_labels[neuron])[0][0] / (len(unique_fcolor) - 1)
+                color2_idx = np.argwhere(unique_ecolor == edge_labels[neuron])[0][0] / (len(unique_ecolor) - 1)
+
+                # Get the corresponding color from the colormap
+                patches[neuron][0]._facecolor = cmap1(color1_idx)
+                patches[neuron][0]._linewidth = edge_width[neuron]
+                patches[neuron][0]._edgecolor = cmap2(color2_idx)
+
+        # Get rid of extra white space on sides
+        plt.tight_layout()
+
+        print(cmap1)
+        print(cmap2)
+
+        return fig, ax, patches, text
+
     def plt_nc(self, mouse_click=False, connect_pick_event=True, **kwargs):
         """ Generates neighborhood connection map.
         The gray hexagons represent cluster centers.
 
         Args:
             mouse_click: bool
                 If true, the interactive plot and sub-clustering functionalities to be activated
```

### Comparing `nnsom-1.3.9/src/NNSOM/som.py` & `nnsom-1.4.1/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.3.9/src/NNSOM/utils.py` & `nnsom-1.4.1/src/NNSOM/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -572,14 +572,71 @@
         A tuple (min_value, max_value) where min_value is the minimum value
         in the data, and max_value is the maximum value.
     """
     flat_list = flatten(data)
     return min(flat_list), max(flat_list)
 
 
+def get_edge_width(indices, clust):
+    """ Calculate edge width for each cluster based on the number of indices in the cluster.
+
+    Args:
+        indices: 1-d array
+            Array of indices for the specific class.
+        clust: sequence of vectors
+            A sequence of vectors, each containing the indices of elements in a cluster.
+
+    Returns:
+        lwidth: 1-d array
+            Array of edge widths for each cluster.
+    """
+
+    lwidth = np.zeros(len(clust))
+
+    for i in range(len(clust)):
+        if len(clust[i]) != 0:
+            if len(np.intersect1d(clust[i], indices)) > 0:
+                lwidth[i] = 20. * len(np.intersect1d(clust[i], indices)) / len(clust[i])
+            else:
+                lwidth[i] = None
+        else:
+            lwidth[i] = None
+
+    return lwidth
+
+
+def get_edge_color(clust, *args):
+    """ Calculate edge color for each cluster based on the number of indices in the cluster.
+
+    Args:
+        clust: sequence of vectors
+            A sequence of vectors, each containing the indices of elements in a cluster.
+
+        *args: 1-d array
+            A list of indices where the specific class is present.
+    """
+
+    # unpack the args
+    numst = list(args)
+
+    # Initialize the edge color array
+    edge_color = np.zeros(len(clust))
+
+    # Detect the intersection of the cluster and each list of indices (class),
+    # and get the majority class in the cluster.
+    # Append the majority class to the edge color array.
+    for i in range(len(clust)):
+        if len(clust[i]) != 0:
+            intersection = [len(np.intersect1d(clust[i], numst[j])) for j in range(len(numst))]
+            edge_color[i] = np.argmax(intersection)
+        else:
+            edge_color[i] = None
+
+    return edge_color
+
 
 # Helper functions to create button objects in the interactive plot
 def create_buttons(fig, button_types):
     sidebar_width = 0.2
     button_config = calculate_button_positions(len(button_types), sidebar_width)
 
     buttons = {}
```

### Comparing `nnsom-1.3.9/.gitignore` & `nnsom-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.3.9/pyproject.toml` & `nnsom-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.3.9"
+version = "1.4.1"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.3.9/PKG-INFO` & `nnsom-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.3.9
+Version: 1.4.1
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

