# Comparing `tmp/GraphSL-0.1.tar.gz` & `tmp/GraphSL-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSL-0.1.tar", last modified: Thu Apr  4 02:46:00 2024, max compression
+gzip compressed data, was "GraphSL-0.1.1.tar", last modified: Thu Apr  4 04:46:32 2024, max compression
```

## Comparing `GraphSL-0.1.tar` & `GraphSL-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 02:46:00.471221 GraphSL-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-04 02:46:00.468287 GraphSL-0.1/GraphSL.egg-info/
--rw-rw-rw-   0        0        0      707 2024-04-04 02:46:00.000000 GraphSL-0.1/GraphSL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-04 02:46:00.000000 GraphSL-0.1/GraphSL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 02:46:00.000000 GraphSL-0.1/GraphSL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-04-04 02:46:00.000000 GraphSL-0.1/GraphSL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 02:46:00.000000 GraphSL-0.1/GraphSL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.1/LICENSE
--rw-rw-rw-   0        0        0      707 2024-04-04 02:46:00.472162 GraphSL-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.1/README.md
--rw-rw-rw-   0        0        0       86 2024-04-04 02:46:00.473274 GraphSL-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1893 2024-04-04 02:45:28.000000 GraphSL-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 04:46:32.183702 GraphSL-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-04 04:46:32.181707 GraphSL-0.1.1/GraphSL.egg-info/
+-rw-rw-rw-   0        0        0      709 2024-04-04 04:46:32.000000 GraphSL-0.1.1/GraphSL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-04 04:46:32.000000 GraphSL-0.1.1/GraphSL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 04:46:32.000000 GraphSL-0.1.1/GraphSL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-04 04:46:32.000000 GraphSL-0.1.1/GraphSL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 04:46:32.000000 GraphSL-0.1.1/GraphSL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      709 2024-04-04 04:46:32.184699 GraphSL-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-04 04:46:32.186103 GraphSL-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1874 2024-04-04 04:46:22.000000 GraphSL-0.1.1/setup.py
```

### Comparing `GraphSL-0.1/GraphSL.egg-info/PKG-INFO` & `GraphSL-0.1.1/GraphSL.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSL
-Version: 0.1
+Version: 0.1.1
 Summary: Graph Source Localization Approaches and Benchmark Datasets
 Home-page: https://xianggebenben.github.io/Junxiang_Wang.github.io/
 Author: Junxiang Wang
 Author-email: junxiang.wang@alumni.emory.edu
 License: MIT
 Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v_01.tar.gz
 Keywords: Graph Diffusion,Graph Source Localization,Prescribed Methods,GNN Methods,Benchmark
```

### Comparing `GraphSL-0.1/LICENSE` & `GraphSL-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GraphSL-0.1/PKG-INFO` & `GraphSL-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSL
-Version: 0.1
+Version: 0.1.1
 Summary: Graph Source Localization Approaches and Benchmark Datasets
 Home-page: https://xianggebenben.github.io/Junxiang_Wang.github.io/
 Author: Junxiang Wang
 Author-email: junxiang.wang@alumni.emory.edu
 License: MIT
 Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v_01.tar.gz
 Keywords: Graph Diffusion,Graph Source Localization,Prescribed Methods,GNN Methods,Benchmark
```

### Comparing `GraphSL-0.1/README.md` & `GraphSL-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `GraphSL-0.1/setup.py` & `GraphSL-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
   name = 'GraphSL',         # How you named your package folder (MyLib)
   packages = find_packages('GraphSL',exclude=['all']),   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Graph Source Localization Approaches and Benchmark Datasets',   # Give a short description about your library
   author = 'Junxiang Wang',                   # Type in your name
   author_email = 'junxiang.wang@alumni.emory.edu',      # Type in your E-Mail
   url = 'https://xianggebenben.github.io/Junxiang_Wang.github.io/',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/xianggebenben/GraphSL/archive/refs/tags/v_01.tar.gz',    # I explain this later on
   keywords = ['Graph Diffusion', 'Graph Source Localization', 'Prescribed Methods', 'GNN Methods','Benchmark'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'networkx',
-          'random',
           'ndlib',
           'torch',
           'copy',
           'sklearn',
           'scipy',
           'torch_geometric',
           'warnings',
```

