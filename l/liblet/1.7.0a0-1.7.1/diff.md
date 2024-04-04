# Comparing `tmp/liblet-1.7.0a0.tar.gz` & `tmp/liblet-1.7.1.tar.gz`

## Comparing `liblet-1.7.0a0.tar` & `liblet-1.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/api.rst
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/conf.py
--rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/examples.ipynb
--rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/examples.rst
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/index.rst
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/installation.rst
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/stg.svg
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/tree.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/_static/custom.css
--rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/_static/logo.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/_templates/project.html
--rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/examples_files/examples_70_0.svg
--rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/examples_files/examples_71_0.svg
--rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/examples_files/examples_82_0.svg
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/examples_files/examples_83_0.svg
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.0a0/docs/examples_files/examples_8_0.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/scripts.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/__init__.py
--rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/antlr.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/automaton.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/const.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/decorators.py
--rw-r--r--   0        0        0    19497 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/display.py
--rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/grammar.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/llvm.py
--rw-r--r--   0        0        0     9671 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/liblet/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/tests/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/tests/antlr_test.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/tests/automaton_test.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/tests/decorators_test.py
--rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/tests/grammar_test.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/tests/run.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.0a0/src/tests/utils_test.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.0a0/.gitignore
--rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.0a0/LICENSE-CC.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.0a0/LICENSE-GPL.txt
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.0a0/README.md
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 liblet-1.7.0a0/pyproject.toml
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 liblet-1.7.0a0/PKG-INFO
+-rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/api.rst
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/conf.py
+-rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples.ipynb
+-rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples.rst
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/index.rst
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/installation.rst
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/stg.svg
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/tree.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/_static/custom.css
+-rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/_static/logo.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/_templates/project.html
+-rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_70_0.svg
+-rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_71_0.svg
+-rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_82_0.svg
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_83_0.svg
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_8_0.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.1/src/scripts.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/__init__.py
+-rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/antlr.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/automaton.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/const.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/decorators.py
+-rw-r--r--   0        0        0    20296 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/display.py
+-rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/grammar.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/llvm.py
+-rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/antlr_test.py
+-rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/automaton_test.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/decorators_test.py
+-rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/grammar_test.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/run.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/utils_test.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.1/.gitignore
+-rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.1/LICENSE-CC.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.1/LICENSE-GPL.txt
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.1/README.md
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.1/PKG-INFO
```

### Comparing `liblet-1.7.0a0/docs/api.rst` & `liblet-1.7.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/conf.py` & `liblet-1.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/examples.ipynb` & `liblet-1.7.1/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/examples.rst` & `liblet-1.7.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/index.rst` & `liblet-1.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/installation.rst` & `liblet-1.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/stg.svg` & `liblet-1.7.1/docs/stg.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/tree.svg` & `liblet-1.7.1/docs/tree.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/_static/logo.png` & `liblet-1.7.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/_templates/project.html` & `liblet-1.7.1/docs/_templates/project.html`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/examples_files/examples_70_0.svg` & `liblet-1.7.1/docs/examples_files/examples_70_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/examples_files/examples_71_0.svg` & `liblet-1.7.1/docs/examples_files/examples_71_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/examples_files/examples_82_0.svg` & `liblet-1.7.1/docs/examples_files/examples_82_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/examples_files/examples_83_0.svg` & `liblet-1.7.1/docs/examples_files/examples_83_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/docs/examples_files/examples_8_0.svg` & `liblet-1.7.1/docs/examples_files/examples_8_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/liblet/__init__.py` & `liblet-1.7.1/src/liblet/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.7.0a0'
+__version__ = '1.7.1'
 
 from liblet.antlr import ANTLR, AnnotatedTreeWalker
 from liblet.automaton import (
   Automaton,
   BottomUpInstantaneousDescription,
   InstantaneousDescription,
   TopDownInstantaneousDescription,
@@ -19,29 +19,45 @@
   cyk2table,
   dict2table,
   dod2table,
   ff2table,
   iter2table,
   prods2table,
   pyast2tree,
+  resized_svg_repr,
   side_by_side,
 )
 from liblet.grammar import Derivation, Grammar, Item, Production, Productions
 from liblet.llvm import LLVM
-from liblet.utils import AttrDict, CYKTable, Queue, Stack, Table, first, letstr, peek, suffixes, uc, union_of, warn
+from liblet.utils import (
+  AttrDict,
+  CYKTable,
+  Queue,
+  Stack,
+  Table,
+  compose,
+  first,
+  letstr,
+  peek,
+  suffixes,
+  uc,
+  union_of,
+  warn,
+)
 
 __all__ = [
   '__version__',
   'animate_derivation',
   'AnnotatedTreeWalker',
   'ANTLR',
   'AttrDict',
   'Automaton',
   'BottomUpInstantaneousDescription',
   'closure',
+  'compose',
   'cyk2table',
   'CYKTable',
   'Derivation',
   'DIAMOND',
   'dict2table',
   'dod2table',
   'ff2table',
@@ -57,14 +73,15 @@
   'peek',
   'prods2table',
   'Production',
   'ProductionGraph',
   'Productions',
   'pyast2tree',
   'Queue',
+  'resized_svg_repr',
   'show_calls',
   'side_by_side',
   'Stack',
   'StateTransitionGraph',
   'suffixes',
   'Table',
   'TopDownInstantaneousDescription',
```

### Comparing `liblet-1.7.0a0/src/liblet/antlr.py` & `liblet-1.7.1/src/liblet/antlr.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/liblet/automaton.py` & `liblet-1.7.1/src/liblet/automaton.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/liblet/decorators.py` & `liblet-1.7.1/src/liblet/decorators.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/liblet/display.py` & `liblet-1.7.1/src/liblet/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import ast
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from collections.abc import Mapping, Set  # noqa: PYI025
 from functools import partial
 from html import escape
 from itertools import chain, pairwise
+from operator import itemgetter
 from re import sub
 from warnings import warn as wwarn
 
+import svgutils.transform as svg_ttransform
 from graphviz import Digraph
-from IPython.display import HTML, display
+from IPython.display import HTML, SVG, display
 from ipywidgets import IntSlider, interactive
 
 from liblet.const import ε
 from liblet.grammar import HAIR_SPACE, Derivation, Productions
-from liblet.utils import AttrDict, CYKTable, letstr
+from liblet.utils import AttrDict, CYKTable, compose, letstr
 
 
 def _escape(label):
   return sub(r'\]', '&#93;', sub(r'\[', '&#91;', escape(str(label))))
 
 
-def make_node_wrapper(
-  node_label='default',  # how to produce the node label from the node object
-  node_eq='obj',  # how to decide equality between nodes
-  default_gv_args=None,  # default gv arguments for nodes
+def make_mapping_aware_str(
   other_str=letstr,  # in mapping_aware_str, how to represent non-mapping objects
   key_str=str,  # in mapping_aware_str, how to represent keys
   value_str=_escape,  # in mapping_aware_str, how to represent values
   key_filter=lambda k: not k.startswith('_thread_'),  # in mapping_aware_str, which keys to show
 ):
   def mapping_aware_str(obj):
     if obj is None:
@@ -37,37 +36,42 @@
       return ''.join(
         ['<<FONT POINT-SIZE="12"><TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0">']
         + [f'<TR><TD>{key_str(k)}</TD><TD>{value_str(obj[k])}</TD></TR>' for k in filter(key_filter, obj)]
         + ['</TABLE></FONT>>']
       )
     return other_str(obj)
 
-  def mapping_aware_gv_args(obj):
-    return {'shape': 'none', 'margin': '0'} if isinstance(obj, Mapping) else {'margin': '.05'}
+  return mapping_aware_str
+
+
+def mapping_aware_gv_args(obj):
+  return {'shape': 'none', 'margin': '0'} if isinstance(obj, Mapping) else {'margin': '.05'}
 
-  if node_label == 'default':
-    node_label = mapping_aware_str
-    if default_gv_args is None:
-      default_gv_args = lambda x: mapping_aware_gv_args(x)
-  elif node_label == 'first':
-    node_label = lambda x: mapping_aware_str(x[0])
-    if default_gv_args is None:
-      default_gv_args = lambda x: mapping_aware_gv_args(x[0])
+
+def make_node_wrapper(
+  node_label=None,  # how to produce the node label from the node object
+  node_eq='obj',  # how to decide equality between nodes
+  default_gv_args=None,  # how to produce the default gv args from the node object
+):
+  if node_label is None:
+    node_label = make_mapping_aware_str()
   elif not callable(node_label):
-    raise ValueError('node_label must be either "default", "first" or a callable')
+    raise ValueError('node_label must be either None or a callable')
 
   if node_eq == 'obj':
     node_eq = lambda x, y: x == y
   elif node_eq == 'str':
     node_eq = lambda x, y: node_label(x) == node_label(y)
   elif not callable(node_eq):
     raise ValueError('node_eq must be either "obj", "str" or a callable')
 
-  if not callable(default_gv_args):
-    raise TypeError('default_gv_args must be a callable')
+  if default_gv_args is None:
+    default_gv_args = lambda x: mapping_aware_gv_args(x)
+  elif not callable(default_gv_args):
+    raise ValueError('default_gv_args must be either None or a callable')
 
   class NodeWrapper:
     def __init__(self, obj):
       self.obj = obj
 
     def __eq__(self, other):
       return node_eq(self.obj, other.obj)
@@ -87,15 +91,19 @@
     def __repr__(self):
       return f'NodeWrapper[obj = {self.obj}, label = {self.label()}, hash = {hash(self)}]'
 
   return NodeWrapper
 
 
 class GVWrapper:
-  def __init__(self, gv_graph_args, node_wrapper):
+  def __init__(self, gv_graph_args=None, node_wrapper=None):
+    if gv_graph_args is None:
+      gv_graph_args = {}
+    if node_wrapper is None:
+      node_wrapper = make_node_wrapper()
     self.G = Digraph(**gv_graph_args)
     self.node_wrapper = node_wrapper
     self.wn2gid = {}
 
   def wrapped_graph(self):
     return self.G
 
@@ -244,15 +252,18 @@
   def _gv_graph_(self):
     G = GVWrapper(
       dict(  # noqa: C408
         graph_attr={'nodesep': '.25', 'ranksep': '.25'},
         node_attr={'shape': 'box', 'width': '0', 'height': '0', 'style': 'rounded, setlinewidth(.25)'},
         edge_attr={'dir': 'none'},
       ),
-      make_node_wrapper(node_label='first', node_shape='box'),
+      make_node_wrapper(
+        node_label=compose(make_mapping_aware_str(), itemgetter(0)),
+        default_gv_args=compose(mapping_aware_gv_args, itemgetter(0)),
+      ),
     )
 
     def walk(T):
       curr = (T.root, T)
       for child in T.children:
         G.edge(curr, (child.root, child))
       if len(T.children) > 1:
@@ -307,15 +318,15 @@
     return G
 
 
 class Graph:
   def __init__(self, arcs, sep=None):
     self.G = GVWrapper(
       dict(graph_attr={'size': '8', 'rankdir': 'LR'}, node_attr={'shape': 'oval'}),  # noqa: C408
-      make_node_wrapper(other_str=partial(letstr, sep=sep)),
+      make_node_wrapper(node_label=make_mapping_aware_str(other_str=partial(letstr, sep=sep))),
     )
     self.adj = {}
     for src, dst in arcs:
       self.adj[src] = self.adj.get(src, set()) | {dst}
       self.adj[dst] = self.adj.get(dst, set())
       self.G.edge(src, dst)
 
@@ -367,15 +378,15 @@
           'margin': '.05',
           'width': '0',
           'height': '0',
           'style': 'rounded, setlinewidth(.25)',
         },
         edge_attr={'dir': 'none', 'penwidth': '.5', 'arrowsize': '.5'},
       ),
-      make_node_wrapper(node_label='first'),
+      make_node_wrapper(node_label=compose(make_mapping_aware_str(), itemgetter(0))),
     )
 
     def remove_ε(sentence):
       return tuple(_ for _ in sentence if _[0] != ε)
 
     sentence = ((derivation.start, 0, 0),)
     for step, (rule, pos) in enumerate(derivation.steps(), 1):
@@ -496,27 +507,29 @@
     G = GVWrapper(
       dict(  # noqa: C408
         graph_attr={'rankdir': 'LR', 'size': '32'},
         node_attr={'margin': '.05'} if self.large_labels else {},
         engine='dot',
       ),
       make_node_wrapper(
-        node_label='default',
-        other_str=partial(letstr, sep=sep),
+        node_label=make_mapping_aware_str(other_str=partial(letstr, sep=sep)),
         default_gv_args=lambda X: {'peripheries': '2' if X in self.F else '1'},
       ),
     )
     if self.S is not None:
       (G.node('', gv_args={'shape': 'point'}),)
       G.edge('', self.S)
     for X, x, Y in self.transitions:
       G.edge(X, Y, gv_args={'xlabel' if self.large_labels else 'label': x})
     self.G = G
     return G
 
+  def _repr_svg_(self):
+    return self._gv_graph_()._repr_svg_()
+
 
 # Python AST stuff
 
 
 def pyast2tree(node):
   return (
     Tree(
@@ -539,21 +552,33 @@
   steps = d.steps()
   d = Derivation(d.G)
   ui = interactive(lambda n: display(ProductionGraph(d.step(steps[:n]))), n=IntSlider(min=0, max=len(steps), value=0))
   ui.children[-1].layout.height = height
   return ui
 
 
-# HTML stuff
+# HTML/SVG stuff
 
 
 def __bordered_table__(content):  # noqa: N807
   return HTML('<style>td, th {border: 1pt solid lightgray !important ;}</style><table>' + content + '</table>')
 
 
+def resized_svg_repr(obj, width=800, height=600):
+  if hasattr(obj, '_repr_image_svg_xml'):
+    svg_str = obj._repr_image_svg_xml()
+  elif hasattr(obj, '_repr_svg_'):
+    svg_str = obj._repr_svg_()
+  else:
+    raise TypeError('The given object has no svg representation')
+  svg_figure = svg_ttransform.fromstring(svg_str)
+  svg_figure.set_size((str(width), str(height)))
+  return SVG(svg_figure.to_str())
+
+
 def side_by_side(*iterable):
   if len(iterable) == 1:
     iterable = iterable[0]
   return HTML('<div>{}</div>'.format(' '.join(item._repr_svg_() for item in iterable)))
 
 
 def iter2table(it):
```

### Comparing `liblet-1.7.0a0/src/liblet/grammar.py` & `liblet-1.7.1/src/liblet/grammar.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/liblet/llvm.py` & `liblet-1.7.1/src/liblet/llvm.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/liblet/utils.py` & `liblet-1.7.1/src/liblet/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import OrderedDict, defaultdict, deque
 from collections.abc import MutableMapping, Set  #  noqa: PYI025
-from functools import partial
+from functools import partial, reduce
 from html import escape
 from itertools import chain
 from sys import stderr
 from warnings import warn as wwarn
 
 
 def suffixes(α):
@@ -29,14 +29,18 @@
 
 
 def union_of(s):
   """Return the set union of its arguments."""
   return set().union(*s)
 
 
+def compose(*funcs):
+  return reduce(lambda f, g: lambda x: f(g(x)), funcs)
+
+
 def letstr(obj, sep=None, sort=True, remove_outer=False):
   if sep is None:
     sep = ', '
 
   def _ls(obj):
     if isinstance(obj, str):
       return obj
```

### Comparing `liblet-1.7.0a0/src/tests/antlr_test.py` & `liblet-1.7.1/src/tests/antlr_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/tests/automaton_test.py` & `liblet-1.7.1/src/tests/automaton_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/tests/decorators_test.py` & `liblet-1.7.1/src/tests/decorators_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/tests/grammar_test.py` & `liblet-1.7.1/src/tests/grammar_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/src/tests/utils_test.py` & `liblet-1.7.1/src/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/LICENSE-CC.txt` & `liblet-1.7.1/LICENSE-CC.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/LICENSE-GPL.txt` & `liblet-1.7.1/LICENSE-GPL.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/README.md` & `liblet-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `liblet-1.7.0a0/pyproject.toml` & `liblet-1.7.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "liblet"
 description = "A teaching aid library for formal languages and compiler courses."
 readme = "README.md"
 requires-python = ">=3.10"
-license-files = { paths = ["LICENSE-GPL.txt", "LICENSE-CC.txt"] }
 authors = [{ name = "Massimo Santini", email = "massimo.santini@unimi.it" }]
 keywords = [
   "automata",
   "formal",
   "grammar",
   "graph",
   "language",
@@ -30,17 +29,18 @@
   "Programming Language :: Python :: 3.10",
   "Topic :: Education",
   "Topic :: Scientific/Engineering :: Visualization",
   "Topic :: Software Development :: Compilers"
 ]
 dependencies = [
   "antlr4-python3-runtime==4.13.1",
-  "jupyter",
   "graphviz",
-  "ipywidgets"
+  "ipywidgets",
+  "jupyter",
+  "svgutils",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://liblet.readthedocs.io/"
 "Source code" = "https://github.com/let-unimi/liblet"
 Changelog = "https://github.com/let-unimi/liblet/blob/master/CHANGELOG.txt"
```

### Comparing `liblet-1.7.0a0/PKG-INFO` & `liblet-1.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: liblet
-Version: 1.7.0a0
+Version: 1.7.1
 Summary: A teaching aid library for formal languages and compiler courses.
 Project-URL: Documentation, https://liblet.readthedocs.io/
 Project-URL: Source code, https://github.com/let-unimi/liblet
 Project-URL: Changelog, https://github.com/let-unimi/liblet/blob/master/CHANGELOG.txt
 Project-URL: Bug Tracker, https://github.com/let-unimi/liblet/issues
 Author-email: Massimo Santini <massimo.santini@unimi.it>
 License-File: LICENSE-CC.txt
@@ -22,14 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Compilers
 Requires-Python: >=3.10
 Requires-Dist: antlr4-python3-runtime==4.13.1
 Requires-Dist: graphviz
 Requires-Dist: ipywidgets
 Requires-Dist: jupyter
+Requires-Dist: svgutils
 Provides-Extra: docs
 Requires-Dist: pallets-sphinx-themes; extra == 'docs'
 Requires-Dist: pystache; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # LibLET
```

