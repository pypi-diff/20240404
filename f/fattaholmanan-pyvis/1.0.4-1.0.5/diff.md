# Comparing `tmp/fattaholmanan-pyvis-1.0.4.tar.gz` & `tmp/fattaholmanan-pyvis-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fattaholmanan-pyvis-1.0.4.tar", last modified: Thu Apr  4 14:30:08 2024, max compression
+gzip compressed data, was "fattaholmanan-pyvis-1.0.5.tar", last modified: Thu Apr  4 14:32:29 2024, max compression
```

## Comparing `fattaholmanan-pyvis-1.0.4.tar` & `fattaholmanan-pyvis-1.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.425966 fattaholmanan-pyvis-1.0.4/
--rw-rw-r--   0 afattaholman   (502) staff       (20)     1533 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/LICENSE_BSD.txt
--rw-rw-r--   0 afattaholman   (502) staff       (20)       66 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/MANIFEST.in
--rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 14:30:08.425433 fattaholmanan-pyvis-1.0.4/PKG-INFO
--rw-rw-r--   0 afattaholman   (502) staff       (20)     1270 2024-04-04 12:55:09.000000 fattaholmanan-pyvis-1.0.4/README.md
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.425070 fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/
--rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 14:30:08.000000 fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/PKG-INFO
--rw-r--r--   0 afattaholman   (502) staff       (20)      890 2024-04-04 14:30:08.000000 fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/SOURCES.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 14:30:08.000000 fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/dependency_links.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 14:30:08.000000 fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/requires.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 14:30:08.000000 fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/top_level.txt
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.418497 fattaholmanan-pyvis-1.0.4/pyvis/
--rw-rw-r--   0 afattaholman   (502) staff       (20)       56 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/__init__.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 14:29:28.000000 fattaholmanan-pyvis-1.0.4/pyvis/_version.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)      292 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/edge.py
--rw-r--r--   0 afattaholman   (502) staff       (20)    39208 2024-04-04 14:29:21.000000 fattaholmanan-pyvis-1.0.4/pyvis/network.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)      310 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/node.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     7782 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/options.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     4086 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/physics.py
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.419157 fattaholmanan-pyvis-1.0.4/pyvis/templates/
--rw-rw-r--   0 afattaholman   (502) staff       (20)     3188 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/animation_template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.412646 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.419518 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/bindings/
--rw-rw-r--   0 afattaholman   (502) staff       (20)     6311 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/bindings/utils.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.420484 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/tom-select/
--rw-rw-r--   0 afattaholman   (502) staff       (20)    44776 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/tom-select/tom-select.complete.min.js
--rw-rw-r--   0 afattaholman   (502) staff       (20)     9328 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/tom-select/tom-select.css
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.421423 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.0.4/
--rw-rw-r--   0 afattaholman   (502) staff       (20)   225666 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.0.4/vis-network.css
--rw-rw-r--   0 afattaholman   (502) staff       (20)   895821 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.423075 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.1.2/
--rw-rw-r--   0 afattaholman   (502) staff       (20)   220163 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.1.2/vis-network.css
--rw-rw-r--   0 afattaholman   (502) staff       (20)   468813 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
--rw-rw-r--   0 afattaholman   (502) staff       (20)    25032 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/templates/template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:30:08.424692 fattaholmanan-pyvis-1.0.4/pyvis/tests/
--rw-rw-r--   0 afattaholman   (502) staff       (20)        0 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/tests/__init__.py
--rw-r--r--   0 afattaholman   (502) staff       (20)    11835 2024-04-04 13:33:37.000000 fattaholmanan-pyvis-1.0.4/pyvis/tests/test_graph.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     8816 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/tests/test_html.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)     1744 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/tests/test_me.py
--rw-rw-r--   0 afattaholman   (502) staff       (20)      380 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.4/pyvis/utils.py
--rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 14:30:08.426022 fattaholmanan-pyvis-1.0.4/setup.cfg
--rw-rw-r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 12:54:03.000000 fattaholmanan-pyvis-1.0.4/setup.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.518636 fattaholmanan-pyvis-1.0.5/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1533 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/LICENSE_BSD.txt
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       66 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/MANIFEST.in
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 14:32:29.518211 fattaholmanan-pyvis-1.0.5/PKG-INFO
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1270 2024-04-04 12:55:09.000000 fattaholmanan-pyvis-1.0.5/README.md
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.517842 fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 14:32:29.000000 fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/PKG-INFO
+-rw-r--r--   0 afattaholman   (502) staff       (20)      890 2024-04-04 14:32:29.000000 fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/SOURCES.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 14:32:29.000000 fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/dependency_links.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 14:32:29.000000 fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/requires.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 14:32:29.000000 fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/top_level.txt
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.511143 fattaholmanan-pyvis-1.0.5/pyvis/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       56 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/__init__.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 14:31:54.000000 fattaholmanan-pyvis-1.0.5/pyvis/_version.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      292 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/edge.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)    39253 2024-04-04 14:31:49.000000 fattaholmanan-pyvis-1.0.5/pyvis/network.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      310 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/node.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     7782 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/options.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     4086 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/physics.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.511781 fattaholmanan-pyvis-1.0.5/pyvis/templates/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     3188 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/animation_template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.505604 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.512137 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/bindings/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     6311 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/bindings/utils.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.512981 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/tom-select/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    44776 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/tom-select/tom-select.complete.min.js
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     9328 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/tom-select/tom-select.css
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.514366 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.0.4/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   225666 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.0.4/vis-network.css
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   895821 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.515784 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.1.2/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   220163 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.1.2/vis-network.css
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   468813 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    25032 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/templates/template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 14:32:29.517362 fattaholmanan-pyvis-1.0.5/pyvis/tests/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)        0 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/tests/__init__.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)    11835 2024-04-04 13:33:37.000000 fattaholmanan-pyvis-1.0.5/pyvis/tests/test_graph.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     8816 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/tests/test_html.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1744 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/tests/test_me.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      380 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.5/pyvis/utils.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 14:32:29.518753 fattaholmanan-pyvis-1.0.5/setup.cfg
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 12:54:03.000000 fattaholmanan-pyvis-1.0.5/setup.py
```

### Comparing `fattaholmanan-pyvis-1.0.4/LICENSE_BSD.txt` & `fattaholmanan-pyvis-1.0.5/LICENSE_BSD.txt`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/PKG-INFO` & `fattaholmanan-pyvis-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fattaholmanan-pyvis
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python network graph visualization library
 Home-page: https://github.com/fattaholmanan/pyvis
 Author: Ali Fattaholmanan
 Author-email: alii.fattah@gmail.com
 License: BSD
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `fattaholmanan-pyvis-1.0.4/README.md` & `fattaholmanan-pyvis-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/PKG-INFO` & `fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fattaholmanan-pyvis
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python network graph visualization library
 Home-page: https://github.com/fattaholmanan/pyvis
 Author: Ali Fattaholmanan
 Author-email: alii.fattah@gmail.com
 License: BSD
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `fattaholmanan-pyvis-1.0.4/fattaholmanan_pyvis.egg-info/SOURCES.txt` & `fattaholmanan-pyvis-1.0.5/fattaholmanan_pyvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/network.py` & `fattaholmanan-pyvis-1.0.5/pyvis/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,16 @@
             if key in self.edges_lookup or key[::-1] in self.edges_lookup:
                 edge_exists = True
 
         if not edge_exists:
             e = Edge(source, to, self.directed, **options)
             self.edges.append(e.options)
             self.edges_lookup[key] = e
+            return True
+        return False
 
     def add_edges(self, edges):
         """
         This method serves to add multiple edges between existing nodes
         in the network instance. Adding of the edges is done based off
         of the IDs of the nodes. Order does not matter unless dealing with a
         directed graph.
```

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/options.py` & `fattaholmanan-pyvis-1.0.5/pyvis/options.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/physics.py` & `fattaholmanan-pyvis-1.0.5/pyvis/physics.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/animation_template.html` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/animation_template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/bindings/utils.js` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/bindings/utils.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/tom-select/tom-select.complete.min.js` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/tom-select/tom-select.complete.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/tom-select/tom-select.css` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/tom-select/tom-select.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.0.4/vis-network.css` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.0.4/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.0.4/vis-network.min.js` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.0.4/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.1.2/vis-network.css` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.1.2/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/lib/vis-9.1.2/vis-network.min.js` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/lib/vis-9.1.2/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/templates/template.html` & `fattaholmanan-pyvis-1.0.5/pyvis/templates/template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/tests/test_graph.py` & `fattaholmanan-pyvis-1.0.5/pyvis/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/tests/test_html.py` & `fattaholmanan-pyvis-1.0.5/pyvis/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/pyvis/tests/test_me.py` & `fattaholmanan-pyvis-1.0.5/pyvis/tests/test_me.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-1.0.4/setup.py` & `fattaholmanan-pyvis-1.0.5/setup.py`

 * *Files identical despite different names*

