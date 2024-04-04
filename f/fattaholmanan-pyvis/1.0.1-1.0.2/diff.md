# Comparing `tmp/fattaholmanan-pyvis-1.0.1.tar.gz` & `tmp/fattaholmanan-pyvis-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fattaholmanan-pyvis-1.0.1.tar", last modified: Thu Apr  4 12:56:59 2024, max compression
+gzip compressed data, was "fattaholmanan-pyvis-1.0.2.tar", last modified: Thu Apr  4 13:56:52 2024, max compression
```

## Comparing `fattaholmanan-pyvis-1.0.1.tar` & `fattaholmanan-pyvis-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.710292 fattaholmanan-pyvis-1.0.1/
--rw-rw-r--   0 afattaholman   (502) staff       (20)     1533 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/LICENSE_BSD.txt
--rw-rw-r--   0 afattaholman   (502) staff       (20)       66 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/MANIFEST.in
--rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 12:56:59.709907 fattaholmanan-pyvis-1.0.1/PKG-INFO
--rw-rw-r--   0 afattaholman   (502) staff       (20)     1270 2024-04-04 12:55:09.000000 fattaholmanan-pyvis-1.0.1/README.md
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.709516 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/
--rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/PKG-INFO
--rw-r--r--   0 afattaholman   (502) staff       (20)      890 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/SOURCES.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/dependency_links.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/requires.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/top_level.txt
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.702745 fattaholmanan-pyvis-1.0.1/pyvis/
--rw-rw-r--   0 afattaholman   (502) staff       (20)       56 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/__init__.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 12:53:38.000000 fattaholmanan-pyvis-1.0.1/pyvis/_version.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)      292 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/edge.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)    39291 2024-04-04 12:54:44.000000 fattaholmanan-pyvis-1.0.1/pyvis/network.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)      310 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/node.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     7782 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/options.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     4086 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/physics.py
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.703455 fattaholmanan-pyvis-1.0.1/pyvis/templates/
--rw-rw-r--   0 afattaholman   (502) staff       (20)     3188 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/animation_template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.696764 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.703808 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/bindings/
--rw-rw-r--   0 afattaholman   (502) staff       (20)     6311 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/bindings/utils.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.704801 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/
--rw-rw-r--   0 afattaholman   (502) staff       (20)    44776 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.complete.min.js
--rw-rw-r--   0 afattaholman   (502) staff       (20)     9328 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.css
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.705773 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/
--rw-rw-r--   0 afattaholman   (502) staff       (20)   225666 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.css
--rw-rw-r--   0 afattaholman   (502) staff       (20)   895821 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.707497 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/
--rw-rw-r--   0 afattaholman   (502) staff       (20)   220163 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.css
--rw-rw-r--   0 afattaholman   (502) staff       (20)   468813 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
--rw-rw-r--   0 afattaholman   (502) staff       (20)    25032 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.709106 fattaholmanan-pyvis-1.0.1/pyvis/tests/
--rw-rw-r--   0 afattaholman   (502) staff       (20)        0 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/__init__.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)    11835 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/test_graph.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     8816 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/test_html.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     1744 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/test_me.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)      380 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/utils.py
--rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 12:56:59.710344 fattaholmanan-pyvis-1.0.1/setup.cfg
--rw-rw-r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 12:54:03.000000 fattaholmanan-pyvis-1.0.1/setup.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.228414 fattaholmanan-pyvis-1.0.2/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1533 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/LICENSE_BSD.txt
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       66 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/MANIFEST.in
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 13:56:52.227879 fattaholmanan-pyvis-1.0.2/PKG-INFO
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1270 2024-04-04 12:55:09.000000 fattaholmanan-pyvis-1.0.2/README.md
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.227511 fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 13:56:52.000000 fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/PKG-INFO
+-rw-r--r--   0 afattaholman   (502) staff       (20)      890 2024-04-04 13:56:52.000000 fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/SOURCES.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 13:56:52.000000 fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/dependency_links.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 13:56:52.000000 fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/requires.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 13:56:52.000000 fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/top_level.txt
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.221116 fattaholmanan-pyvis-1.0.2/pyvis/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       56 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/__init__.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 13:51:17.000000 fattaholmanan-pyvis-1.0.2/pyvis/_version.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      292 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/edge.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)    39124 2024-04-04 13:50:47.000000 fattaholmanan-pyvis-1.0.2/pyvis/network.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      310 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/node.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     7782 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/options.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     4086 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/physics.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.221789 fattaholmanan-pyvis-1.0.2/pyvis/templates/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     3188 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/animation_template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.215317 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.222123 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/bindings/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     6311 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/bindings/utils.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.222913 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/tom-select/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    44776 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/tom-select/tom-select.complete.min.js
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     9328 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/tom-select/tom-select.css
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.223882 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.0.4/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   225666 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.0.4/vis-network.css
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   895821 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.225235 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.1.2/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   220163 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.1.2/vis-network.css
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   468813 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    25032 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/templates/template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 13:56:52.227124 fattaholmanan-pyvis-1.0.2/pyvis/tests/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)        0 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/tests/__init__.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)    11835 2024-04-04 13:33:37.000000 fattaholmanan-pyvis-1.0.2/pyvis/tests/test_graph.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     8816 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/tests/test_html.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1744 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/tests/test_me.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      380 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.2/pyvis/utils.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 13:56:52.228480 fattaholmanan-pyvis-1.0.2/setup.cfg
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 12:54:03.000000 fattaholmanan-pyvis-1.0.2/setup.py
```

### Comparing `fattaholmanan-pyvis-1.0.1/LICENSE_BSD.txt` & `fattaholmanan-pyvis-1.0.2/LICENSE_BSD.txt`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/PKG-INFO` & `fattaholmanan-pyvis-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fattaholmanan-pyvis
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python network graph visualization library
 Home-page: https://github.com/fattaholmanan/pyvis
 Author: Ali Fattaholmanan
 Author-email: alii.fattah@gmail.com
 License: BSD
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `fattaholmanan-pyvis-1.0.1/README.md` & `fattaholmanan-pyvis-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/PKG-INFO` & `fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fattaholmanan-pyvis
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python network graph visualization library
 Home-page: https://github.com/fattaholmanan/pyvis
 Author: Ali Fattaholmanan
 Author-email: alii.fattah@gmail.com
 License: BSD
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/SOURCES.txt` & `fattaholmanan-pyvis-1.0.2/fattaholmanan_pyvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/network.py` & `fattaholmanan-pyvis-1.0.2/pyvis/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         :type bgcolor: str
         :type font_color: str
         :type layout: bool
         :type cdn_resources: str
         """
         self.nodes = []
         self.edges = []
+        self.edges_lookup = {}
         self.height = height
         self.width = width
         self.heading = heading
         self.html = ""
         self.shape = "dot"
         self.font_color = font_color
         self.directed = directed
@@ -307,15 +308,15 @@
         """
         Return number of edges
 
         :returns: :py:class:`int`
         """
         return len(self.edges)
 
-    def add_edge(self, source, to, check_duplicates=True, **options):
+    def add_edge(self, source, to, **options):
         """
 
         Adding edges is done based off of the IDs of the nodes. Order does
         not matter unless dealing with a directed graph.
 
         >>> nt.add_edge(0, 1) # adds an edge from node ID 0 to node ID
         >>> nt.add_edge(0, 1, value = 4) # adds an edge with a width of 4
@@ -366,28 +367,23 @@
         assert source in self.get_nodes(), \
             "non existent node '" + str(source) + "'"
 
         assert to in self.get_nodes(), \
             "non existent node '" + str(to) + "'"
 
         # we only check existing edge for undirected graphs
-        if not self.directed and check_duplicates:
-            for e in self.edges:
-                frm = e['from']
-                dest = e['to']
-                if (
-                        (source == dest and to == frm) or
-                        (source == frm and to == dest)
-                ):
-                    # edge already exists
-                    edge_exists = True
+        key = (source, to)
+        if not self.directed:
+            if key in self.edges_lookup or key[::-1] in self.edges_lookup:
+                edge_exists = True
 
         if not edge_exists:
             e = Edge(source, to, self.directed, **options)
             self.edges.append(e.options)
+            self.edges_lookup[key] = e
 
     def add_edges(self, edges):
         """
         This method serves to add multiple edges between existing nodes
         in the network instance. Adding of the edges is done based off
         of the IDs of the nodes. Order does not matter unless dealing with a
         directed graph.
```

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/options.py` & `fattaholmanan-pyvis-1.0.2/pyvis/options.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/physics.py` & `fattaholmanan-pyvis-1.0.2/pyvis/physics.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/animation_template.html` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/animation_template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/bindings/utils.js` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/bindings/utils.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.complete.min.js` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/tom-select/tom-select.complete.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.css` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/tom-select/tom-select.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.css` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.0.4/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.min.js` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.0.4/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.css` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.1.2/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.min.js` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/lib/vis-9.1.2/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/templates/template.html` & `fattaholmanan-pyvis-1.0.2/pyvis/templates/template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/tests/test_graph.py` & `fattaholmanan-pyvis-1.0.2/pyvis/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/tests/test_html.py` & `fattaholmanan-pyvis-1.0.2/pyvis/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/pyvis/tests/test_me.py` & `fattaholmanan-pyvis-1.0.2/pyvis/tests/test_me.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.1/setup.py` & `fattaholmanan-pyvis-1.0.2/setup.py`

 * *Files identical despite different names*

