# Comparing `tmp/pipe-2.1.tar.gz` & `tmp/pipe-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipe-2.1.tar", last modified: Wed Dec 20 20:54:57 2023, max compression
+gzip compressed data, was "pipe-2.2.tar", last modified: Thu Apr  4 06:37:14 2024, max compression
```

## Comparing `pipe-2.1.tar` & `pipe-2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-12-20 20:54:57.807548 pipe-2.1/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1070 2023-12-01 23:21:46.000000 pipe-2.1/LICENSE
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16577 2023-12-20 20:54:57.807548 pipe-2.1/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15849 2023-12-20 20:52:50.000000 pipe-2.1/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-12-20 20:54:57.807548 pipe-2.1/pipe.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16577 2023-12-20 20:54:57.000000 pipe-2.1/pipe.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      171 2023-12-20 20:54:57.000000 pipe-2.1/pipe.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-12-20 20:54:57.000000 pipe-2.1/pipe.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        5 2023-12-20 20:54:57.000000 pipe-2.1/pipe.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4740 2023-12-20 20:52:50.000000 pipe-2.1/pipe.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)      947 2023-12-20 08:02:31.000000 pipe-2.1/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-12-20 20:54:57.807548 pipe-2.1/setup.cfg
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-12-20 20:54:57.803548 pipe-2.1/tests/
--rw-r--r--   0 mdk       (1000) mdk       (1000)      719 2023-12-20 20:52:50.000000 pipe-2.1/tests/test_pipe.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2024-04-04 06:37:14.070414 pipe-2.2/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1070 2023-12-01 23:21:46.000000 pipe-2.2/LICENSE
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17441 2024-04-04 06:37:14.070414 pipe-2.2/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16713 2024-04-04 06:34:28.000000 pipe-2.2/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2024-04-04 06:37:14.070414 pipe-2.2/pipe.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17441 2024-04-04 06:37:14.000000 pipe-2.2/pipe.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      171 2024-04-04 06:37:14.000000 pipe-2.2/pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2024-04-04 06:37:14.000000 pipe-2.2/pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        5 2024-04-04 06:37:14.000000 pipe-2.2/pipe.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4846 2024-04-04 06:35:57.000000 pipe-2.2/pipe.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      947 2024-04-04 06:34:24.000000 pipe-2.2/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2024-04-04 06:37:14.070414 pipe-2.2/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2024-04-04 06:37:14.070414 pipe-2.2/tests/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      863 2024-04-04 06:34:24.000000 pipe-2.2/tests/test_pipe.py
```

### Comparing `pipe-2.1/LICENSE` & `pipe-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipe-2.1/PKG-INFO` & `pipe-2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipe
-Version: 2.1
+Version: 2.2
 Summary: Module enabling a sh like infix syntax (using pipes)
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: repository, https://github.com/JulienPalard/Pipe
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 
 # Pipe — Infix programming toolkit
 
 [![PyPI](https://img.shields.io/pypi/v/pipe)
  ![Monthly downloads](https://img.shields.io/pypi/dm/pipe)
  ![Supported Python Version](https://img.shields.io/pypi/pyversions/pipe.svg)
 ](https://pypi.org/project/pipe)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/JulienPalard/pipe/tests.yml?branch=main)](https://github.com/JulienPalard/pipe/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JulienPalard/pipe/tests.yml?branch=main)](https://github.com/JulienPalard/pipe/actions)
 
 Module enabling a sh like infix syntax (using pipes).
 
 
 # Introduction
 
 As an example, here is the solution for the [2nd Euler Project
@@ -549,14 +549,48 @@
 [0, 0.5, 1.5, 2.5, 3.5, 4.5, 5.5, 6.5, 7.5, 8.5, 9.5, 10.5, 11.5, 12.5, 13.5, 14.5, 15.5, 16.5, 17.5, 18.5]
 >>> list(range(20) | running_average(width=10))
 [0, 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5.5, 6.5, 7.5, 8.5, 9.5, 10.5, 11.5, 12.5, 13.5, 14.5]
 >>>
 ```
 
 
+## One-off pipes
+
+Sometimes you just want a one-liner, when creating a pipe you can specify the function's positional and named arguments directly
+
+```python
+>>> from itertools import combinations
+
+>>> list(range(5) | Pipe(combinations, 2))
+[(0, 1), (0, 2), (0, 3), (0, 4), (1, 2), (1, 3), (1, 4), (2, 3), (2, 4), (3, 4)]
+>>>
+```
+
+a simple running sum with initial starting value
+
+```python
+>>> from itertools import accumulate
+
+>>> list(range(10) | Pipe(accumulate, initial=1))
+[1, 1, 2, 4, 7, 11, 16, 22, 29, 37, 46]
+>>>
+```
+
+or filter your data based on some criteria
+
+```python
+>>> from itertools import compress
+
+list(range(20) | Pipe(compress, selectors=[1, 0] * 10))
+[0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
+>>> list(range(20) | Pipe(compress, selectors=[0, 1] * 10))
+[1, 3, 5, 7, 9, 11, 13, 15, 17, 19]
+>>>
+```
+
 ## Euler project samples
 
 > Find the sum of all the multiples of 3 or 5 below 1000.
 
 ```python
 >>> sum(count() | where(lambda x: x % 3 == 0 or x % 5 == 0) | take_while(lambda x: x < 1000))
 233168
@@ -593,14 +627,15 @@
 >>>
 ```
 
 For multi-argument pipes then can be partially initialized, you can think of curying:
 
 ```python
 some_iterable | some_pipe(1, 2, 3)
+some_iterable | Pipe(some_func, 1, 2, 3)
 ```
 
 is strictly equivalent to:
 
 ```python
 some_iterable | some_pipe(1)(2)(3)
 ```
```

### Comparing `pipe-2.1/README.md` & `pipe-2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Pipe — Infix programming toolkit
 
 [![PyPI](https://img.shields.io/pypi/v/pipe)
  ![Monthly downloads](https://img.shields.io/pypi/dm/pipe)
  ![Supported Python Version](https://img.shields.io/pypi/pyversions/pipe.svg)
 ](https://pypi.org/project/pipe)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/JulienPalard/pipe/tests.yml?branch=main)](https://github.com/JulienPalard/pipe/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JulienPalard/pipe/tests.yml?branch=main)](https://github.com/JulienPalard/pipe/actions)
 
 Module enabling a sh like infix syntax (using pipes).
 
 
 # Introduction
 
 As an example, here is the solution for the [2nd Euler Project
@@ -530,14 +530,48 @@
 [0, 0.5, 1.5, 2.5, 3.5, 4.5, 5.5, 6.5, 7.5, 8.5, 9.5, 10.5, 11.5, 12.5, 13.5, 14.5, 15.5, 16.5, 17.5, 18.5]
 >>> list(range(20) | running_average(width=10))
 [0, 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5.5, 6.5, 7.5, 8.5, 9.5, 10.5, 11.5, 12.5, 13.5, 14.5]
 >>>
 ```
 
 
+## One-off pipes
+
+Sometimes you just want a one-liner, when creating a pipe you can specify the function's positional and named arguments directly
+
+```python
+>>> from itertools import combinations
+
+>>> list(range(5) | Pipe(combinations, 2))
+[(0, 1), (0, 2), (0, 3), (0, 4), (1, 2), (1, 3), (1, 4), (2, 3), (2, 4), (3, 4)]
+>>>
+```
+
+a simple running sum with initial starting value
+
+```python
+>>> from itertools import accumulate
+
+>>> list(range(10) | Pipe(accumulate, initial=1))
+[1, 1, 2, 4, 7, 11, 16, 22, 29, 37, 46]
+>>>
+```
+
+or filter your data based on some criteria
+
+```python
+>>> from itertools import compress
+
+list(range(20) | Pipe(compress, selectors=[1, 0] * 10))
+[0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
+>>> list(range(20) | Pipe(compress, selectors=[0, 1] * 10))
+[1, 3, 5, 7, 9, 11, 13, 15, 17, 19]
+>>>
+```
+
 ## Euler project samples
 
 > Find the sum of all the multiples of 3 or 5 below 1000.
 
 ```python
 >>> sum(count() | where(lambda x: x % 3 == 0 or x % 5 == 0) | take_while(lambda x: x < 1000))
 233168
@@ -574,14 +608,15 @@
 >>>
 ```
 
 For multi-argument pipes then can be partially initialized, you can think of curying:
 
 ```python
 some_iterable | some_pipe(1, 2, 3)
+some_iterable | Pipe(some_func, 1, 2, 3)
 ```
 
 is strictly equivalent to:
 
 ```python
 some_iterable | some_pipe(1)(2)(3)
 ```
```

### Comparing `pipe-2.1/pipe.egg-info/PKG-INFO` & `pipe-2.2/pipe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipe
-Version: 2.1
+Version: 2.2
 Summary: Module enabling a sh like infix syntax (using pipes)
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: repository, https://github.com/JulienPalard/Pipe
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 
 # Pipe — Infix programming toolkit
 
 [![PyPI](https://img.shields.io/pypi/v/pipe)
  ![Monthly downloads](https://img.shields.io/pypi/dm/pipe)
  ![Supported Python Version](https://img.shields.io/pypi/pyversions/pipe.svg)
 ](https://pypi.org/project/pipe)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/JulienPalard/pipe/tests.yml?branch=main)](https://github.com/JulienPalard/pipe/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/JulienPalard/pipe/tests.yml?branch=main)](https://github.com/JulienPalard/pipe/actions)
 
 Module enabling a sh like infix syntax (using pipes).
 
 
 # Introduction
 
 As an example, here is the solution for the [2nd Euler Project
@@ -549,14 +549,48 @@
 [0, 0.5, 1.5, 2.5, 3.5, 4.5, 5.5, 6.5, 7.5, 8.5, 9.5, 10.5, 11.5, 12.5, 13.5, 14.5, 15.5, 16.5, 17.5, 18.5]
 >>> list(range(20) | running_average(width=10))
 [0, 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4, 4.5, 5.5, 6.5, 7.5, 8.5, 9.5, 10.5, 11.5, 12.5, 13.5, 14.5]
 >>>
 ```
 
 
+## One-off pipes
+
+Sometimes you just want a one-liner, when creating a pipe you can specify the function's positional and named arguments directly
+
+```python
+>>> from itertools import combinations
+
+>>> list(range(5) | Pipe(combinations, 2))
+[(0, 1), (0, 2), (0, 3), (0, 4), (1, 2), (1, 3), (1, 4), (2, 3), (2, 4), (3, 4)]
+>>>
+```
+
+a simple running sum with initial starting value
+
+```python
+>>> from itertools import accumulate
+
+>>> list(range(10) | Pipe(accumulate, initial=1))
+[1, 1, 2, 4, 7, 11, 16, 22, 29, 37, 46]
+>>>
+```
+
+or filter your data based on some criteria
+
+```python
+>>> from itertools import compress
+
+list(range(20) | Pipe(compress, selectors=[1, 0] * 10))
+[0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
+>>> list(range(20) | Pipe(compress, selectors=[0, 1] * 10))
+[1, 3, 5, 7, 9, 11, 13, 15, 17, 19]
+>>>
+```
+
 ## Euler project samples
 
 > Find the sum of all the multiples of 3 or 5 below 1000.
 
 ```python
 >>> sum(count() | where(lambda x: x % 3 == 0 or x % 5 == 0) | take_while(lambda x: x < 1000))
 233168
@@ -593,14 +627,15 @@
 >>>
 ```
 
 For multi-argument pipes then can be partially initialized, you can think of curying:
 
 ```python
 some_iterable | some_pipe(1, 2, 3)
+some_iterable | Pipe(some_func, 1, 2, 3)
 ```
 
 is strictly equivalent to:
 
 ```python
 some_iterable | some_pipe(1)(2)(3)
 ```
```

### Comparing `pipe-2.1/pipe.py` & `pipe-2.2/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Library allowing a sh like infix syntax using pipes."""
 
 __author__ = "Julien Palard <julien@python.org>"
-__version__ = "2.1"
+__version__ = "2.2"
 __credits__ = """Jérôme Schneider for teaching me the Python datamodel,
 and all contributors."""
 
 import functools
 import itertools
 import socket
 import sys
@@ -28,16 +28,18 @@
     Described as :
     select = Pipe(lambda iterable, pred: (pred(x) for x in iterable))
     and used as :
     print [1, 2, 3] | select(lambda x: x * 2)
     # 2, 4, 6
     """
 
-    def __init__(self, function):
-        self.function = function
+    def __init__(self, function, *args, **kwargs):
+        self.function = lambda iterable, *args2, **kwargs2: function(
+            iterable, *args, *args2, **kwargs, **kwargs2
+        )
         functools.update_wrapper(self, function)
 
     def __ror__(self, other):
         return self.function(other)
 
     def __call__(self, *args, **kwargs):
         return Pipe(
@@ -106,16 +108,15 @@
 enumerate = Pipe(builtins.enumerate)
 
 
 @Pipe
 def permutations(iterable, r=None):
     # permutations('ABCD', 2) --> AB AC AD BA BC BD CA CB CD DA DB DC
     # permutations(range(3)) --> 012 021 102 120 201 210
-    for x in itertools.permutations(iterable, r):
-        yield x
+    yield from itertools.permutations(iterable, r)
 
 
 @Pipe
 def netcat(to_send, host, port):
     """Send and receive bytes over TCP."""
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
         s.connect((host, port))
```

### Comparing `pipe-2.1/pyproject.toml` & `pipe-2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipe-2.1/tests/test_pipe.py` & `pipe-2.2/tests/test_pipe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import pipe
 
 
 def test_uniq():
     assert list(() | pipe.uniq) == []
 
 
+def test_take_zero():
+    assert list([1, 2, 3] | pipe.take(0)) == []
+
+
+def test_take_one():
+    assert list([1, 2, 3] | pipe.take(1)) == [1]
+
+
 def test_empty_iterable():
     assert list([] | pipe.take(999)) == []
 
 
 def test_aliasing():
     is_even = pipe.where(lambda x: not x % 2)
```

