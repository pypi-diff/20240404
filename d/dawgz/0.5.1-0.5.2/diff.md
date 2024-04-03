# Comparing `tmp/dawgz-0.5.1.tar.gz` & `tmp/dawgz-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawgz-0.5.1.tar", last modified: Wed Apr  3 20:58:35 2024, max compression
+gzip compressed data, was "dawgz-0.5.2.tar", last modified: Wed Apr  3 22:14:56 2024, max compression
```

## Comparing `dawgz-0.5.1.tar` & `dawgz-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 20:58:35.574680 dawgz-0.5.1/
--rw-r--r--   0 francois  (1000) francois  (1000)     1072 2024-01-08 18:47:00.000000 dawgz-0.5.1/LICENSE
--rw-r--r--   0 francois  (1000) francois  (1000)     8284 2024-04-03 20:58:35.574680 dawgz-0.5.1/PKG-INFO
--rw-r--r--   0 francois  (1000) francois  (1000)     7433 2024-01-26 14:19:11.000000 dawgz-0.5.1/README.md
-drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 20:58:35.574680 dawgz-0.5.1/dawgz/
--rw-r--r--   0 francois  (1000) francois  (1000)      849 2024-04-03 20:57:05.000000 dawgz-0.5.1/dawgz/__init__.py
--rw-rw-r--   0 francois  (1000) francois  (1000)     1882 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/__main__.py
--rw-rw-r--   0 francois  (1000) francois  (1000)    14399 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/schedulers.py
--rw-rw-r--   0 francois  (1000) francois  (1000)     2363 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/utils.py
--rw-rw-r--   0 francois  (1000) francois  (1000)     6367 2024-04-03 20:55:27.000000 dawgz-0.5.1/dawgz/workflow.py
-drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 20:58:35.574680 dawgz-0.5.1/dawgz.egg-info/
--rw-r--r--   0 francois  (1000) francois  (1000)     8284 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1000) francois  (1000)      314 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1000) francois  (1000)        1 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1000) francois  (1000)       46 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/entry_points.txt
--rw-rw-r--   0 francois  (1000) francois  (1000)       35 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/requires.txt
--rw-rw-r--   0 francois  (1000) francois  (1000)        6 2024-04-03 20:58:35.000000 dawgz-0.5.1/dawgz.egg-info/top_level.txt
--rw-r--r--   0 francois  (1000) francois  (1000)     1019 2024-04-03 20:57:00.000000 dawgz-0.5.1/pyproject.toml
--rw-r--r--   0 francois  (1000) francois  (1000)       35 2024-01-08 18:47:00.000000 dawgz-0.5.1/requirements.txt
--rw-rw-r--   0 francois  (1000) francois  (1000)       38 2024-04-03 20:58:35.574680 dawgz-0.5.1/setup.cfg
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 22:14:56.646526 dawgz-0.5.2/
+-rw-r--r--   0 francois  (1000) francois  (1000)     1072 2024-01-08 18:47:00.000000 dawgz-0.5.2/LICENSE
+-rw-r--r--   0 francois  (1000) francois  (1000)     8284 2024-04-03 22:14:56.642526 dawgz-0.5.2/PKG-INFO
+-rw-r--r--   0 francois  (1000) francois  (1000)     7433 2024-01-26 14:19:11.000000 dawgz-0.5.2/README.md
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 22:14:56.642526 dawgz-0.5.2/dawgz/
+-rw-rw-r--   0 francois  (1000) francois  (1000)      849 2024-04-03 22:14:24.000000 dawgz-0.5.2/dawgz/__init__.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)     1882 2024-04-03 20:55:27.000000 dawgz-0.5.2/dawgz/__main__.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)    14651 2024-04-03 22:14:17.000000 dawgz-0.5.2/dawgz/schedulers.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)     2540 2024-04-03 22:14:17.000000 dawgz-0.5.2/dawgz/utils.py
+-rw-rw-r--   0 francois  (1000) francois  (1000)     6367 2024-04-03 20:55:27.000000 dawgz-0.5.2/dawgz/workflow.py
+drwxrwxr-x   0 francois  (1000) francois  (1000)        0 2024-04-03 22:14:56.642526 dawgz-0.5.2/dawgz.egg-info/
+-rw-r--r--   0 francois  (1000) francois  (1000)     8284 2024-04-03 22:14:56.000000 dawgz-0.5.2/dawgz.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1000) francois  (1000)      314 2024-04-03 22:14:56.000000 dawgz-0.5.2/dawgz.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)        1 2024-04-03 22:14:56.000000 dawgz-0.5.2/dawgz.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)       46 2024-04-03 22:14:56.000000 dawgz-0.5.2/dawgz.egg-info/entry_points.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)       35 2024-04-03 22:14:56.000000 dawgz-0.5.2/dawgz.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)        6 2024-04-03 22:14:56.000000 dawgz-0.5.2/dawgz.egg-info/top_level.txt
+-rw-r--r--   0 francois  (1000) francois  (1000)     1019 2024-04-03 20:57:00.000000 dawgz-0.5.2/pyproject.toml
+-rw-r--r--   0 francois  (1000) francois  (1000)       35 2024-01-08 18:47:00.000000 dawgz-0.5.2/requirements.txt
+-rw-rw-r--   0 francois  (1000) francois  (1000)       38 2024-04-03 22:14:56.646526 dawgz-0.5.2/setup.cfg
```

### Comparing `dawgz-0.5.1/LICENSE` & `dawgz-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dawgz-0.5.1/PKG-INFO` & `dawgz-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgz
-Version: 0.5.1
+Version: 0.5.2
 Summary: Directed Acyclic Workflow Graph Scheduling
 Author: Joeri Hermans
 Author-email: François Rozet <francois.rozet@outlook.com>
 Project-URL: documentation, https://github.com/francois-rozet/dawgz
 Project-URL: source, https://github.com/francois-rozet/dawgz
 Project-URL: tracker, https://github.com/francois-rozet/dawgz/issues
 Keywords: workflow,scheduling,slurm,hpc
```

### Comparing `dawgz-0.5.1/README.md` & `dawgz-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dawgz-0.5.1/dawgz/__init__.py` & `dawgz-0.5.2/dawgz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 r"""Directed Acyclic Workflow Graph Scheduling"""
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 from functools import partial
 from typing import *
 
 from .schedulers import schedule
 from .workflow import Job, leafs, roots
```

### Comparing `dawgz-0.5.1/dawgz/__main__.py` & `dawgz-0.5.2/dawgz/__main__.py`

 * *Files identical despite different names*

### Comparing `dawgz-0.5.1/dawgz/schedulers.py` & `dawgz-0.5.2/dawgz/schedulers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from functools import lru_cache
 from inspect import isawaitable
 from pathlib import Path
 from random import random
 from tabulate import tabulate
 from typing import *
 
-from .utils import comma_separated, eprint, future, pickle, runpickle, trace, slugify
+from .utils import comma_separated, eprint, future, pickle, runpickle, trace, slugify, wrap
 from .workflow import Job, cycles, prune as _prune
 
 
 DIR = os.environ.get('DAWGZ_DIR', '.dawgz')
 DIR = Path(DIR).resolve()
 
 
@@ -117,14 +117,23 @@
             else:
                 array = sorted(job.array)
                 rows = [
                     (f'{job.name}[{i}]', self.state(job, i), self.output(job, i))
                     for i in array
                 ]
 
+            rows = [
+                (
+                    name,
+                    state,
+                    None if output is None else wrap(output, width=120),
+                )
+                for name, state, output in rows
+            ]
+
             return tabulate(rows, headers, showindex=array)
 
     def cancel(self, job: Job = None) -> str:
         raise NotImplementedError(f"'cancel' is not implemented for the {self.backend} backend.")
 
     @contextmanager
     def context(self):
```

### Comparing `dawgz-0.5.1/dawgz/utils.py` & `dawgz-0.5.2/dawgz/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,7 +96,15 @@
     lines = traceback.format_exception(
         type(error),
         error,
         error.__traceback__,
     )
 
     return ''.join(lines).strip('\n')
+
+
+def wrap(text: str, width: int) -> str:
+    return '\n'.join(
+        line[i:i + width]
+        for line in text.split('\n')
+        for i in range(0, len(line), width)
+    )
```

### Comparing `dawgz-0.5.1/dawgz/workflow.py` & `dawgz-0.5.2/dawgz/workflow.py`

 * *Files identical despite different names*

### Comparing `dawgz-0.5.1/dawgz.egg-info/PKG-INFO` & `dawgz-0.5.2/dawgz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawgz
-Version: 0.5.1
+Version: 0.5.2
 Summary: Directed Acyclic Workflow Graph Scheduling
 Author: Joeri Hermans
 Author-email: François Rozet <francois.rozet@outlook.com>
 Project-URL: documentation, https://github.com/francois-rozet/dawgz
 Project-URL: source, https://github.com/francois-rozet/dawgz
 Project-URL: tracker, https://github.com/francois-rozet/dawgz/issues
 Keywords: workflow,scheduling,slurm,hpc
```

### Comparing `dawgz-0.5.1/pyproject.toml` & `dawgz-0.5.2/pyproject.toml`

 * *Files identical despite different names*

