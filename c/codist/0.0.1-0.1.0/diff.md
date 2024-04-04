# Comparing `tmp/codist-0.0.1.tar.gz` & `tmp/codist-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codist-0.0.1.tar", last modified: Wed Apr  3 04:51:07 2024, max compression
+gzip compressed data, was "codist-0.1.0.tar", last modified: Thu Apr  4 10:38:10 2024, max compression
```

## Comparing `codist-0.0.1.tar` & `codist-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-03 04:51:07.814084 codist-0.0.1/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3348 2024-04-03 04:51:07.813878 codist-0.0.1/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2965 2024-04-03 04:37:29.000000 codist-0.0.1/README.md
--rw-r--r--   0 jfin305  (1356368322) 1403514002      635 2024-04-03 04:51:04.000000 codist-0.0.1/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-03 04:51:07.814128 codist-0.0.1/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-03 04:51:07.811268 codist-0.0.1/src/
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-03 04:51:07.812368 codist-0.0.1/src/codist/
--rw-r--r--   0 jfin305  (1356368322) 1403514002       24 2024-04-03 04:37:29.000000 codist-0.0.1/src/codist/__init__.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002      540 2024-04-03 04:37:29.000000 codist-0.0.1/src/codist/ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2967 2024-04-03 04:37:29.000000 codist-0.0.1/src/codist/distance.py
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-03 04:51:07.813693 codist-0.0.1/src/codist.egg-info/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3348 2024-04-03 04:51:07.000000 codist-0.0.1/src/codist.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002      265 2024-04-03 04:51:07.000000 codist-0.0.1/src/codist.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-03 04:51:07.000000 codist-0.0.1/src/codist.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-03 04:51:07.000000 codist-0.0.1/src/codist.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-03 04:51:07.813421 codist-0.0.1/tests/
--rw-r--r--   0 jfin305  (1356368322) 1403514002      452 2024-04-03 00:56:51.000000 codist-0.0.1/tests/test_ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2492 2024-04-03 00:45:49.000000 codist-0.0.1/tests/test_distance.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.963887 codist-0.1.0/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-04 10:38:10.963688 codist-0.1.0/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3446 2024-04-04 10:33:01.000000 codist-0.1.0/README.md
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      561 2024-04-04 10:38:08.000000 codist-0.1.0/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-04 10:38:10.963929 codist-0.1.0/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.960588 codist-0.1.0/src/
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.961963 codist-0.1.0/src/codist/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002       44 2024-04-04 10:36:12.000000 codist-0.1.0/src/codist/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      547 2024-04-04 03:48:03.000000 codist-0.1.0/src/codist/ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     6319 2024-04-04 10:19:05.000000 codist-0.1.0/src/codist/distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     1721 2024-04-04 10:12:00.000000 codist-0.1.0/src/codist/tree.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.963501 codist-0.1.0/src/codist.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      304 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-04 10:38:10.000000 codist-0.1.0/src/codist.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-04 10:38:10.963212 codist-0.1.0/tests/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      350 2024-04-04 03:47:43.000000 codist-0.1.0/tests/test_ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     2654 2024-04-04 07:20:13.000000 codist-0.1.0/tests/test_distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     1204 2024-04-04 10:36:27.000000 codist-0.1.0/tests/test_trees.py
```

### Comparing `codist-0.0.1/README.md` & `codist-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+Metadata-Version: 2.1
+Name: codist
+Version: 0.1.0
+Summary: AST edit distance
+Project-URL: repository, https://github.com/James-Ansley/codist
+Classifier: Development Status :: 1 - Planning
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+
 # CoDist
 
 CoDist (Code Distance) is a library that provides functions to calculate the
-edit distance of abstract syntax trees.
+edit distance and edit paths of abstract syntax trees.
 
 While this library is primarily concerned with AST edit distances, it can handle
-any generic tree of the form: `Tree[T] = tuple[T, tuple[Tree[T], ...]]` or
-forest of the form: `Forest[T] = tuple[Tree[T], ...]`.
-
-To compare the distances of trees use `codist.tree_dist` and for forests,
-use `codist.forest_dist`.
+any generic tree of the form: `Tree[T] = tuple[T, tuple[Tree[T], ...]]`
 
 ## Install
 
 ```
 pip install codist
 ```
 
 ## Usage
 
 Currently, only AST node _type_ information is compared. A silhouette of an AST
 (an AST containing only type information) is constructed with
-the `parse_ast_silhouette` function. The distance between two ASTs can be
-calculated with the `tree_dist` function.
+the `parse_ast_silhouette` function.
 
 ```python
 from pprint import pprint
-
-from codist import tree_dist
 from codist.ast import parse_ast_silhouette
 
 code1 = """
 def process(data):
     result = []
     for x in data:
         if x > 5:
@@ -46,24 +51,21 @@
             result += [x]
     return result
 """
 
 ast1 = parse_ast_silhouette(code1)
 ast2 = parse_ast_silhouette(code2)
 
-dist = tree_dist(ast1, ast2)
-
 pprint(ast1)
 pprint(ast2)
-print("The above trees have a distance of:", dist)
 ```
 
-Would print:
+Which prints:
 
-```text
+```
 ('Module',
  (('FunctionDef',
    (('arguments', (('arg', ()),)),
     ('Assign', (('Name', (('Store', ()),)), ('List', (('Load', ()),)))),
     ('For',
      (('Name', (('Store', ()),)),
       ('Name', (('Load', ()),)),
@@ -84,15 +86,57 @@
       ('If',
        (('Compare', (('Name', (('Load', ()),)), ('GtE', ()), ('Constant', ()))),
         ('AugAssign',
          (('Name', (('Store', ()),)),
           ('Add', ()),
           ('List', (('Name', (('Load', ()),)), ('Load', ()))))))))),
     ('Return', (('Name', (('Load', ()),)),)))),))
+```
+
+The distance between two ASTs can be computed with the `tree_dist` function.
+
+```python
+from codist import tree_dist
+
+print("The above trees have a distance of:", tree_dist(ast1, ast2))
+```
+
+Would print:
+
+```text
+The above trees have a distance of: 8
+```
+
+The edit path and distance between two trees can be computed with
+the `tree_edit` function. For convenience, this function also computes the
+edit distance:
+
+```python
+from codist import tree_edit
+
+dist, path = tree_edit(ast1, ast2)
+print("The above trees have a distance of:", dist)
+print("And an edit path of:")
+pprint(tuple(e for e in path if e[0] != e[1]))
+```
+
+which prints:
+
+
+```
 The above trees have a distance of: 8
+And an edit path of:
+(('Gt', 'GtE'),
+ ('Load', 'Store'),
+ ('Load', 'Add'),
+ ('Attribute', 'Λ'),
+ ('Λ', 'Load'),
+ ('Λ', 'List'),
+ ('Call', 'AugAssign'),
+ ('Expr', 'Λ'))
 ```
 
 A custom set of `Cost` functions can be provided to change the weights of
 insertions, deletions, and relabelings. By default, all change operations are 1
 except for the case of γ(a -> a) which is 0. To change the cost, construct
 a `Cost` object:
```

### Comparing `codist-0.0.1/pyproject.toml` & `codist-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codist"
-version = "0.0.1"
+version = "0.1.0"
 description = "AST edit distance"
 
 readme = "README.md"
 requires-python = ">=3.12"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -17,12 +17,9 @@
     "License :: OSI Approved :: MIT License",
 ]
 dynamic = ["dependencies"]
 
 [project.urls]
 repository = "https://github.com/James-Ansley/codist"
 
-[tool.setuptools.dynamic]
-dependencies = { file = ["requirements.txt"] }
-
 [tool.setuptools.packages.find]
 where = ["src"]
```

