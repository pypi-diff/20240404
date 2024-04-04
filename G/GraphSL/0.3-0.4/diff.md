# Comparing `tmp/GraphSL-0.3.tar.gz` & `tmp/GraphSL-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphSL-0.3.tar", last modified: Thu Apr  4 05:17:38 2024, max compression
+gzip compressed data, was "GraphSL-0.4.tar", last modified: Thu Apr  4 05:19:51 2024, max compression
```

## Comparing `GraphSL-0.3.tar` & `GraphSL-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 05:17:38.965063 GraphSL-0.3/
-drwxrwxrwx   0        0        0        0 2024-04-04 05:17:38.963068 GraphSL-0.3/GraphSL.egg-info/
--rw-rw-rw-   0        0        0      708 2024-04-04 05:17:38.000000 GraphSL-0.3/GraphSL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-04-04 05:17:38.000000 GraphSL-0.3/GraphSL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:17:38.000000 GraphSL-0.3/GraphSL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-04-04 05:17:38.000000 GraphSL-0.3/GraphSL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:17:38.000000 GraphSL-0.3/GraphSL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.3/LICENSE
--rw-rw-rw-   0        0        0      708 2024-04-04 05:17:38.966060 GraphSL-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.3/README.md
--rw-rw-rw-   0        0        0       86 2024-04-04 05:17:38.967068 GraphSL-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1854 2024-04-04 05:17:10.000000 GraphSL-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:19:51.256425 GraphSL-0.4/
+drwxrwxrwx   0        0        0        0 2024-04-04 05:19:51.254433 GraphSL-0.4/GraphSL.egg-info/
+-rw-rw-rw-   0        0        0      708 2024-04-04 05:19:51.000000 GraphSL-0.4/GraphSL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-04-04 05:19:51.000000 GraphSL-0.4/GraphSL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 05:19:51.000000 GraphSL-0.4/GraphSL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-04 05:19:51.000000 GraphSL-0.4/GraphSL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 05:19:51.000000 GraphSL-0.4/GraphSL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2024-04-02 03:37:06.000000 GraphSL-0.4/LICENSE
+-rw-rw-rw-   0        0        0      708 2024-04-04 05:19:51.256425 GraphSL-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9089 2024-04-03 23:13:28.000000 GraphSL-0.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-04 05:19:51.257388 GraphSL-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1859 2024-04-04 05:19:39.000000 GraphSL-0.4/setup.py
```

### Comparing `GraphSL-0.3/GraphSL.egg-info/PKG-INFO` & `GraphSL-0.4/GraphSL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSL
-Version: 0.3
+Version: 0.4
 Summary: Graph Source Localization Approaches and Benchmark Datasets
 Home-page: https://xianggebenben.github.io/Junxiang_Wang.github.io/
 Author: Junxiang Wang
 Author-email: junxiang.wang@alumni.emory.edu
 License: MIT
 Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.3.tar.gz
 Keywords: Graph Diffusion,Graph Source Localization,Prescribed Methods,GNN Methods,Benchmark
```

### Comparing `GraphSL-0.3/LICENSE` & `GraphSL-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GraphSL-0.3/PKG-INFO` & `GraphSL-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphSL
-Version: 0.3
+Version: 0.4
 Summary: Graph Source Localization Approaches and Benchmark Datasets
 Home-page: https://xianggebenben.github.io/Junxiang_Wang.github.io/
 Author: Junxiang Wang
 Author-email: junxiang.wang@alumni.emory.edu
 License: MIT
 Download-URL: https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.3.tar.gz
 Keywords: Graph Diffusion,Graph Source Localization,Prescribed Methods,GNN Methods,Benchmark
```

### Comparing `GraphSL-0.3/README.md` & `GraphSL-0.4/README.md`

 * *Files identical despite different names*

### Comparing `GraphSL-0.3/setup.py` & `GraphSL-0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
   name = 'GraphSL',         # How you named your package folder (MyLib)
   packages = find_packages('GraphSL',exclude=['all']),   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Graph Source Localization Approaches and Benchmark Datasets',   # Give a short description about your library
   author = 'Junxiang Wang',                   # Type in your name
   author_email = 'junxiang.wang@alumni.emory.edu',      # Type in your E-Mail
   url = 'https://xianggebenben.github.io/Junxiang_Wang.github.io/',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/xianggebenben/GraphSL/archive/refs/tags/v.0.3.tar.gz',    # I explain this later on
   keywords = ['Graph Diffusion', 'Graph Source Localization', 'Prescribed Methods', 'GNN Methods','Benchmark'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'networkx',
           'ndlib',
           'torch',
-          'sklearn',
+          'scikit-learn',
           'scipy',
           'torch_geometric',
           'warnings',
           'operator',
           'enum',
           'typing',
           'sys'
```

