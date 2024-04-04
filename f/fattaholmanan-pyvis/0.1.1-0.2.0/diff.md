# Comparing `tmp/fattaholmanan-pyvis-0.1.1.tar.gz` & `tmp/fattaholmanan-pyvis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fattaholmanan-pyvis-0.1.1.tar", last modified: Thu Apr  4 12:40:39 2024, max compression
+gzip compressed data, was "fattaholmanan-pyvis-0.2.0.tar", last modified: Thu Apr  4 11:43:13 2024, max compression
```

## Comparing `fattaholmanan-pyvis-0.1.1.tar` & `fattaholmanan-pyvis-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.602320 fattaholmanan-pyvis-0.1.1/
--rw-r--r--   0 afattaholman   (502) staff       (20)     1533 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/LICENSE_BSD.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)       66 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/MANIFEST.in
--rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 12:40:39.601904 fattaholmanan-pyvis-0.1.1/PKG-INFO
--rw-r--r--   0 afattaholman   (502) staff       (20)     1270 2024-04-04 12:01:42.000000 fattaholmanan-pyvis-0.1.1/README.md
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.599054 fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/
--rw-r--r--   0 afattaholman   (502) staff       (20)     1727 2024-04-04 12:40:39.000000 fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/PKG-INFO
--rw-r--r--   0 afattaholman   (502) staff       (20)     1152 2024-04-04 12:40:39.000000 fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/SOURCES.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 12:40:39.000000 fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/dependency_links.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 12:40:39.000000 fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/requires.txt
--rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 12:40:39.000000 fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/top_level.txt
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.587612 fattaholmanan-pyvis-0.1.1/pyvis/
--rw-r--r--   0 afattaholman   (502) staff       (20)       56 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/__init__.py
--rw-r--r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 12:40:25.000000 fattaholmanan-pyvis-0.1.1/pyvis/_version.py
--rw-r--r--   0 afattaholman   (502) staff       (20)      292 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/edge.py
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.581486 fattaholmanan-pyvis-0.1.1/pyvis/lib/
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.587918 fattaholmanan-pyvis-0.1.1/pyvis/lib/bindings/
--rw-r--r--   0 afattaholman   (502) staff       (20)     6311 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/lib/bindings/utils.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.588650 fattaholmanan-pyvis-0.1.1/pyvis/lib/tom-select/
--rw-r--r--   0 afattaholman   (502) staff       (20)    44776 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/lib/tom-select/tom-select.complete.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)     9328 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/lib/tom-select/tom-select.css
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.589530 fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.0.4/
--rw-r--r--   0 afattaholman   (502) staff       (20)   225666 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.0.4/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   895821 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.0.4/vis-network.min.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.591156 fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.1.2/
--rw-r--r--   0 afattaholman   (502) staff       (20)   220163 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.1.2/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   468813 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.1.2/vis-network.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)    39677 2024-04-04 11:40:09.000000 fattaholmanan-pyvis-0.1.1/pyvis/network.py
--rw-r--r--   0 afattaholman   (502) staff       (20)      310 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/node.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     7782 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/options.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     4086 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/physics.py
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.592210 fattaholmanan-pyvis-0.1.1/pyvis/templates/
--rw-r--r--   0 afattaholman   (502) staff       (20)     3188 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/animation_template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.582534 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.592569 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/bindings/
--rw-r--r--   0 afattaholman   (502) staff       (20)     6311 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/bindings/utils.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.595062 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/tom-select/
--rw-r--r--   0 afattaholman   (502) staff       (20)    44776 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/tom-select/tom-select.complete.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)     9328 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/tom-select/tom-select.css
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.595853 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.0.4/
--rw-r--r--   0 afattaholman   (502) staff       (20)   225666 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.0.4/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   895821 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.596978 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.1.2/
--rw-r--r--   0 afattaholman   (502) staff       (20)   220163 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.1.2/vis-network.css
--rw-r--r--   0 afattaholman   (502) staff       (20)   468813 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
--rw-r--r--   0 afattaholman   (502) staff       (20)    25032 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/templates/template.html
-drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 12:40:39.598688 fattaholmanan-pyvis-0.1.1/pyvis/tests/
--rw-r--r--   0 afattaholman   (502) staff       (20)        0 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/tests/__init__.py
--rw-r--r--   0 afattaholman   (502) staff       (20)    11835 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/tests/test_graph.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     8816 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/tests/test_html.py
--rw-r--r--   0 afattaholman   (502) staff       (20)     1744 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/tests/test_me.py
--rw-r--r--   0 afattaholman   (502) staff       (20)      380 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.1.1/pyvis/utils.py
--rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 12:40:39.602379 fattaholmanan-pyvis-0.1.1/setup.cfg
--rw-r--r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 12:40:01.000000 fattaholmanan-pyvis-0.1.1/setup.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.295975 fattaholmanan-pyvis-0.2.0/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1533 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/LICENSE_BSD.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)       66 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/MANIFEST.in
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1611 2024-04-04 11:43:13.295761 fattaholmanan-pyvis-0.2.0/PKG-INFO
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1256 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/README.md
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.280949 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1611 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/PKG-INFO
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1152 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/SOURCES.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        1 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/dependency_links.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)       62 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/requires.txt
+-rw-r--r--   0 afattaholman   (502) staff       (20)        6 2024-04-04 11:43:13.000000 fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/top_level.txt
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.284044 fattaholmanan-pyvis-0.2.0/pyvis/
+-rw-r--r--   0 afattaholman   (502) staff       (20)       56 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/__init__.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)       37 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/_version.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)      292 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/edge.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.277565 fattaholmanan-pyvis-0.2.0/pyvis/lib/
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.284738 fattaholmanan-pyvis-0.2.0/pyvis/lib/bindings/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     6311 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/bindings/utils.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.285685 fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/
+-rw-r--r--   0 afattaholman   (502) staff       (20)    44776 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.complete.min.js
+-rw-r--r--   0 afattaholman   (502) staff       (20)     9328 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.css
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.287132 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/
+-rw-r--r--   0 afattaholman   (502) staff       (20)   225666 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.css
+-rw-r--r--   0 afattaholman   (502) staff       (20)   895821 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.min.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.289064 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/
+-rw-r--r--   0 afattaholman   (502) staff       (20)   220163 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.css
+-rw-r--r--   0 afattaholman   (502) staff       (20)   468813 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.min.js
+-rw-r--r--   0 afattaholman   (502) staff       (20)    39677 2024-04-04 11:40:09.000000 fattaholmanan-pyvis-0.2.0/pyvis/network.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)      310 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/node.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)     7782 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/options.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)     4086 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/physics.py
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.290171 fattaholmanan-pyvis-0.2.0/pyvis/templates/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     3188 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/animation_template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.278458 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.290713 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/bindings/
+-rw-r--r--   0 afattaholman   (502) staff       (20)     6311 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/bindings/utils.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.291411 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/
+-rw-r--r--   0 afattaholman   (502) staff       (20)    44776 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/tom-select.complete.min.js
+-rw-r--r--   0 afattaholman   (502) staff       (20)     9328 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/tom-select.css
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.292368 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/
+-rw-r--r--   0 afattaholman   (502) staff       (20)   225666 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/vis-network.css
+-rw-r--r--   0 afattaholman   (502) staff       (20)   895821 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/vis-network.min.js
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.293637 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/
+-rw-r--r--   0 afattaholman   (502) staff       (20)   220163 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/vis-network.css
+-rw-r--r--   0 afattaholman   (502) staff       (20)   468813 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/vis-network.min.js
+-rw-r--r--   0 afattaholman   (502) staff       (20)    25032 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/templates/template.html
+drwxr-xr-x   0 afattaholman   (502) staff       (20)        0 2024-04-04 11:43:13.295452 fattaholmanan-pyvis-0.2.0/pyvis/tests/
+-rw-r--r--   0 afattaholman   (502) staff       (20)        0 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/__init__.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)    11835 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/test_graph.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)     8816 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/test_html.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)     1744 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/tests/test_me.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)      380 2024-04-04 08:25:54.000000 fattaholmanan-pyvis-0.2.0/pyvis/utils.py
+-rw-r--r--   0 afattaholman   (502) staff       (20)       38 2024-04-04 11:43:13.296025 fattaholmanan-pyvis-0.2.0/setup.cfg
+-rw-r--r--   0 afattaholman   (502) staff       (20)      766 2024-04-04 11:40:40.000000 fattaholmanan-pyvis-0.2.0/setup.py
```

### Comparing `fattaholmanan-pyvis-0.1.1/LICENSE_BSD.txt` & `fattaholmanan-pyvis-0.2.0/LICENSE_BSD.txt`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/PKG-INFO` & `fattaholmanan-pyvis-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: fattaholmanan-pyvis
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python network graph visualization library
 Home-page: https://github.com/fattaholmanan/pyvis
 Author: Ali Fattaholmanan
 Author-email: alii.fattah@gmail.com
 License: BSD
+Platform: UNKNOWN
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE_BSD.txt
-Requires-Dist: jinja2>=2.9.6
-Requires-Dist: networkx>=1.11
-Requires-Dist: ipython>=5.3.0
-Requires-Dist: jsonpickle>=1.4.1
 
 ## Pyvis - a Python library for visualizing networks
 
 ![](pyvis/source/tut.gif?raw=true)
 
 ## Description
 Pyvis is built around [visjs](http://visjs.org/), a JavaScript visualization library.
 
 ## Documentation
 Pyvis' full documentation can be found at http://pyvis.readthedocs.io/en/latest/
 ## Installation
 You can install pyvis through pip:
 
 ```bash
-pip install fattaholmanan-pyvis
+pip install pyvis
 ```
 Or if you have an archive of the project simply run the following from the top level directory:
 
 ```bash
 python setup.py install
 ```
 
@@ -59,7 +56,9 @@
 g.add_node(1)
 g.add_edge(0, 1)
 g.show("basic.html")
 ```
 
 ## Interactive Notebook playground with examples
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/WestHealth/pyvis/master?filepath=notebooks%2Fexample.ipynb)
+
+
```

### Comparing `fattaholmanan-pyvis-0.1.1/README.md` & `fattaholmanan-pyvis-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 ## Documentation
 Pyvis' full documentation can be found at http://pyvis.readthedocs.io/en/latest/
 ## Installation
 You can install pyvis through pip:
 
 ```bash
-pip install fattaholmanan-pyvis
+pip install pyvis
 ```
 Or if you have an archive of the project simply run the following from the top level directory:
 
 ```bash
 python setup.py install
 ```
```

### Comparing `fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/PKG-INFO` & `fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: fattaholmanan-pyvis
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python network graph visualization library
 Home-page: https://github.com/fattaholmanan/pyvis
 Author: Ali Fattaholmanan
 Author-email: alii.fattah@gmail.com
 License: BSD
+Platform: UNKNOWN
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE_BSD.txt
-Requires-Dist: jinja2>=2.9.6
-Requires-Dist: networkx>=1.11
-Requires-Dist: ipython>=5.3.0
-Requires-Dist: jsonpickle>=1.4.1
 
 ## Pyvis - a Python library for visualizing networks
 
 ![](pyvis/source/tut.gif?raw=true)
 
 ## Description
 Pyvis is built around [visjs](http://visjs.org/), a JavaScript visualization library.
 
 ## Documentation
 Pyvis' full documentation can be found at http://pyvis.readthedocs.io/en/latest/
 ## Installation
 You can install pyvis through pip:
 
 ```bash
-pip install fattaholmanan-pyvis
+pip install pyvis
 ```
 Or if you have an archive of the project simply run the following from the top level directory:
 
 ```bash
 python setup.py install
 ```
 
@@ -59,7 +56,9 @@
 g.add_node(1)
 g.add_edge(0, 1)
 g.show("basic.html")
 ```
 
 ## Interactive Notebook playground with examples
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/WestHealth/pyvis/master?filepath=notebooks%2Fexample.ipynb)
+
+
```

### Comparing `fattaholmanan-pyvis-0.1.1/fattaholmanan_pyvis.egg-info/SOURCES.txt` & `fattaholmanan-pyvis-0.2.0/fattaholmanan_pyvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/lib/bindings/utils.js` & `fattaholmanan-pyvis-0.2.0/pyvis/lib/bindings/utils.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/lib/tom-select/tom-select.complete.min.js` & `fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.complete.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/lib/tom-select/tom-select.css` & `fattaholmanan-pyvis-0.2.0/pyvis/lib/tom-select/tom-select.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.0.4/vis-network.css` & `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.0.4/vis-network.min.js` & `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.0.4/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.1.2/vis-network.css` & `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/lib/vis-9.1.2/vis-network.min.js` & `fattaholmanan-pyvis-0.2.0/pyvis/lib/vis-9.1.2/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/network.py` & `fattaholmanan-pyvis-0.2.0/pyvis/network.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/options.py` & `fattaholmanan-pyvis-0.2.0/pyvis/options.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/physics.py` & `fattaholmanan-pyvis-0.2.0/pyvis/physics.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/animation_template.html` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/animation_template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/bindings/utils.js` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/bindings/utils.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/tom-select/tom-select.complete.min.js` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/tom-select.complete.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/tom-select/tom-select.css` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/tom-select/tom-select.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.0.4/vis-network.css` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.0.4/vis-network.min.js` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.0.4/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.1.2/vis-network.css` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/vis-network.css`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/lib/vis-9.1.2/vis-network.min.js` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/lib/vis-9.1.2/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/templates/template.html` & `fattaholmanan-pyvis-0.2.0/pyvis/templates/template.html`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/tests/test_graph.py` & `fattaholmanan-pyvis-0.2.0/pyvis/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/tests/test_html.py` & `fattaholmanan-pyvis-0.2.0/pyvis/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/pyvis/tests/test_me.py` & `fattaholmanan-pyvis-0.2.0/pyvis/tests/test_me.py`

 * *Files identical despite different names*

### Comparing `fattaholmanan-pyvis-0.1.1/setup.py` & `fattaholmanan-pyvis-0.2.0/setup.py`

 * *Files identical despite different names*

