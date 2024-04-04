# Comparing `tmp/pyBallMapper-0.3.3.tar.gz` & `tmp/pyBallMapper-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBallMapper-0.3.3.tar", last modified: Thu Jan  4 18:52:17 2024, max compression
+gzip compressed data, was "pyBallMapper-0.3.4.tar", last modified: Thu Apr  4 10:15:37 2024, max compression
```

## Comparing `pyBallMapper-0.3.3.tar` & `pyBallMapper-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-01-04 18:52:17.637337 pyBallMapper-0.3.3/
--rw-r--r--   0 dgurnari   (503) staff       (20)     1108 2023-10-03 15:56:33.000000 pyBallMapper-0.3.3/LICENSE.md
--rw-r--r--   0 dgurnari   (503) staff       (20)       29 2023-10-03 15:56:33.000000 pyBallMapper-0.3.3/MANIFEST.in
--rw-r--r--   0 dgurnari   (503) staff       (20)     1500 2024-01-04 18:52:17.637174 pyBallMapper-0.3.3/PKG-INFO
--rw-r--r--   0 dgurnari   (503) staff       (20)     1019 2024-01-04 18:33:57.000000 pyBallMapper-0.3.3/README.md
-drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-01-04 18:52:17.636998 pyBallMapper-0.3.3/pyBallMapper.egg-info/
--rw-r--r--   0 dgurnari   (503) staff       (20)     1500 2024-01-04 18:52:17.000000 pyBallMapper-0.3.3/pyBallMapper.egg-info/PKG-INFO
--rw-r--r--   0 dgurnari   (503) staff       (20)      349 2024-01-04 18:52:17.000000 pyBallMapper-0.3.3/pyBallMapper.egg-info/SOURCES.txt
--rw-r--r--   0 dgurnari   (503) staff       (20)        1 2024-01-04 18:52:17.000000 pyBallMapper-0.3.3/pyBallMapper.egg-info/dependency_links.txt
--rw-r--r--   0 dgurnari   (503) staff       (20)       58 2024-01-04 18:52:17.000000 pyBallMapper-0.3.3/pyBallMapper.egg-info/requires.txt
--rw-r--r--   0 dgurnari   (503) staff       (20)       13 2024-01-04 18:52:17.000000 pyBallMapper-0.3.3/pyBallMapper.egg-info/top_level.txt
-drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-01-04 18:52:17.636580 pyBallMapper-0.3.3/pyballmapper/
--rw-r--r--   0 dgurnari   (503) staff       (20)       34 2023-10-03 15:56:33.000000 pyBallMapper-0.3.3/pyballmapper/__init__.py
--rw-r--r--   0 dgurnari   (503) staff       (20)    19762 2024-01-04 18:48:57.000000 pyBallMapper-0.3.3/pyballmapper/ballmapper.py
--rw-r--r--   0 dgurnari   (503) staff       (20)     4865 2024-01-04 18:23:28.000000 pyBallMapper-0.3.3/pyballmapper/mobm.py
--rw-r--r--   0 dgurnari   (503) staff       (20)     8870 2023-10-03 15:56:33.000000 pyBallMapper-0.3.3/pyballmapper/plotting.py
-drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-01-04 18:52:17.636853 pyBallMapper-0.3.3/pyballmapper/tests/
--rw-r--r--   0 dgurnari   (503) staff       (20)        0 2023-10-03 15:56:33.000000 pyBallMapper-0.3.3/pyballmapper/tests/__init__.py
--rw-r--r--   0 dgurnari   (503) staff       (20)       38 2024-01-04 18:52:17.637370 pyBallMapper-0.3.3/setup.cfg
--rw-r--r--   0 dgurnari   (503) staff       (20)      790 2024-01-04 18:37:05.000000 pyBallMapper-0.3.3/setup.py
+drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-04-04 10:15:37.411543 pyBallMapper-0.3.4/
+-rw-r--r--   0 dgurnari   (503) staff       (20)     1108 2023-10-03 15:56:33.000000 pyBallMapper-0.3.4/LICENSE.md
+-rw-r--r--   0 dgurnari   (503) staff       (20)       29 2023-10-03 15:56:33.000000 pyBallMapper-0.3.4/MANIFEST.in
+-rw-r--r--   0 dgurnari   (503) staff       (20)     1500 2024-04-04 10:15:37.411382 pyBallMapper-0.3.4/PKG-INFO
+-rw-r--r--   0 dgurnari   (503) staff       (20)     1019 2024-01-04 18:33:57.000000 pyBallMapper-0.3.4/README.md
+drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-04-04 10:15:37.411223 pyBallMapper-0.3.4/pyBallMapper.egg-info/
+-rw-r--r--   0 dgurnari   (503) staff       (20)     1500 2024-04-04 10:15:37.000000 pyBallMapper-0.3.4/pyBallMapper.egg-info/PKG-INFO
+-rw-r--r--   0 dgurnari   (503) staff       (20)      349 2024-04-04 10:15:37.000000 pyBallMapper-0.3.4/pyBallMapper.egg-info/SOURCES.txt
+-rw-r--r--   0 dgurnari   (503) staff       (20)        1 2024-04-04 10:15:37.000000 pyBallMapper-0.3.4/pyBallMapper.egg-info/dependency_links.txt
+-rw-r--r--   0 dgurnari   (503) staff       (20)       58 2024-04-04 10:15:37.000000 pyBallMapper-0.3.4/pyBallMapper.egg-info/requires.txt
+-rw-r--r--   0 dgurnari   (503) staff       (20)       13 2024-04-04 10:15:37.000000 pyBallMapper-0.3.4/pyBallMapper.egg-info/top_level.txt
+drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-04-04 10:15:37.410894 pyBallMapper-0.3.4/pyballmapper/
+-rw-r--r--   0 dgurnari   (503) staff       (20)       34 2023-10-03 15:56:33.000000 pyBallMapper-0.3.4/pyballmapper/__init__.py
+-rw-r--r--   0 dgurnari   (503) staff       (20)    19722 2024-02-16 09:04:34.000000 pyBallMapper-0.3.4/pyballmapper/ballmapper.py
+-rw-r--r--   0 dgurnari   (503) staff       (20)     4865 2024-04-04 10:10:48.000000 pyBallMapper-0.3.4/pyballmapper/mobm.py
+-rw-r--r--   0 dgurnari   (503) staff       (20)     9453 2024-04-04 10:03:13.000000 pyBallMapper-0.3.4/pyballmapper/plotting.py
+drwxr-xr-x   0 dgurnari   (503) staff       (20)        0 2024-04-04 10:15:37.411095 pyBallMapper-0.3.4/pyballmapper/tests/
+-rw-r--r--   0 dgurnari   (503) staff       (20)        0 2023-10-03 15:56:33.000000 pyBallMapper-0.3.4/pyballmapper/tests/__init__.py
+-rw-r--r--   0 dgurnari   (503) staff       (20)       38 2024-04-04 10:15:37.411577 pyBallMapper-0.3.4/setup.cfg
+-rw-r--r--   0 dgurnari   (503) staff       (20)      790 2024-04-04 09:45:21.000000 pyBallMapper-0.3.4/setup.py
```

### Comparing `pyBallMapper-0.3.3/LICENSE.md` & `pyBallMapper-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyBallMapper-0.3.3/PKG-INFO` & `pyBallMapper-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBallMapper
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python implementation of the Ball Mapper algorithm.
 Home-page: https://github.com/dgurnari/pyBallMapper
 Author: Davide Gurnari
 Author-email: davide.gurnari@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pyBallMapper-0.3.3/README.md` & `pyBallMapper-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyBallMapper-0.3.3/pyBallMapper.egg-info/PKG-INFO` & `pyBallMapper-0.3.4/pyBallMapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBallMapper
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python implementation of the Ball Mapper algorithm.
 Home-page: https://github.com/dgurnari/pyBallMapper
 Author: Davide Gurnari
 Author-email: davide.gurnari@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `pyBallMapper-0.3.3/pyballmapper/ballmapper.py` & `pyBallMapper-0.3.4/pyballmapper/ballmapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -489,15 +489,15 @@
 
     def draw_networkx(
         self,
         coloring_variable=None,
         color_palette=cm.get_cmap("Reds"),
         colorbar=False,
         colorbar_label=None,
-        this_ax=None,
+        ax=None,
         MIN_VALUE=np.inf,
         MAX_VALUE=-np.inf,
         MIN_SCALE=100,  # default in nx.draw_networkx is 300
         MAX_SCALE=600,
         pos=None,
         **kwargs
     ):
@@ -509,38 +509,38 @@
             the variable to use for coloring the BM graph, by default None
         color_palette : matplotlib.colors.Colormap, optional
             the coloring palette to use, by default cm.get_cmap("Reds")
         colorbar : bool, optional
             the label on the colorbar's long axis.
         colorbar_label : str, optional
             whether to add a colorbar to the plot, by default False
-        this_ax : matplotlib.axes.Axes, optional
+        ax : matplotlib.axes.Axes, optional
             the matplotlib ax where to plot the graph. If None, the current ax is used. By default None
         MIN_VALUE : float, optional
             the value to be assigned to the lowest color in the cmap, by default np.inf
         MAX_VALUE : float, optional
             the value to be assigned to the highest color in the cmap, by default -np.inf
         MIN_SCALE : int, optional
             the minimum radius for the nodes, by default 100
         MIN_SCALE : int, optional
             the maximum radius for the nodes, by default 100
         pos : dictionary, optional
             A dictionary with nodes as keys and positions as values. If not specified a spring layout positioning will be computed. See `networkx.drawing.layout` for functions that compute node positions. By default None
 
         Returns
         -------
-        this_ax
+        ax
             the matplotlib ax
         """
         MAX_NODE_SIZE = max(
             [self.Graph.nodes[node]["size"] for node in self.Graph.nodes]
         )
 
-        if this_ax == None:
-            this_ax = plt.gca()
+        if ax == None:
+            ax = plt.gca()
 
         MIN_VALUE, MAX_VALUE = self.color_by_variable(
             coloring_variable, color_palette, MIN_VALUE, MAX_VALUE
         )
 
         if pos is None:
             pos = nx.spring_layout(self.Graph, seed=24)
@@ -550,23 +550,23 @@
             pos=pos,
             node_color=[self.Graph.nodes[node]["color"] for node in self.Graph.nodes],
             node_size=[
                 MAX_SCALE * self.Graph.nodes[node]["size"] / MAX_NODE_SIZE + MIN_SCALE
                 for node in self.Graph.nodes
             ],
             alpha=0.8,
-            ax=this_ax,
+            ax=ax,
             **kwargs
         )
 
         # plot a legend
         if colorbar:
             sm = plt.cm.ScalarMappable(
                 cmap=color_palette,
                 norm=plt.Normalize(
                     vmin=MIN_VALUE,
                     vmax=MAX_VALUE,
                 ),
             )
-            plt.colorbar(sm, label=colorbar_label, ax=this_ax)
+            plt.colorbar(sm, label=colorbar_label, ax=ax)
 
-        return this_ax
+        return ax
```

### Comparing `pyBallMapper-0.3.3/pyballmapper/mobm.py` & `pyBallMapper-0.3.4/pyballmapper/mobm.py`

 * *Files identical despite different names*

### Comparing `pyBallMapper-0.3.3/pyballmapper/plotting.py` & `pyBallMapper-0.3.4/pyballmapper/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
 import networkx as nx
 
 import csv
 from tqdm.notebook import tqdm
 
-from matplotlib.colors import to_hex
+from matplotlib.colors import to_hex, to_rgb
 
 from bokeh.plotting import figure, show
 
 from bokeh.models import (
     BoxZoomTool,
     Circle,
     HoverTool,
@@ -37,14 +37,17 @@
         # rescale the size for display
         G.nodes[node]["size rescaled"] = (
             MAX_SIZE * G.nodes[node]["size"] / MAX_NODE_SIZE + MIN_SIZE
         )
 
         G.nodes[node]["color"] = to_hex(my_palette(0))
 
+    for edge in G.edges:
+        G.edges[edge]["color"] = to_hex((0, 0, 0))
+
     return G
 
 
 def _color_nodes(
     G, my_variable, my_palette, MIN_VALUE=10000, MAX_VALUE=-10000, logscale=False
 ):
     for node in G.nodes:
@@ -161,31 +164,30 @@
         zoom_tool = WheelZoomTool()
         self.plot.add_tools(
             PanTool(), node_hover_tool, zoom_tool, ResetTool(), SaveTool()
         )
         self.plot.toolbar.active_scroll = zoom_tool
 
         self.graph_renderer = from_networkx(
-            self.bokeh_graph,
-            nx.spring_layout,
+            graph=self.bokeh_graph,
+            layout_function=nx.spring_layout,
             seed=render_seed,
             scale=1,
             center=(0, 0),
             iterations=render_iterations,
         )
-        # k= 10/np.sqrt(len(self.bokeh_graph.nodes)),
 
-        # nodes
-        self.graph_renderer.node_renderer.glyph = Circle(
-            size="size rescaled", fill_color="color", fill_alpha=0.8
+        self.graph_renderer.node_renderer.glyph.update(
+            size="size rescaled",
+            fill_color="color",
+            fill_alpha=0.8,
         )
 
-        # edges
-        self.graph_renderer.edge_renderer.glyph = MultiLine(
-            line_color="black", line_alpha=0.8, line_width=1
+        self.graph_renderer.edge_renderer.glyph.update(
+            line_color="color", line_alpha=0.8, line_width=1
         )
 
         self.plot.renderers.append(self.graph_renderer)
 
     # this function changes the coloring of the nodes
     def color_by_variable(
         self, variable, MIN_VALUE=np.inf, MAX_VALUE=-np.inf, logscale=False
@@ -226,14 +228,27 @@
 
         self.graph_renderer.node_renderer.data_source.data["color"] = [
             self.bokeh_graph.nodes[n]["color"] for n in self.bokeh_graph.nodes
         ]
 
         return MIN_VALUE, MAX_VALUE
 
+    def color_edges(self):
+        """color edges by interpolating between the nodes' colors"""
+
+        for edge in self.bokeh_graph.edges:
+            c0 = np.array(to_rgb(self.bokeh_graph.nodes[edge[0]]["color"]))
+            c1 = np.array(to_rgb(self.bokeh_graph.nodes[edge[1]]["color"]))
+
+            self.bokeh_graph.edges[edge]["color"] = to_hex((c0 + c1) / 2)
+
+        self.graph_renderer.edge_renderer.data_source.data["color"] = [
+            self.bokeh_graph.edges[e]["color"] for e in self.bokeh_graph.edges
+        ]
+
     def add_colorbar(self, num_ticks, low, high):
         """Add a colorbar to the right side of the Bokeh plot.
 
         Parameters
         ----------
         num_ticks : int
             Number of ticks, use a high number (100) for a continuos \
@@ -258,15 +273,15 @@
             major_label_text_font_size="14pt",
             label_standoff=12,
         )
 
         self.plot.add_layout(color_bar, "right")
 
 
-def kmapper_visualize(bm, coloring_df, path_html='output.html', title=None, **kwargs):
+def kmapper_visualize(bm, coloring_df, path_html="output.html", title=None, **kwargs):
     """leverages kepler-mapper visualization tool to produce an interactive html.
     https://kepler-mapper.scikit-tda.org
 
     Parameters
     ----------
     bm : BallMapper
         the BallMapper graph to plot
@@ -279,24 +294,25 @@
     """
     import kmapper as km
     from collections import defaultdict
 
     mapper = km.KeplerMapper(verbose=0)
 
     graph = {}
-    graph['nodes'] = defaultdict(list) 
+    graph["nodes"] = defaultdict(list)
     for n in bm.points_covered_by_landmarks:
-        graph['nodes'][n] = bm.points_covered_by_landmarks[n]
+        graph["nodes"][n] = bm.points_covered_by_landmarks[n]
 
-    graph['links'] = defaultdict(list)
+    graph["links"] = defaultdict(list)
     for u, v in bm.Graph.edges:
-        graph['links'][u].append(v)
+        graph["links"][u].append(v)
 
     graph["meta_data"] = {}
 
     mapper.visualize(
-        graph, path_html=path_html, color_values=coloring_df.to_numpy() ,
+        graph,
+        path_html=path_html,
+        color_values=coloring_df.to_numpy(),
         color_function_name=coloring_df.columns.tolist(),
         title=title,
         **kwargs
     )
-
```

### Comparing `pyBallMapper-0.3.3/setup.py` & `pyBallMapper-0.3.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="pyBallMapper",
-    version="0.3.3",
+    version="0.3.4",
     author="Davide Gurnari",
     author_email="davide.gurnari@gmail.com",
     packages=["pyballmapper", "pyballmapper.tests"],
     url="https://github.com/dgurnari/pyBallMapper",
     license="LICENSE.txt",
     description="Python implementation of the Ball Mapper algorithm.",
     long_description=long_description,
```

