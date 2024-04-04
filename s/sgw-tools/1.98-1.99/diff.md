# Comparing `tmp/sgw_tools-1.98.tar.gz` & `tmp/sgw_tools-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgw_tools-1.98.tar", last modified: Sun Aug  6 13:54:26 2023, max compression
+gzip compressed data, was "sgw_tools-1.99.tar", last modified: Thu Apr  4 16:51:39 2024, max compression
```

## Comparing `sgw_tools-1.98.tar` & `sgw_tools-1.99.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.811122 sgw_tools-1.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-06 13:53:47.000000 sgw_tools-1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 13:54:26.807122 sgw_tools-1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-06 13:53:47.000000 sgw_tools-1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 13:54:26.811122 sgw_tools-1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-06 13:53:47.000000 sgw_tools-1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.807122 sgw_tools-1.98/sgw_tools/
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-08-06 13:53:47.000000 sgw_tools-1.98/sgw_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.807122 sgw_tools-1.98/sgw_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-06 13:54:26.000000 sgw_tools-1.98/sgw_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 13:54:26.807122 sgw_tools-1.98/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 13:53:47.000000 sgw_tools-1.98/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-08-06 13:53:47.000000 sgw_tools-1.98/tests/test_biggraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:51:39.734174 sgw_tools-1.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 16:51:12.000000 sgw_tools-1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-04 16:51:39.734174 sgw_tools-1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-04 16:51:12.000000 sgw_tools-1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:51:39.734174 sgw_tools-1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 16:51:12.000000 sgw_tools-1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:51:39.734174 sgw_tools-1.99/sgw_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-04-04 16:51:12.000000 sgw_tools-1.99/sgw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-04 16:51:12.000000 sgw_tools-1.99/sgw_tools/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-04-04 16:51:12.000000 sgw_tools-1.99/sgw_tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-04 16:51:12.000000 sgw_tools-1.99/sgw_tools/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-04 16:51:12.000000 sgw_tools-1.99/sgw_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:51:39.734174 sgw_tools-1.99/sgw_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-04 16:51:39.000000 sgw_tools-1.99/sgw_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-04 16:51:39.000000 sgw_tools-1.99/sgw_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:51:39.000000 sgw_tools-1.99/sgw_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 16:51:39.000000 sgw_tools-1.99/sgw_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:51:39.734174 sgw_tools-1.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:51:12.000000 sgw_tools-1.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17924 2024-04-04 16:51:12.000000 sgw_tools-1.99/tests/test_biggraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-04 16:51:12.000000 sgw_tools-1.99/tests/test_util.py
```

### Comparing `sgw_tools-1.98/LICENSE` & `sgw_tools-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.98/PKG-INFO` & `sgw_tools-1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgw_tools
-Version: 1.98
+Version: 1.99
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.98/setup.py` & `sgw_tools-1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sgw_tools",
-    version="1.98",
+    version="1.99",
     author="Mark Hale",
     license="MIT",
     description="Spectral graph wavelet tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pulquero/sgw",
     packages=find_packages(),
```

### Comparing `sgw_tools-1.98/sgw_tools/__init__.py` & `sgw_tools-1.99/sgw_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.98/sgw_tools/filters.py` & `sgw_tools-1.99/sgw_tools/filters.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.98/sgw_tools/graph.py` & `sgw_tools-1.99/sgw_tools/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             raise ValueError('Adjacency: there is a Not a Number (NaN).')
         if np.isinf(self.W.sum()):
             raise ValueError('Adjacency: there is an infinite value.')
         if self.has_loops():
             self.logger.warning('Adjacency: there are self-loops '
                                 '(non-zeros on the diagonal). '
                                 'The Laplacian will not see them.')
-        if (self.W < 0).nnz != 0:
+        if util.count_negatives(self.W) != 0:
             self.logger.warning('Adjacency: there are negative edge weights.')
 
         self.gtype = 'unknown'
 
         self.n_vertices = self.N = self.W.shape[0]
 
         # Don't keep edges of 0 weight. Otherwise Ne will not correspond
```

### Comparing `sgw_tools-1.98/sgw_tools/graphs.py` & `sgw_tools-1.99/sgw_tools/graphs.py`

 * *Files identical despite different names*

### Comparing `sgw_tools-1.98/sgw_tools/util.py` & `sgw_tools-1.99/sgw_tools/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,7 +143,11 @@
     assert np.allclose(p.imag, 0)
     return p.real/p.real.sum()
 
 
 def operator_norm(W, maxiter=1000):
     svals = sparse.linalg.svds(W.asfptype(), k=1, return_singular_vectors=False, solver="lobpcg", maxiter=maxiter)
     return svals[0]
+
+
+def count_negatives(W):
+    return np.count_nonzero(W.data < 0)
```

### Comparing `sgw_tools-1.98/sgw_tools.egg-info/PKG-INFO` & `sgw_tools-1.99/sgw_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sgw-tools
-Version: 1.98
+Name: sgw_tools
+Version: 1.99
 Summary: Spectral graph wavelet tools
 Home-page: https://github.com/pulquero/sgw
 Author: Mark Hale
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sgw_tools-1.98/tests/test_biggraph.py` & `sgw_tools-1.99/tests/test_biggraph.py`

 * *Files identical despite different names*

