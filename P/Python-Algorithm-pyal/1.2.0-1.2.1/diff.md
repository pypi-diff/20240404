# Comparing `tmp/Python-Algorithm-pyal-1.2.0.tar.gz` & `tmp/Python-Algorithm-pyal-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python-Algorithm-pyal-1.2.0.tar", last modified: Wed Apr  3 19:44:13 2024, max compression
+gzip compressed data, was "Python-Algorithm-pyal-1.2.1.tar", last modified: Wed Apr  3 23:29:01 2024, max compression
```

## Comparing `Python-Algorithm-pyal-1.2.0.tar` & `Python-Algorithm-pyal-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.130190 Python-Algorithm-pyal-1.2.0/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 19:44:13.129993 Python-Algorithm-pyal-1.2.0/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.2.0/README.md
--rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.2.0/pyproject.toml
--rw-r--r--   0 summer     (502) staff       (20)      732 2024-04-03 19:44:13.130994 Python-Algorithm-pyal-1.2.0/setup.cfg
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.102186 Python-Algorithm-pyal-1.2.0/src/
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.129182 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/
--rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/PKG-INFO
--rw-r--r--   0 summer     (502) staff       (20)     1236 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
--rw-r--r--   0 summer     (502) staff       (20)        1 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
--rw-r--r--   0 summer     (502) staff       (20)        5 2024-04-03 19:44:13.000000 Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/top_level.txt
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.106181 Python-Algorithm-pyal-1.2.0/src/pyal/
--rw-r--r--   0 summer     (502) staff       (20)      593 2024-04-03 19:43:40.000000 Python-Algorithm-pyal-1.2.0/src/pyal/__init__.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.108081 Python-Algorithm-pyal-1.2.0/src/pyal/common/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.2.0/src/pyal/common/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     9310 2024-03-25 21:11:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm.py
--rw-r--r--   0 summer     (502) staff       (20)     3518 2023-12-20 06:27:08.000000 Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.113408 Python-Algorithm-pyal-1.2.0/src/pyal/graph/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph.py
--rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/minimum_span_tree.py
--rw-r--r--   0 summer     (502) staff       (20)     1387 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path.py
--rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/topological_traversal.py
--rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.0/src/pyal/graph/topological_traversal_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.120067 Python-Algorithm-pyal-1.2.0/src/pyal/list/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/dequeue.py
--rw-r--r--   0 summer     (502) staff       (20)      310 2023-12-16 01:48:08.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/dequeue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/lfu_cache.py
--rw-r--r--   0 summer     (502) staff       (20)     4035 2023-12-19 22:17:29.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list.py
--rw-r--r--   0 summer     (502) staff       (20)     1772 2023-12-19 22:16:39.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     1101 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/lru_cache.py
--rw-r--r--   0 summer     (502) staff       (20)      455 2023-12-16 01:38:35.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/queue.py
--rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/queue_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/stack.py
--rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.0/src/pyal/list/stack_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.121646 Python-Algorithm-pyal-1.2.0/src/pyal/string/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.2.0/src/pyal/string/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.0/src/pyal/string/search.py
--rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.0/src/pyal/string/search_TEST.py
-drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 19:44:13.128213 Python-Algorithm-pyal-1.2.0/src/pyal/tree/
--rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/__init__.py
--rw-r--r--   0 summer     (502) staff       (20)      685 2023-12-25 08:28:48.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/disjoint_set.py
--rw-r--r--   0 summer     (502) staff       (20)      311 2023-12-25 05:29:03.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/disjoint_set_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)     3558 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap.py
--rw-r--r--   0 summer     (502) staff       (20)      704 2023-11-20 21:03:56.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap_TEST.py
--rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/min_heap.py
--rw-r--r--   0 summer     (502) staff       (20)     7179 2024-04-03 19:41:02.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map.py
--rw-r--r--   0 summer     (502) staff       (20)     2212 2024-04-03 17:11:32.000000 Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.252038 Python-Algorithm-pyal-1.2.1/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 23:29:01.251660 Python-Algorithm-pyal-1.2.1/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     3055 2023-12-16 02:37:57.000000 Python-Algorithm-pyal-1.2.1/README.md
+-rw-r--r--   0 summer     (502) staff       (20)       94 2023-11-02 20:23:19.000000 Python-Algorithm-pyal-1.2.1/pyproject.toml
+-rw-r--r--   0 summer     (502) staff       (20)      732 2024-04-03 23:29:01.253607 Python-Algorithm-pyal-1.2.1/setup.cfg
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.200406 Python-Algorithm-pyal-1.2.1/src/
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.250253 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/
+-rw-r--r--   0 summer     (502) staff       (20)     3624 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/PKG-INFO
+-rw-r--r--   0 summer     (502) staff       (20)     1236 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/SOURCES.txt
+-rw-r--r--   0 summer     (502) staff       (20)        1 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/dependency_links.txt
+-rw-r--r--   0 summer     (502) staff       (20)        5 2024-04-03 23:29:01.000000 Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/top_level.txt
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.206599 Python-Algorithm-pyal-1.2.1/src/pyal/
+-rw-r--r--   0 summer     (502) staff       (20)      593 2024-04-03 23:28:24.000000 Python-Algorithm-pyal-1.2.1/src/pyal/__init__.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.209733 Python-Algorithm-pyal-1.2.1/src/pyal/common/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:21.000000 Python-Algorithm-pyal-1.2.1/src/pyal/common/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     9310 2024-03-25 21:11:02.000000 Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm.py
+-rw-r--r--   0 summer     (502) staff       (20)     3518 2023-12-20 06:27:08.000000 Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.218964 Python-Algorithm-pyal-1.2.1/src/pyal/graph/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:25.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)     1842 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph.py
+-rw-r--r--   0 summer     (502) staff       (20)      576 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)        7 2023-12-16 01:35:27.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/minimum_span_tree.py
+-rw-r--r--   0 summer     (502) staff       (20)     1385 2024-04-03 23:22:17.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path.py
+-rw-r--r--   0 summer     (502) staff       (20)      780 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      595 2023-11-20 21:03:58.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/topological_traversal.py
+-rw-r--r--   0 summer     (502) staff       (20)      401 2023-11-20 21:03:57.000000 Python-Algorithm-pyal-1.2.1/src/pyal/graph/topological_traversal_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.235016 Python-Algorithm-pyal-1.2.1/src/pyal/list/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:28.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      130 2023-12-16 01:45:31.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/dequeue.py
+-rw-r--r--   0 summer     (502) staff       (20)      310 2023-12-16 01:48:08.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/dequeue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     2340 2023-11-23 05:16:03.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/lfu_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)     4035 2023-12-19 22:17:29.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list.py
+-rw-r--r--   0 summer     (502) staff       (20)     1772 2023-12-19 22:16:39.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     1099 2024-04-03 23:22:27.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/lru_cache.py
+-rw-r--r--   0 summer     (502) staff       (20)      455 2023-12-16 01:38:35.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/queue.py
+-rw-r--r--   0 summer     (502) staff       (20)      259 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/queue_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      484 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/stack.py
+-rw-r--r--   0 summer     (502) staff       (20)      318 2023-12-16 01:42:13.000000 Python-Algorithm-pyal-1.2.1/src/pyal/list/stack_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.238828 Python-Algorithm-pyal-1.2.1/src/pyal/string/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:32.000000 Python-Algorithm-pyal-1.2.1/src/pyal/string/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      743 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.1/src/pyal/string/search.py
+-rw-r--r--   0 summer     (502) staff       (20)      337 2023-11-20 21:04:00.000000 Python-Algorithm-pyal-1.2.1/src/pyal/string/search_TEST.py
+drwxr-xr-x   0 summer     (502) staff       (20)        0 2024-04-03 23:29:01.248761 Python-Algorithm-pyal-1.2.1/src/pyal/tree/
+-rw-r--r--   0 summer     (502) staff       (20)        0 2023-11-03 00:24:36.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/__init__.py
+-rw-r--r--   0 summer     (502) staff       (20)      685 2023-12-25 08:28:48.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/disjoint_set.py
+-rw-r--r--   0 summer     (502) staff       (20)      311 2023-12-25 05:29:03.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/disjoint_set_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)     3533 2024-04-03 23:23:06.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)      702 2024-04-03 23:20:55.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap_TEST.py
+-rw-r--r--   0 summer     (502) staff       (20)      448 2023-12-16 01:22:02.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/min_heap.py
+-rw-r--r--   0 summer     (502) staff       (20)     6805 2024-04-03 21:25:24.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map.py
+-rw-r--r--   0 summer     (502) staff       (20)     2290 2024-04-03 21:26:09.000000 Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map_TEST.py
```

### Comparing `Python-Algorithm-pyal-1.2.0/PKG-INFO` & `Python-Algorithm-pyal-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.2.0
+Version: 1.2.1
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `Python-Algorithm-pyal-1.2.0/README.md` & `Python-Algorithm-pyal-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/setup.cfg` & `Python-Algorithm-pyal-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = Python-Algorithm-pyal
 authors = Summer Xia
 author_email = tianxia0209@gmail.com
-version = 1.2.0
+version = 1.2.1
 description = PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/PKG-INFO` & `Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Python-Algorithm-pyal
-Version: 1.2.0
+Version: 1.2.1
 Summary: PYthon Algorithm Library (pyal) targets at providing a python version substitue of STL in C++, such as linked list, tree map, and other data structures and popular algorithms.
 Home-page: https://github.com/SummerRainET2008/PYthon_Algorithms_Library
 Author-email: tianxia0209@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/Python_Algorithm_pyal.egg-info/SOURCES.txt` & `Python-Algorithm-pyal-1.2.1/src/Python_Algorithm_pyal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/__init__.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from .tree.min_heap import MinHeap
 from .tree.tree_map import TreeMap
 from .graph.shortest_path import Dijkstra
 from .graph.graph import Graph
 from .graph.topological_traversal import topological_traversal
 from .string.search import search_KMP
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/common/algorithm_TEST.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/common/algorithm_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/graph/graph_TEST.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/graph/graph_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
       for edge in graph.get_out_edges(v):
         if edge.v2 in self._opt_dist:
           continue
 
         old_value = heap.get(edge.v2)
         new_value = dist + edge.weight
         if new_value < old_value:
-          heap.update(edge.v2, new_value)
+          heap.push(edge.v2, new_value)
           self._opt_in_edge[edge.v2] = edge.v1
 
   def get_min_distance(self, target_vertex: int):
     return self._opt_dist.get(target_vertex, None)
 
   def get_optimal_paths(self, target_vertex: int):
     paths = []
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/graph/shortest_path_TEST.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/graph/shortest_path_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/graph/topological_traversal.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/graph/topological_traversal.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/list/lfu_cache.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/list/lfu_cache.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/list/linked_list_TEST.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/list/linked_list_TEST.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/list/lru_cache.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/list/lru_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     self._update_node(node)
     return node.get().value
 
   def put(self, key: int, value: int) -> None:
     node = self._key2node.get(key, None)
     if node is not None:
-      node.content = node.get().update(value)
+      node.content = node.get().push(value)
       self._update_node(node)
 
     else:
       if len(self._key2node) == self._capacity:
         del self._key2node[self._list.pop_back().key]
 
       self._list.push_front(Item(key, value))
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/string/search.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/string/search.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/tree/disjoint_set.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/tree/disjoint_set.py`

 * *Files identical despite different names*

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,17 @@
     return len(self._data) - 1
 
   def top(self):
     assert self.size() > 0
     return self._data[1]
 
   def push(self, id, value):
-    pos = self._id2pos.get(id, None)
-    assert pos is None, f"id={id} is existent. You could use self.update(...)."
+    if id in self._id2pos:
+      self._update(id, value)
+      return
 
     pos = len(self._data)
     self._assign_item(pos, self.Item(id=id, value=value))
     self._adjust_bottom_to_up(pos)
     # print(self.__data)
 
   def pop(self):
@@ -87,15 +88,17 @@
     new_item = self._data.pop()
     self._assign_item(pos, new_item)
     if new_item.value < old_item.value:
       self._adjust_bottom_to_up(pos)
     else:
       self._adjust_up_to_bottom(pos)
 
-  def update(self, id, value):
+  def _update(self, id, value):
+    assert id in self._id2pos
+
     pos = self._id2pos[id]
     old_item = self._data[pos]
     if value == old_item.value:
       return
 
     new_item = self.Item(id=old_item.id, value=value)
     self._data[pos] = new_item
@@ -134,33 +137,33 @@
   heap.push(0, 10)
   heap.push(1, 1)
   heap.push(2, 20)
   heap.push(3, 30)
   heap.push(4, 2)
   heap.push(5, 90)
 
-  heap.update(0, 0)
-  heap.update(1, 25)
-  heap.update(5, 10)
+  heap.push(0, 0)
+  heap.push(1, 25)
+  heap.push(5, 10)
 
   heap.remove(4)
   heap.remove(3)
 
   heap.push(5, 20)
   heap.push(6, 0)
-  heap.update(0, 1)
+  heap.push(0, 1)
 
   while heap.size() > 2:
     print(heap.top())
     heap.pop()
   print("-" * 32)
 
   heap.push(7, 100)
   # heap.remove(5)
-  heap.update(1, 15)
+  heap.push(1, 15)
 
   while heap.size() > 0:
     print(heap.top())
     heap.pop()
 
 
 def main():
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/tree/dynamic_heap_TEST.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/tree/dynamic_heap_TEST.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   heap.push(2, 6)
   heap.push(3, 7)
   heap.push(4, 8)
   heap.push(5, 9)
 
   assert heap.top() == DynamicHeap.Item(1, 5)
 
-  heap.update(5, 4)
+  heap.push(5, 4)
   assert heap.top() == DynamicHeap.Item(5, 4)
 
   heap.remove(5)
   heap.remove(1)
   assert heap.top() == DynamicHeap.Item(2, 6)
 
   heap.pop()
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,16 +73,15 @@
 
     else:
       if self._right is None:
         self._right = _AVLTreeNode(key)
       else:
         self._right = self._right._insert(key, next_key)
 
-    self._depth = 1 + max(self._get_depth(self._left),
-                          self._get_depth(self._right))
+    self._reset_depth()
 
     bf = self._get_balance_factor(self)
     if bf > 1:
       if key > self._left._key:
         self._left = self._left._left_rotate()
       return self._right_rotate()
 
@@ -98,54 +97,46 @@
     left = self._left
     left_right = left._right
 
     # Perform rotation
     left._right = self
     self._left = left_right
 
-    # Update heights
-    self._depth = 1 + max(self._get_depth(self._left),
-                          self._get_depth(self._right))
-    left._depth = 1 + max(self._get_depth(left._left),
-                          self._get_depth(left._right))
+    self._reset_depth()
+    left._reset_depth()
 
     return left
 
   def _get_depth(self, node):
     return 0 if node is None else node._depth
 
   def _reset_depth(self):
     self._depth = max(self._get_depth(self._left), self._get_depth(
         self._right)) + 1
 
   def _left_rotate(self):
     right = self._right
     right_left = right._left
 
-    # Perform rotation
     right._left = self
     self._right = right_left
 
-    # Update heights
-    self._depth = 1 + max(self._get_depth(self._left),
-                          self._get_depth(self._right))
-    right._depth = 1 + max(self._get_depth(right._left),
-                       self._get_depth(right._right))
+    self._reset_depth()
+    right._reset_depth()
 
     return right
 
   def _get_min_value_node(self):
     if self._left is None:
       return self
     return self._left._get_min_value_node()
 
   def _get_balance_factor(self, node):
     if node is None:
       return 0
-
     return self._get_depth(node._left) - self._get_depth(node._right)
 
   def _remove(self, key):
     # Key must be existent
     if key < self._key:
       self._left = self._left._remove(key)
     elif key > self._key:
@@ -196,14 +187,20 @@
 
   def _print_tree(self):
     if self._root is None:
       print("null-tree")
     else:
       self._root._print_tree()
 
+  def first_key(self):
+    return self.key_list_begin().get()
+
+  def last_key(self):
+    return self.key_list_rbegin().get()
+
   def keys(self) -> iter:
     node = self._key_list.begin()
     while node is not self._key_list.end():
       yield node.get()
       node = node.next()
 
   def items(self) -> iter:
```

### Comparing `Python-Algorithm-pyal-1.2.0/src/pyal/tree/tree_map_TEST.py` & `Python-Algorithm-pyal-1.2.1/src/pyal/tree/tree_map_TEST.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,14 +58,17 @@
 def test_one_remove():
   tree = TreeMap()
   data = [5, 4, 6, 3, 7, 2, 8, 1, 9, 0, 10]
   for d in data:
     tree[d] = d
   tree._print_tree()
 
+  assert tree.first_key() == min(data)
+  assert tree.last_key() == max(data)
+
   tree.remove(5)
   print(f"Removed 5")
   tree._print_tree()
   node = tree.lower_bound(5)
   assert node.get() == 6
 
   tree.remove(1)
```

