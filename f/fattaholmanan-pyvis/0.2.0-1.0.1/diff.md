# Comparing `tmp/fattaholmanan-pyvis-0.2.0.tar.gz` & `tmp/fattaholmanan-pyvis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fattaholmanan-pyvis-0.2.0.tar", last modified: Thu Apr  4 11:43:13 2024, max compression
+gzip compressed data, was "fattaholmanan-pyvis-1.0.1.tar", last modified: Thu Apr  4 12:56:59 2024, max compression
```

## Comparing `fattaholmanan-pyvis-0.2.0.tar` & `fattaholmanan-pyvis-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,42 @@
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.295975 fattaholmanan-pyvis-0.2.0/
--rw-r--r--   0 afattaholman   (502) staff       (20)     1533 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/LICENSE_BSD.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)       66 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/MANIFEST.in
--rw-r--r--   0 afattaholman   (502) staff       (20)     1611 2024-04-04 11:43:13.295761 fattaholmanan-pyvis-0.2.0/PKG-INFO
--rw-r--r--   0 afattaholman   (502) staff       (20)     1256 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/README.md
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.280949 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/
--rw-r--r--   0 afattaholman   (502) staff       (20)     1611 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/PKG-INFO
--rw-r--r--   0 afattaholman   (502) staff       (20)     1152 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/SOURCES.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/dependency_links.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/requires.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/top_level.txt
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.284044 fattaholmanan-pyvis-0.2.0/pyvis/
--rw-r--r--   0 afattaholman   (502) staff       (20)       56 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/__init__.py
--rw-r--r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/_version.py
--rw-r--r--   0 afattaholman   (502) staff       (20)      292 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/edge.py
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.277565 fattaholmanan-pyvis-0.2.0/pyvis/lib/
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.284738 fattaholmanan-pyvis-0.2.0/pyvis/lib/bindings/
--rw-r--r--   0 afattaholman   (502) staff       (20)     6311 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/bindings/utils.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.285685 fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/
--rw-r--r--   0 afattaholman   (502) staff       (20)    44776 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.complete.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)     9328 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.css
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.287132 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/
--rw-r--r--   0 afattaholman   (502) staff       (20)   225666 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   895821 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.min.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.289064 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/
--rw-r--r--   0 afattaholman   (502) staff       (20)   220163 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   468813 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)    39677 2024-04-04 11:40:09.000000 fattaholmanan-pyvis-0.2.0/pyvis/network.py
--rw-r--r--   0 afattaholman   (502) staff       (20)      310 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/node.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     7782 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/options.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     4086 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/physics.py
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.290171 fattaholmanan-pyvis-0.2.0/pyvis/templates/
--rw-r--r--   0 afattaholman   (502) staff       (20)     3188 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/animation_template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.278458 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.290713 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/bindings/
--rw-r--r--   0 afattaholman   (502) staff       (20)     6311 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/bindings/utils.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.291411 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/
--rw-r--r--   0 afattaholman   (502) staff       (20)    44776 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/tom-select.complete.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)     9328 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/tom-select.css
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.292368 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/
--rw-r--r--   0 afattaholman   (502) staff       (20)   225666 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   895821 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.293637 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/
--rw-r--r--   0 afattaholman   (502) staff       (20)   220163 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   468813 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)    25032 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.295452 fattaholmanan-pyvis-0.2.0/pyvis/tests/
--rw-r--r--   0 afattaholman   (502) staff       (20)        0 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/__init__.py
--rw-r--r--   0 afattaholman   (502) staff       (20)    11835 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/test_graph.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     8816 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/test_html.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     1744 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/test_me.py
--rw-r--r--   0 afattaholman   (502) staff       (20)      380 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/utils.py
--rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 11:43:13.296025 fattaholmanan-pyvis-0.2.0/setup.cfg
--rw-r--r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 11:40:40.000000 fattaholmanan-pyvis-0.2.0/setup.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.710292 fattaholmanan-pyvis-1.0.1/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1533 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/LICENSE_BSD.txt
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       66 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/MANIFEST.in
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 12:56:59.709907 fattaholmanan-pyvis-1.0.1/PKG-INFO
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1270 2024-04-04 12:55:09.000000 fattaholmanan-pyvis-1.0.1/README.md
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.709516 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/PKG-INFO
+-rw-r--r--   0 afattaholman   (502) staff       (20)      890 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/SOURCES.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/dependency_links.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/requires.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 12:56:59.000000 fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/top_level.txt
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.702745 fattaholmanan-pyvis-1.0.1/pyvis/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       56 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/__init__.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 12:53:38.000000 fattaholmanan-pyvis-1.0.1/pyvis/_version.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      292 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/edge.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    39291 2024-04-04 12:54:44.000000 fattaholmanan-pyvis-1.0.1/pyvis/network.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      310 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/node.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     7782 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/options.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     4086 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/physics.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.703455 fattaholmanan-pyvis-1.0.1/pyvis/templates/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     3188 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/animation_template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.696764 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.703808 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/bindings/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     6311 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/bindings/utils.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.704801 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    44776 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.complete.min.js
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     9328 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.css
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.705773 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   225666 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.css
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   895821 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.707497 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   220163 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.css
+-rw-rw-r--   0 afattaholman   (502) staff       (20)   468813 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    25032 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/templates/template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:56:59.709106 fattaholmanan-pyvis-1.0.1/pyvis/tests/
+-rw-rw-r--   0 afattaholman   (502) staff       (20)        0 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/__init__.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)    11835 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/test_graph.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     8816 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/test_html.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)     1744 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/tests/test_me.py
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      380 2022-11-04 20:39:15.000000 fattaholmanan-pyvis-1.0.1/pyvis/utils.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 12:56:59.710344 fattaholmanan-pyvis-1.0.1/setup.cfg
+-rw-rw-r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 12:54:03.000000 fattaholmanan-pyvis-1.0.1/setup.py
```

### Comparing `fattaholmanan-pyvis-0.2.0/LICENSE_BSD.txt` & `fattaholmanan-pyvis-1.0.1/LICENSE_BSD.txt`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/PKG-INFO` & `fattaholmanan-pyvis-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-Metadata-Version: 2.1
-Name: fattaholmanan-pyvis
-Version: 0.2.0
-Summary: A Python network graph visualization library
-Home-page: https://github.com/fattaholmanan/pyvis
-Author: Ali Fattaholmanan
-Author-email: alii.fattah@gmail.com
-License: BSD
-Platform: UNKNOWN
-Requires-Python: >3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE_BSD.txt
-
 ## Pyvis - a Python library for visualizing networks
 
 ![](pyvis/source/tut.gif?raw=true)
 
 ## Description
 Pyvis is built around [visjs](http://visjs.org/), a JavaScript visualization library.
 
 ## Documentation
 Pyvis' full documentation can be found at http://pyvis.readthedocs.io/en/latest/
 ## Installation
 You can install pyvis through pip:
 
 ```bash
-pip install pyvis
+pip install fattaholmanan-pyvis
 ```
 Or if you have an archive of the project simply run the following from the top level directory:
 
 ```bash
 python setup.py install
 ```
 
@@ -56,9 +43,7 @@
 g.add_node(1)
 g.add_edge(0, 1)
 g.show("basic.html")
 ```
 
 ## Interactive Notebook playground with examples
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/WestHealth/pyvis/master?filepath=notebooks%2Fexample.ipynb)
-
-
```

### Comparing `fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/PKG-INFO` & `fattaholmanan-pyvis-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: fattaholmanan-pyvis
-Version: 0.2.0
+Version: 1.0.1
 Summary: A Python network graph visualization library
 Home-page: https://github.com/fattaholmanan/pyvis
 Author: Ali Fattaholmanan
 Author-email: alii.fattah@gmail.com
 License: BSD
-Platform: UNKNOWN
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE_BSD.txt
+Requires-Dist: jinja2>=2.9.6
+Requires-Dist: networkx>=1.11
+Requires-Dist: ipython>=5.3.0
+Requires-Dist: jsonpickle>=1.4.1
 
 ## Pyvis - a Python library for visualizing networks
 
 ![](pyvis/source/tut.gif?raw=true)
 
 ## Description
 Pyvis is built around [visjs](http://visjs.org/), a JavaScript visualization library.
 
 ## Documentation
 Pyvis' full documentation can be found at http://pyvis.readthedocs.io/en/latest/
 ## Installation
 You can install pyvis through pip:
 
 ```bash
-pip install pyvis
+pip install fattaholmanan-pyvis
 ```
 Or if you have an archive of the project simply run the following from the top level directory:
 
 ```bash
 python setup.py install
 ```
 
@@ -56,9 +59,7 @@
 g.add_node(1)
 g.add_edge(0, 1)
 g.show("basic.html")
 ```
 
 ## Interactive Notebook playground with examples
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/WestHealth/pyvis/master?filepath=notebooks%2Fexample.ipynb)
-
-
```

### Comparing `fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/SOURCES.txt` & `fattaholmanan-pyvis-1.0.1/fattaholmanan_pyvis.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,14 @@
 pyvis/_version.py
 pyvis/edge.py
 pyvis/network.py
 pyvis/node.py
 pyvis/options.py
 pyvis/physics.py
 pyvis/utils.py
-pyvis/lib/bindings/utils.js
-pyvis/lib/tom-select/tom-select.complete.min.js
-pyvis/lib/tom-select/tom-select.css
-pyvis/lib/vis-9.0.4/vis-network.css
-pyvis/lib/vis-9.0.4/vis-network.min.js
-pyvis/lib/vis-9.1.2/vis-network.css
-pyvis/lib/vis-9.1.2/vis-network.min.js
 pyvis/templates/animation_template.html
 pyvis/templates/template.html
 pyvis/templates/lib/bindings/utils.js
 pyvis/templates/lib/tom-select/tom-select.complete.min.js
 pyvis/templates/lib/tom-select/tom-select.css
 pyvis/templates/lib/vis-9.0.4/vis-network.css
 pyvis/templates/lib/vis-9.0.4/vis-network.min.js
```

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/lib/bindings/utils.js` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/bindings/utils.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.complete.min.js` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.complete.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.css` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/tom-select/tom-select.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.css` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.min.js` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.0.4/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.css` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.min.js` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/lib/vis-9.1.2/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/network.py` & `fattaholmanan-pyvis-1.0.1/pyvis/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,27 +81,24 @@
         self.dot_lang = ""
         self.options = Options(layout)
         self.widget = False
         self.node_ids = []
         self.node_map = {}
         self.template = None
         self.conf = False
+        self.path = "template.html"  # os.path.dirname(__file__) + "/templates/
         self.neighborhood_highlight = neighborhood_highlight
         self.select_menu = select_menu
         self.filter_menu = filter_menu
         assert cdn_resources in ["local", "in_line", "remote"], "cdn_resources not in [local, in_line, remote]."
-        # path is the root template located in the template_dir
-        self.path = "template.html"
         self.template_dir = os.path.dirname(__file__) + "/templates/"
         self.templateEnv = Environment(loader=FileSystemLoader(self.template_dir))
 
         if cdn_resources == "local" and notebook == True:
-            print("Warning: When  cdn_resources is 'local' jupyter notebook has issues displaying graphics on chrome/safari."
-                  " Use cdn_resources='in_line' or cdn_resources='remote' if you have issues "
-                  "viewing graphics in a notebook.")
+            print("Local cdn resources have problems on chrome/safari when used in jupyter-notebook. ")
         self.cdn_resources = cdn_resources
 
         if notebook:
             self.prep_notebook()
 
     def __str__(self):
         """
@@ -493,65 +490,70 @@
                                     select_menu=self.select_menu,
                                     filter_menu=self.filter_menu,
                                     notebook=notebook,
                                     cdn_resources=self.cdn_resources
                                     )
         return self.html
 
-    def write_html(self, name, local=True, notebook=False,open_browser=False):
+    def write_html(self, name, local=True, notebook=False):
         """
         This method gets the data structures supporting the nodes, edges,
         and options and updates the template to write the HTML holding
         the visualization.
-
-        To work with the old local methods local is being depricated, but not removed.
         :type name_html: str
-        @param name: name of the file to save the graph as.
-        @param local: Depricated parameter. Used to be used to determine how the graph needs deploy. Has been removed in favor of using the class cdn_resources instead.
-        @param notebook: If true, this object will return the iframe document for use in juptyer notebook.
-        @param open_browser: If true, will open a web browser with the generated graph.
         """
-        getcwd_name = name
-        check_html(getcwd_name)
+        check_html(name)
         self.html = self.generate_html(notebook=notebook)
 
-        if self.cdn_resources == "local":
+        with open(name, "w+") as out:
+            out.write(self.html)
+
+        if notebook:
+            with open(name, "w+") as out:
+                out.write(self.html)
+            return IFrame(name, width=self.width, height=self.height)
+        elif notebook and local:
             if not os.path.exists("lib"):
-                os.makedirs("lib")
+                os.makedirs(os.path.dirname("lib"))
             if not os.path.exists("lib/bindings"):
                 shutil.copytree(f"{os.path.dirname(__file__)}/templates/lib/bindings", "lib/bindings")
-            if not os.path.exists(os.getcwd()+"/lib/tom-select"):
+            if not os.path.exists("lib/tom-select"):
                 shutil.copytree(f"{os.path.dirname(__file__)}/templates/lib/tom-select", "lib/tom-select")
-            if not os.path.exists(os.getcwd()+"/lib/vis-9.1.2"):
+            if not os.path.exists("lib/bindings"):
                 shutil.copytree(f"{os.path.dirname(__file__)}/templates/lib/vis-9.1.2", "lib/vis-9.1.2")
-            with open(getcwd_name, "w+") as out:
-                out.write(self.html)
-        elif self.cdn_resources == "in_line" or self.cdn_resources == "remote":
-            with open(getcwd_name, "w+") as out:
+            with open(name, "w+") as out:
                 out.write(self.html)
+            return IFrame(name, width=self.width, height=self.height)
         else:
-            assert "cdn_resources is not in ['in_line','remote','local']."
-        if open_browser: # open the saved file in a new browser window.
-            webbrowser.open(getcwd_name)
+            if local:
+                tempdir = "."
+            else:
+                tempdir = tempfile.mkdtemp()
+            # with tempfile.mkdtemp() as tempdir:
+            if os.path.exists(f"{tempdir}/lib"):
+                shutil.rmtree(f"{tempdir}/lib")
+            shutil.copytree(f"{os.path.dirname(__file__)}/templates/lib", f"{tempdir}/lib")
 
+            with open(f"{tempdir}/{name}", "w+") as out:
+                out.write(self.html)
+                webbrowser.open(f"{tempdir}/{name}")
 
-    def show(self, name, local=True,notebook=True):
+    def show(self, name, local=True):
         """
         Writes a static HTML file and saves it locally before opening.
 
         :param: name: the name of the html file to save as
         :type name: str
         """
-        print(name)
-        if notebook:
-            self.write_html(name, open_browser=False,notebook=True)
+        check_html(name)
+        if self.template is not None:
+            return self.write_html(name, local, notebook=True)
         else:
-            self.write_html(name, open_browser=True)
-        if notebook:
-            return IFrame(name, width=self.width, height=self.height)
+            self.write_html(name, local)
+            # webbrowser.open(name)
 
     def prep_notebook(self,
                       custom_template=False, custom_template_path=None):
         """
         Loads the template data into the template attribute of the network.
         This should be done in a jupyter notebook environment before showing
         the network.
```

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/options.py` & `fattaholmanan-pyvis-1.0.1/pyvis/options.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/physics.py` & `fattaholmanan-pyvis-1.0.1/pyvis/physics.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/templates/animation_template.html` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/animation_template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/templates/template.html` & `fattaholmanan-pyvis-1.0.1/pyvis/templates/template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/tests/test_graph.py` & `fattaholmanan-pyvis-1.0.1/pyvis/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/tests/test_html.py` & `fattaholmanan-pyvis-1.0.1/pyvis/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/pyvis/tests/test_me.py` & `fattaholmanan-pyvis-1.0.1/pyvis/tests/test_me.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.2.0/setup.py` & `fattaholmanan-pyvis-1.0.1/setup.py`

 * *Files identical despite different names*

