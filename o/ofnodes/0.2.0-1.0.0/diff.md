# Comparing `tmp/ofnodes-0.2.0.tar.gz` & `tmp/ofnodes-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-0.2.0.tar", max compression
+gzip compressed data, was "ofnodes-1.0.0.tar", max compression
```

## Comparing `ofnodes-0.2.0.tar` & `ofnodes-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0        0 2024-03-25 17:13:37.977755 ofnodes-0.2.0/README.md
--rw-r--r--   0        0        0      590 2024-03-26 21:32:11.836970 ofnodes-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 16:49:51.247086 ofnodes-0.2.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0     1284 2024-03-26 21:30:39.653576 ofnodes-0.2.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-0.2.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 ofnodes-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-25 17:13:37.977755 ofnodes-1.0.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-04 17:47:49.284523 ofnodes-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1747 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.0.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    18327 2024-04-04 17:47:49.284523 ofnodes-1.0.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 ofnodes-1.0.0/PKG-INFO
```

### Comparing `ofnodes-0.2.0/pyproject.toml` & `ofnodes-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "0.2.0"
+version = "1.0.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-0.2.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.0.0/src/ofnodes/nodes/singlynode.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,40 +8,56 @@
     Typical usage example:
 
         uni_node = SinglyNode("a string of characters")
 """
 
 from typing import Any, Optional
 
+#from ofnodes.nodes.node import Node
 
 class SinglyNode:
     """Represents a node in a singly linked list.
 
     Attributes:
         data: The data stored in the node.
         next: Reference to the next node in the linked list. Defaults to None.
     """
 
     def __init__(self, data: Any) -> None:
-        self.data: Optional[Any] = data
-        self.next: Optional[SinglyNode] = None
+        self._data: Optional[Any] = data
+        self._next: Optional[SinglyNode] = None
 
-    def __repr__(self):
+    @property
+    def data(self):
+        return self._data
+
+    @data.setter
+    def data(self, value):
+        # all data welcome
+        self._data = value
+
+    @property
+    def next(self):
+        return self._next
+
+    @next.setter
+    def next(self, value):
+        raise AttributeError("Cannot set 'next' attribute directly. Use linked list methods for modification.")
+
+    def __repr__(self) -> str:
+        # when repr is called on a Node with .next,
+        # is next=itsvalue in the return?
         return (
             f"{type(self).__name__}("
             f"data={repr(self.data)}"
             #f", next={repr(self.next)}"
             ")"
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         if hasattr(self.data, "__len__"):
             return (
                 "This node's data is"
                 f" {len(self.data)}"  # type: ignore # noqa
-                f" of type {type(self.data)}."
+                f" of type {type(self.data).__name__}."
             )
-        return f"This node's data is of type {type(self.data)}"
-
-
-if __name__ == "__main__":
-    uni_node = SinglyNode("a string of characters")
+        return f"This node's data is of type {type(self.data).__name__}."
```

