# Comparing `tmp/Python-Algorithm-pyal-1.2.1.tar.gz` & `tmp/Python-Algorithm-pyal-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-Algorithm-pyal-1.2.1.tar", last modified: Wed Apr  3 23:29:01 2024, max compression
+gzip compressed data, was "Python-Algorithm-pyal-1.2.2.tar", last modified: Thu Apr  4 05:44:45 2024, max compression
```

## Comparing `Python-Algorithm-pyal-1.2.1.tar` & `Python-Algorithm-pyal-1.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.252038 Python-Algorithm-pyal-1.2.1/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 23:29:01.251660 Python-Algorithm-pyal-1.2.1/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.2.1/README.md
--rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.2.1/pyproject.toml
--rw-r--r--   0 summer     (502) staff       (20)      732 2024-04-03 23:29:01.253607 Python-Algorithm-pyal-1.2.1/setup.cfg
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.200406 Python-Algorithm-pyal-1.2.1/src/
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.250253 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     1236 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
--rw-r--r--   0 summer     (502) staff       (20)        1 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
--rw-r--r--   0 summer     (502) staff       (20)        5 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/top_level.txt
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.206599 Python-Algorithm-pyal-1.2.1/src/pyal/
--rw-r--r--   0 summer     (502) staff       (20)      593 2024-04-03 23:28:24.000000 Python-Algorithm-pyal-1.2.1/src/pyal/__init__.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.209733 Python-Algorithm-pyal-1.2.1/src/pyal/common/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.2.1/src/pyal/common/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     9310 2024-03-25 21:11:02.000000 Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm.py
--rw-r--r--   0 summer     (502) staff       (20)     3518 2023-12-20 06:27:08.000000 Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.218964 Python-Algorithm-pyal-1.2.1/src/pyal/graph/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph.py
--rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/minimum_span_tree.py
--rw-r--r--   0 summer     (502) staff       (20)     1385 2024-04-03 23:22:17.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path.py
--rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/topological_traversal.py
--rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/topological_traversal_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.235016 Python-Algorithm-pyal-1.2.1/src/pyal/list/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/dequeue.py
--rw-r--r--   0 summer     (502) staff       (20)      310 2023-12-16 01:48:08.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/dequeue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/lfu_cache.py
--rw-r--r--   0 summer     (502) staff       (20)     4035 2023-12-19 22:17:29.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list.py
--rw-r--r--   0 summer     (502) staff       (20)     1772 2023-12-19 22:16:39.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     1099 2024-04-03 23:22:27.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/lru_cache.py
--rw-r--r--   0 summer     (502) staff       (20)      455 2023-12-16 01:38:35.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/queue.py
--rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/queue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/stack.py
--rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/stack_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.238828 Python-Algorithm-pyal-1.2.1/src/pyal/string/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.2.1/src/pyal/string/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.1/src/pyal/string/search.py
--rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.1/src/pyal/string/search_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.248761 Python-Algorithm-pyal-1.2.1/src/pyal/tree/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      685 2023-12-25 08:28:48.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/disjoint_set.py
--rw-r--r--   0 summer     (502) staff       (20)      311 2023-12-25 05:29:03.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/disjoint_set_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     3533 2024-04-03 23:23:06.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap.py
--rw-r--r--   0 summer     (502) staff       (20)      702 2024-04-03 23:20:55.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/min_heap.py
--rw-r--r--   0 summer     (502) staff       (20)     6805 2024-04-03 21:25:24.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map.py
--rw-r--r--   0 summer     (502) staff       (20)     2290 2024-04-03 21:26:09.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.101559 Python-Algorithm-pyal-1.2.2/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-04 05:44:45.101401 Python-Algorithm-pyal-1.2.2/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.2.2/README.md
+-rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.2.2/pyproject.toml
+-rw-r--r--   0 summer     (502) staff       (20)      732 2024-04-04 05:44:45.102208 Python-Algorithm-pyal-1.2.2/setup.cfg
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.070201 Python-Algorithm-pyal-1.2.2/src/
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.100814 Python-Algorithm-pyal-1.2.2/src/Python_Algorithm_pyal.egg-info/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-04 05:44:45.000000 Python-Algorithm-pyal-1.2.2/src/Python_Algorithm_pyal.egg-info/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     1236 2024-04-04 05:44:45.000000 Python-Algorithm-pyal-1.2.2/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
+-rw-r--r--   0 summer     (502) staff       (20)        1 2024-04-04 05:44:45.000000 Python-Algorithm-pyal-1.2.2/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
+-rw-r--r--   0 summer     (502) staff       (20)        5 2024-04-04 05:44:45.000000 Python-Algorithm-pyal-1.2.2/src/Python_Algorithm_pyal.egg-info/top_level.txt
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.075951 Python-Algorithm-pyal-1.2.2/src/pyal/
+-rw-r--r--   0 summer     (502) staff       (20)      593 2024-04-04 05:44:23.000000 Python-Algorithm-pyal-1.2.2/src/pyal/__init__.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.078315 Python-Algorithm-pyal-1.2.2/src/pyal/common/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.2.2/src/pyal/common/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     9310 2024-03-25 21:11:02.000000 Python-Algorithm-pyal-1.2.2/src/pyal/common/algorithm.py
+-rw-r--r--   0 summer     (502) staff       (20)     3518 2023-12-20 06:27:08.000000 Python-Algorithm-pyal-1.2.2/src/pyal/common/algorithm_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.085130 Python-Algorithm-pyal-1.2.2/src/pyal/graph/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/graph.py
+-rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/graph_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/minimum_span_tree.py
+-rw-r--r--   0 summer     (502) staff       (20)     1385 2024-04-03 23:22:17.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/shortest_path.py
+-rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/shortest_path_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/topological_traversal.py
+-rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.2/src/pyal/graph/topological_traversal_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.092045 Python-Algorithm-pyal-1.2.2/src/pyal/list/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/dequeue.py
+-rw-r--r--   0 summer     (502) staff       (20)      328 2024-04-04 05:41:57.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/dequeue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/lfu_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)     4051 2024-04-04 05:37:55.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/linked_list.py
+-rw-r--r--   0 summer     (502) staff       (20)     1772 2024-04-04 05:38:07.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/linked_list_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     1099 2024-04-03 23:22:27.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/lru_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)      463 2024-04-04 05:42:34.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/queue.py
+-rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/queue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/stack.py
+-rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.2/src/pyal/list/stack_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.093840 Python-Algorithm-pyal-1.2.2/src/pyal/string/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.2.2/src/pyal/string/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.2/src/pyal/string/search.py
+-rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.2/src/pyal/string/search_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-04 05:44:45.100017 Python-Algorithm-pyal-1.2.2/src/pyal/tree/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      685 2023-12-25 08:28:48.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/disjoint_set.py
+-rw-r--r--   0 summer     (502) staff       (20)      311 2023-12-25 05:29:03.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/disjoint_set_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     3533 2024-04-03 23:23:06.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/dynamic_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)      702 2024-04-03 23:20:55.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/dynamic_heap_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/min_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)     6805 2024-04-03 21:25:24.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/tree_map.py
+-rw-r--r--   0 summer     (502) staff       (20)     2290 2024-04-03 21:26:09.000000 Python-Algorithm-pyal-1.2.2/src/pyal/tree/tree_map_TEST.py
```

### Comparing `Python-Algorithm-pyal-1.2.1/PKG-INFO` & `Python-Algorithm-pyal-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.2.1
+Version: 1.2.2
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `Python-Algorithm-pyal-1.2.1/README.md` & `Python-Algorithm-pyal-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/setup.cfg` & `Python-Algorithm-pyal-1.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = Python-Algorithm-pyal
 authors = Summer Xia
 author_email = tianxia0209@gmail.com
-version = 1.2.1
+version = 1.2.2
 description = PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/PKG-INFO` & `Python-Algorithm-pyal-1.2.2/src/Python_Algorithm_pyal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.2.1
+Version: 1.2.2
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/SOURCES.txt` & `Python-Algorithm-pyal-1.2.2/src/Python_Algorithm_pyal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/__init__.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .tree.min_heap import MinHeap
 from .tree.tree_map import TreeMap
 from .graph.shortest_path import Dijkstra
 from .graph.graph import Graph
 from .graph.topological_traversal import topological_traversal
 from .string.search import search_KMP
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
```

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/common/algorithm.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm_TEST.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/common/algorithm_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/graph/graph.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph_TEST.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/graph/graph_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/graph/shortest_path.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path_TEST.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/graph/shortest_path_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/graph/topological_traversal.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/graph/topological_traversal.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/list/lfu_cache.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/list/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/list/linked_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,19 +100,19 @@
 
   def pop_back(self):
     assert self._num > 0
     value = self.rbegin().get()
     self.remove(self.rbegin())
     return value
 
-  def front(self):
+  def first_element(self):
     assert self._num > 0
     return self.begin().get()
 
-  def back(self):
+  def last_element(self):
     assert self._num > 0
     return self.rbegin().get()
 
   def begin(self):
     return self._fake_head._next
 
   def end(self):
```

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list_TEST.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/list/linked_list_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/list/lru_cache.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/list/lru_cache.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/string/search.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/string/search.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/tree/disjoint_set.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/tree/disjoint_set.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/tree/dynamic_heap.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap_TEST.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/tree/dynamic_heap_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/tree/tree_map.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map_TEST.py` & `Python-Algorithm-pyal-1.2.2/src/pyal/tree/tree_map_TEST.py`

 * *Files identical despite different names*

