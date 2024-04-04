# Comparing `tmp/mutmut-2.4.4.tar.gz` & `tmp/mutmut-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutmut-2.4.4.tar", last modified: Thu Aug 31 06:30:37 2023, max compression
+gzip compressed data, was "mutmut-2.4.5.tar", last modified: Thu Apr  4 07:16:13 2024, max compression
```

## Comparing `mutmut-2.4.4.tar` & `mutmut-2.4.5.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-08-31 06:30:37.137989 mutmut-2.4.4/
--rw-r--r--   0 boxed      (501) staff       (20)     1007 2023-08-31 06:27:26.000000 mutmut-2.4.4/AUTHORS.rst
--rw-r--r--   0 boxed      (501) staff       (20)    12956 2023-08-31 06:30:04.000000 mutmut-2.4.4/HISTORY.rst
--rw-r--r--   0 boxed      (501) staff       (20)     1471 2021-07-21 11:45:51.000000 mutmut-2.4.4/LICENSE
--rw-r--r--   0 boxed      (501) staff       (20)      110 2021-07-21 11:45:51.000000 mutmut-2.4.4/MANIFEST.in
--rw-r--r--   0 boxed      (501) staff       (20)    17748 2023-08-31 06:30:37.138119 mutmut-2.4.4/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)    14120 2023-08-31 06:27:26.000000 mutmut-2.4.4/README.rst
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-08-31 06:30:37.136274 mutmut-2.4.4/mutmut/
--rw-r--r--   0 boxed      (501) staff       (20)    43494 2023-08-31 06:30:14.000000 mutmut-2.4.4/mutmut/__init__.py
--rw-r--r--   0 boxed      (501) staff       (20)    17993 2023-08-31 06:27:26.000000 mutmut-2.4.4/mutmut/__main__.py
--rw-r--r--   0 boxed      (501) staff       (20)    18153 2023-08-31 06:27:26.000000 mutmut-2.4.4/mutmut/cache.py
-drwxr-xr-x   0 boxed      (501) staff       (20)        0 2023-08-31 06:30:37.137888 mutmut-2.4.4/mutmut.egg-info/
--rw-r--r--   0 boxed      (501) staff       (20)    17748 2023-08-31 06:30:37.000000 mutmut-2.4.4/mutmut.egg-info/PKG-INFO
--rw-r--r--   0 boxed      (501) staff       (20)      383 2023-08-31 06:30:37.000000 mutmut-2.4.4/mutmut.egg-info/SOURCES.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2023-08-31 06:30:37.000000 mutmut-2.4.4/mutmut.egg-info/dependency_links.txt
--rw-r--r--   0 boxed      (501) staff       (20)       52 2023-08-31 06:30:37.000000 mutmut-2.4.4/mutmut.egg-info/entry_points.txt
--rw-r--r--   0 boxed      (501) staff       (20)        1 2021-07-21 11:54:27.000000 mutmut-2.4.4/mutmut.egg-info/not-zip-safe
--rw-r--r--   0 boxed      (501) staff       (20)      124 2023-08-31 06:30:37.000000 mutmut-2.4.4/mutmut.egg-info/requires.txt
--rw-r--r--   0 boxed      (501) staff       (20)        7 2023-08-31 06:30:37.000000 mutmut-2.4.4/mutmut.egg-info/top_level.txt
--rw-r--r--   0 boxed      (501) staff       (20)       46 2023-08-31 06:27:30.000000 mutmut-2.4.4/requirements.txt
--rw-r--r--   0 boxed      (501) staff       (20)      375 2023-08-31 06:30:37.138393 mutmut-2.4.4/setup.cfg
--rwxr-xr-x   0 boxed      (501) staff       (20)     3621 2023-08-31 06:27:26.000000 mutmut-2.4.4/setup.py
--rw-r--r--   0 boxed      (501) staff       (20)       67 2021-07-21 11:45:51.000000 mutmut-2.4.4/test_requirements.txt
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.526012 mutmut-2.4.5/
+-rw-r--r--   0 boxed      (501) staff       (20)     1345 2024-04-04 07:15:09.000000 mutmut-2.4.5/AUTHORS.rst
+-rw-r--r--   0 boxed      (501) staff       (20)    13241 2024-04-04 07:12:53.000000 mutmut-2.4.5/HISTORY.rst
+-rw-r--r--   0 boxed      (501) staff       (20)     1471 2021-07-21 11:45:51.000000 mutmut-2.4.5/LICENSE
+-rw-r--r--   0 boxed      (501) staff       (20)      110 2021-07-21 11:45:51.000000 mutmut-2.4.5/MANIFEST.in
+-rw-r--r--   0 boxed      (501) staff       (20)    18267 2024-04-04 07:16:13.526171 mutmut-2.4.5/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)    14511 2024-04-04 07:11:00.000000 mutmut-2.4.5/README.rst
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.523447 mutmut-2.4.5/mutmut/
+-rw-r--r--   0 boxed      (501) staff       (20)    42440 2024-04-04 07:13:03.000000 mutmut-2.4.5/mutmut/__init__.py
+-rw-r--r--   0 boxed      (501) staff       (20)    19122 2024-04-04 07:11:00.000000 mutmut-2.4.5/mutmut/__main__.py
+-rw-r--r--   0 boxed      (501) staff       (20)    18528 2024-04-04 07:11:00.000000 mutmut-2.4.5/mutmut/cache.py
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.524667 mutmut-2.4.5/mutmut.egg-info/
+-rw-r--r--   0 boxed      (501) staff       (20)    18267 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/PKG-INFO
+-rw-r--r--   0 boxed      (501) staff       (20)      464 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/SOURCES.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/dependency_links.txt
+-rw-r--r--   0 boxed      (501) staff       (20)       52 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/entry_points.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        1 2021-07-21 11:54:27.000000 mutmut-2.4.5/mutmut.egg-info/not-zip-safe
+-rw-r--r--   0 boxed      (501) staff       (20)      124 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/requires.txt
+-rw-r--r--   0 boxed      (501) staff       (20)        7 2024-04-04 07:16:13.000000 mutmut-2.4.5/mutmut.egg-info/top_level.txt
+-rw-r--r--   0 boxed      (501) staff       (20)       46 2024-04-04 07:08:51.000000 mutmut-2.4.5/requirements.txt
+-rw-r--r--   0 boxed      (501) staff       (20)      375 2024-04-04 07:16:13.526599 mutmut-2.4.5/setup.cfg
+-rwxr-xr-x   0 boxed      (501) staff       (20)     3621 2024-04-04 07:08:54.000000 mutmut-2.4.5/setup.py
+-rw-r--r--   0 boxed      (501) staff       (20)       67 2021-07-21 11:45:51.000000 mutmut-2.4.5/test_requirements.txt
+drwxr-xr-x   0 boxed      (501) staff       (20)        0 2024-04-04 07:16:13.525750 mutmut-2.4.5/tests/
+-rw-r--r--   0 boxed      (501) staff       (20)      914 2021-07-21 11:45:51.000000 mutmut-2.4.5/tests/test_cache.py
+-rw-r--r--   0 boxed      (501) staff       (20)     5117 2024-04-04 07:08:54.000000 mutmut-2.4.5/tests/test_init.py
+-rw-r--r--   0 boxed      (501) staff       (20)    24908 2024-04-04 07:11:00.000000 mutmut-2.4.5/tests/test_main.py
+-rw-r--r--   0 boxed      (501) staff       (20)    13133 2024-04-04 07:08:54.000000 mutmut-2.4.5/tests/test_mutation.py
```

### Comparing `mutmut-2.4.4/AUTHORS.rst` & `mutmut-2.4.5/AUTHORS.rst`

 * *Files 20% similar despite different names*

```diff
@@ -24,7 +24,15 @@
 * Andreas Finkler <andi.finkler@gmail.com>
 * sed-i
 * Peter Hill <peter.hill@york.ac.uk>
 * Samuel Razzell <srazzell@apple.com>
 * Daniel Versoza Alves <daniel.alves@voxy.com>
 * Zac Hatfield-Dodds <zac.hatfield.dodds@gmail.com>
 * Jan Królikowski <yanekk86@gmail.com>
+* Tal Amuyal <talamuyal@gmail.com>
+* Eivind Jahren <eivind.jahren@gmail.com>
+* WiredNerd <pbuschmail-gitlab@yahoo.com>
+* Kees Hink <kees@fourdigits.nl>
+* Jim Rybarski <jim@rybarski.com>
+* Christopher J. Brody <chris.brody+brodybits@gmail.com>
+* Century-ss <hgfc7543ggfdch@gmail.com>
+* Michael Champagne <michael.champagne@elapsetech.com>
```

### Comparing `mutmut-2.4.4/HISTORY.rst` & `mutmut-2.4.5/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 ---------
 
+2.4.5
+~~~~~
+
+* Add skipped column in html index report
+
+* Untested/skipped in show all does not show skipped
+
+* mutmut should pick up the config before running the original tests. That allows to specify test suits you want to run
+
+* improved some high-level help text & documentation
+
 2.4.4
 ~~~~~
 
 * Fix issue with `TypeError` for empty file diffs
 
 * Introduce mutation of f-strings
```

### Comparing `mutmut-2.4.4/LICENSE` & `mutmut-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mutmut-2.4.4/PKG-INFO` & `mutmut-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutmut
-Version: 2.4.4
+Version: 2.4.5
 Summary: mutation testing for Python 3
 Home-page: https://github.com/boxed/mutmut
 Author: Anders Hovmöller
 Author-email: boxed@killingar.net
 License: BSD
 Description: mutmut - python mutation tester
         ===============================
@@ -52,34 +52,50 @@
         .. code-block:: console
         
             pip install mutmut
             mutmut run
         
         This will by default run pytest (or unittest if pytest is unavailable)
         on tests in the "tests" or "test" folder and
-        it will try to figure out where the code to mutate lies. Run
+        it will try to figure out where the code to mutate lies.
+        
+        NOTE that mutmut will apply the mutations directly, one at a time;
+        it is **highly** recommended to add all changes to source control
+        before running.
+        
+        Enter
         
         .. code-block:: console
         
-            mutmut --help
+            mutmut run --help
         
         for the available flags, to use other runners, etc. The recommended way to use
-        mutmut if the defaults aren't working for you is to add a block in ``setup.cfg``.
+        mutmut if the defaults aren't working for you is to add a
+        block in ``setup.cfg`` or ``project.toml``.
         Then when you come back to mutmut weeks later you don't have to figure out the
-        flags again, just run ``mutmut run`` and it works. Like this:
+        flags again, just run ``mutmut run`` and it works.
+        Like this in ``setup.cfg``:
         
         .. code-block:: ini
         
             [mutmut]
             paths_to_mutate=src/
             backup=False
             runner=python -m hammett -x
             tests_dir=tests/
             dict_synonyms=Struct, NamedStruct
         
+        or like this in ``pyproject.toml``:
+        
+        .. code-block:: ini
+        
+            [tool.mutmut]
+            paths_to_mutate="src"
+            runner="python -m hammett -x"
+        
         To use multiple paths either in the ``paths_to_mutate`` or ``tests_dir`` option
         use a comma or colon separated list. For example:
         
         .. code-block:: ini
         
             [mutmut]
             paths_to_mutate=src/,src2/
@@ -90,19 +106,19 @@
         test suite changes.
         
         To print the results run ``mutmut show``. It will give you a list of the mutants
         grouped by file. You can now look at a specific mutant diff with ``mutmut show 3``,
         all mutants for a specific file with ``mutmut show path/to/file.py`` or all mutants
         with ``mutmut show all``.
         
-        
         You can also write a mutant to disk with ``mutmut apply 3``. You should **REALLY**
         have the file you mutate under source code control and committed before you apply
         a mutant!
         
+        To generate a HTML report for a web browser: ``mutmut html``
         
         Whitelisting
         ------------
         
         You can mark lines like this:
         
         .. code-block:: python
```

### Comparing `mutmut-2.4.4/README.rst` & `mutmut-2.4.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -44,34 +44,50 @@
 .. code-block:: console
 
     pip install mutmut
     mutmut run
 
 This will by default run pytest (or unittest if pytest is unavailable)
 on tests in the "tests" or "test" folder and
-it will try to figure out where the code to mutate lies. Run
+it will try to figure out where the code to mutate lies.
+
+NOTE that mutmut will apply the mutations directly, one at a time;
+it is **highly** recommended to add all changes to source control
+before running.
+
+Enter
 
 .. code-block:: console
 
-    mutmut --help
+    mutmut run --help
 
 for the available flags, to use other runners, etc. The recommended way to use
-mutmut if the defaults aren't working for you is to add a block in ``setup.cfg``.
+mutmut if the defaults aren't working for you is to add a
+block in ``setup.cfg`` or ``project.toml``.
 Then when you come back to mutmut weeks later you don't have to figure out the
-flags again, just run ``mutmut run`` and it works. Like this:
+flags again, just run ``mutmut run`` and it works.
+Like this in ``setup.cfg``:
 
 .. code-block:: ini
 
     [mutmut]
     paths_to_mutate=src/
     backup=False
     runner=python -m hammett -x
     tests_dir=tests/
     dict_synonyms=Struct, NamedStruct
 
+or like this in ``pyproject.toml``:
+
+.. code-block:: ini
+
+    [tool.mutmut]
+    paths_to_mutate="src"
+    runner="python -m hammett -x"
+
 To use multiple paths either in the ``paths_to_mutate`` or ``tests_dir`` option
 use a comma or colon separated list. For example:
 
 .. code-block:: ini
 
     [mutmut]
     paths_to_mutate=src/,src2/
@@ -82,19 +98,19 @@
 test suite changes.
 
 To print the results run ``mutmut show``. It will give you a list of the mutants
 grouped by file. You can now look at a specific mutant diff with ``mutmut show 3``,
 all mutants for a specific file with ``mutmut show path/to/file.py`` or all mutants
 with ``mutmut show all``.
 
-
 You can also write a mutant to disk with ``mutmut apply 3``. You should **REALLY**
 have the file you mutate under source code control and committed before you apply
 a mutant!
 
+To generate a HTML report for a web browser: ``mutmut html``
 
 Whitelisting
 ------------
 
 You can mark lines like this:
 
 .. code-block:: python
```

### Comparing `mutmut-2.4.4/mutmut/__init__.py` & `mutmut-2.4.5/mutmut/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import fnmatch
 import itertools
 import multiprocessing
 import os
 import re
 import shlex
 import subprocess
 import sys
 import toml
 from configparser import ConfigParser
 from copy import copy as copy_obj
+from dataclasses import dataclass, field
 from functools import wraps
 from io import (
     open,
     TextIOBase,
 )
 from os.path import isdir
 from shutil import (
@@ -21,54 +24,46 @@
     copy,
 )
 from threading import (
     Timer,
     Thread,
 )
 from time import time
+from typing import Callable, Dict, Iterator, List, Optional, Set, Tuple
 
 from parso import parse
 from parso.python.tree import Name, Number, Keyword, FStringStart, FStringEnd
 
-__version__ = '2.4.4'
+__version__ = '2.4.5'
 
 
 if os.getcwd() not in sys.path:
     sys.path.insert(0, os.getcwd())
 try:
     import mutmut_config
 except ImportError:
     mutmut_config = None
 
 
-class RelativeMutationID(object):
-    def __init__(self, line, index, line_number, filename=None):
-        self.line = line
-        self.index = index
-        self.line_number = line_number
-        self.filename = filename
-
-    def __repr__(self):
-        return 'MutationID(line="{}", index={}, line_number={}, filename={})'.format(self.line, self.index, self.line_number, self.filename)
-
-    def __eq__(self, other):
-        return (self.line, self.index, self.line_number) == (other.line, other.index, other.line_number)
-
-    def __hash__(self):
-        return hash((self.line, self.index, self.line_number))
+@dataclass(frozen=True)
+class RelativeMutationID:
+    line: str
+    index: int
+    line_number: int
+    filename: Optional[str] = field(default=None, compare=False, hash=False)
 
 
 ALL = RelativeMutationID(filename='%all%', line='%all%', index=-1, line_number=-1)
 
 
 class InvalidASTPatternException(Exception):
     pass
 
 
-class ASTPattern(object):
+class ASTPattern:
     def __init__(self, source, **definitions):
         if definitions is None:
             definitions = {}
         source = source.strip()
 
         self.definitions = definitions
 
@@ -284,20 +279,18 @@
     else:
         return pre + [op] + [Keyword(value=' None', start_pos=post[0].start_pos)]
 
 
 NEWLINE = {'formatting': [], 'indent': '', 'type': 'endl', 'value': ''}
 
 
-def argument_mutation(children, context, **_):
+def argument_mutation(children, context: Context, **_):
     """Mutate the arguments one by one from dict(a=b) to dict(aXXX=b).
 
     This is similar to the mutation of dict literals in the form {'a': b}.
-
-    :type context: Context
     """
     if len(context.stack) >= 3 and context.stack[-3].type in ('power', 'atom_expr'):
         stack_pos_of_power_node = -3
     elif len(context.stack) >= 4 and context.stack[-4].type in ('power', 'atom_expr'):
         stack_pos_of_power_node = -4
     else:
         return
@@ -470,15 +463,15 @@
     'decorator': dict(children=decorator_mutation),
     'annassign': dict(children=expression_mutation),
 }
 
 # TODO: detect regexes and mutate them in nasty ways? Maybe mutate all strings as if they are regexes
 
 
-def should_exclude(context, config):
+def should_exclude(context, config: Optional[Config]):
     if config is None or config.covered_lines_by_filename is None:
         return False
 
     try:
         covered_lines = config.covered_lines_by_filename[context.filename]
     except KeyError:
         if config.coverage_data is not None:
@@ -491,16 +484,24 @@
         return True
     current_line = context.current_line_index + 1
     if current_line not in covered_lines:
         return True
     return False
 
 
-class Context(object):
-    def __init__(self, source=None, mutation_id=ALL, dict_synonyms=None, filename=None, config=None, index=0):
+class Context:
+    def __init__(
+        self,
+        source: Optional[str] = None,
+        mutation_id=ALL,
+        dict_synonyms=None,
+        filename=None,
+        config: Optional[Config] = None,
+        index=0,
+    ):
         self.index = index
         self.remove_newline_at_end = False
         self._source = None
         self._set_source(source)
         self.mutation_id = mutation_id
         self.performed_mutation_ids = []
         assert isinstance(mutation_id, RelativeMutationID)
@@ -558,19 +559,17 @@
         if self.config and node.type not in self.config.mutation_types_to_apply:
             return False
         if self.mutation_id == ALL:
             return True
         return self.mutation_id in (ALL, self.mutation_id_of_current_index)
 
 
-def mutate(context):
+def mutate(context: Context) -> Tuple[str, int]:
     """
-    :type context: Context
     :return: tuple of mutated source code and number of mutations performed
-    :rtype: Tuple[str, int]
     """
     try:
         result = parse(context.source, error_recovery=False)
     except Exception:
         print('Failed to parse {}. Internal error from parso follows.'.format(context.filename))
         print('----------------------------------')
         raise
@@ -586,18 +585,15 @@
             raise RuntimeError(
                 "Mutation context states that a mutation occurred but the "
                 "mutated source remains the same as original")
     context.mutated_source = mutated_source
     return mutated_source, len(context.performed_mutation_ids)
 
 
-def mutate_node(node, context):
-    """
-    :type context: Context
-    """
+def mutate_node(node, context: Context):
     context.stack.append(node)
     try:
         if node.type in ('tfpdef', 'import_from', 'import_name'):
             return
 
         if node.type == 'atom_expr' and node.children and node.children[0].type == 'name' and node.children[0].value == '__import__':
             return
@@ -661,18 +657,15 @@
                 # this is just an optimization to stop early
                 if context.performed_mutation_ids and context.mutation_id != ALL:
                     return
     finally:
         context.stack.pop()
 
 
-def mutate_list_of_nodes(node, context):
-    """
-    :type context: Context
-    """
+def mutate_list_of_nodes(node, context: Context):
     return_annotation_started = False
 
     for child_node in node.children:
         if child_node.type == 'operator' and child_node.value == '->':
             return_annotation_started = True
 
         if return_annotation_started and child_node.type == 'operator' and child_node.value == ':':
@@ -684,42 +677,39 @@
         mutate_node(child_node, context=context)
 
         # this is just an optimization to stop early
         if context.performed_mutation_ids and context.mutation_id != ALL:
             return
 
 
-def list_mutations(context):
-    """
-    :type context: Context
-    """
+def list_mutations(context: Context):
     assert context.mutation_id == ALL
     mutate(context)
     return context.performed_mutation_ids
 
 
-def mutate_file(backup, context):
-    """
-    :type backup: bool
-    :type context: Context
-
-    :return: Tuple[str, str]
-    """
+def mutate_file(backup: bool, context: Context) -> Tuple[str, str]:
     with open(context.filename) as f:
         original = f.read()
     if backup:
         with open(context.filename + '.bak', 'w') as f:
             f.write(original)
     mutated, _ = mutate(context)
     with open(context.filename, 'w') as f:
         f.write(mutated)
     return original, mutated
 
 
-def queue_mutants(*, progress, config, mutants_queue, mutations_by_file):
+def queue_mutants(
+    *,
+    progress: Progress,
+    config: Config,
+    mutants_queue,
+    mutations_by_file: Dict[str, List[RelativeMutationID]],
+):
     from mutmut.cache import get_cached_mutation_statuses
 
     try:
         index = 0
         for filename, mutations in mutations_by_file.items():
             cached_mutation_statuses = get_cached_mutation_statuses(filename, mutations, config.hash_of_tests)
             with open(filename) as f:
@@ -806,15 +796,17 @@
                 # rerun the whole test suite to be sure the mutant can not be killed by other tests
                 config.test_command = config._default_test_command
                 survived = tests_pass(config=config, callback=callback)
         except TimeoutError:
             return BAD_TIMEOUT
 
         time_elapsed = time() - start
-        if not survived and time_elapsed > config.test_time_base + (config.baseline_time_elapsed * config.test_time_multipler):
+        if not survived and time_elapsed > config.test_time_base + (
+            config.baseline_time_elapsed * config.test_time_multiplier
+        ):
             return OK_SUSPICIOUS
 
         if survived:
             return BAD_SURVIVED
         else:
             return OK_KILLED
     except SkipException:
@@ -826,39 +818,39 @@
 
         if config.post_mutation:
             result = subprocess.check_output(config.post_mutation, shell=True).decode().strip()
             if result and not config.swallow_output:
                 callback(result)
 
 
-class Config(object):
-    def __init__(self, swallow_output, test_command, covered_lines_by_filename,
-                 baseline_time_elapsed, test_time_multiplier, test_time_base,
-                 dict_synonyms, total, using_testmon,
-                 tests_dirs, hash_of_tests, pre_mutation, post_mutation,
-                 coverage_data, paths_to_mutate, mutation_types_to_apply, no_progress, ci, rerun_all):
-        self.swallow_output = swallow_output
-        self.test_command = self._default_test_command = test_command
-        self.covered_lines_by_filename = covered_lines_by_filename
-        self.baseline_time_elapsed = baseline_time_elapsed
-        self.test_time_multipler = test_time_multiplier
-        self.test_time_base = test_time_base
-        self.dict_synonyms = dict_synonyms
-        self.total = total
-        self.using_testmon = using_testmon
-        self.tests_dirs = tests_dirs
-        self.hash_of_tests = hash_of_tests
-        self.post_mutation = post_mutation
-        self.pre_mutation = pre_mutation
-        self.coverage_data = coverage_data
-        self.paths_to_mutate = paths_to_mutate
-        self.mutation_types_to_apply = mutation_types_to_apply
-        self.no_progress = no_progress
-        self.ci = ci
-        self.rerun_all = rerun_all
+@dataclass
+class Config:
+    swallow_output: bool
+    test_command: str
+    _default_test_command: str = field(init=False)
+    covered_lines_by_filename: Optional[Dict[str, set[Optional[int]]]]
+    baseline_time_elapsed: float
+    test_time_multiplier: float
+    test_time_base: float
+    dict_synonyms: List[str]
+    total: int
+    using_testmon: bool
+    tests_dirs: List[str]
+    hash_of_tests: str
+    post_mutation: str
+    pre_mutation: str
+    coverage_data: Dict[str, Dict[int, List[str]]]
+    paths_to_mutate: List[str]
+    mutation_types_to_apply: Set[str]
+    no_progress: bool
+    ci: bool
+    rerun_all: bool
+
+    def __post_init__(self):
+        self._default_test_command = self.test_command
 
 
 def tests_pass(config: Config, callback) -> bool:
     """
     :return: :obj:`True` if the tests pass, otherwise :obj:`False`
     """
     if config.using_testmon:
@@ -919,19 +911,17 @@
         output = '\r' + s + (' ' * max(last_len[0] - len_s, 0))
         sys.stdout.write(output)
         sys.stdout.flush()
         last_len[0] = len_s
     return p
 
 
-def guess_paths_to_mutate():
-    """Guess the path to source code to mutate
 
-    :rtype: str
-    """
+def guess_paths_to_mutate() -> str:
+    """Guess the path to source code to mutate"""
     this_dir = os.getcwd().split(os.sep)[-1]
     if isdir('lib'):
         return 'lib'
     elif isdir('src'):
         return 'src'
     elif isdir(this_dir):
         return this_dir
@@ -946,15 +936,15 @@
     raise FileNotFoundError(
         'Could not figure out where the code to mutate is. '
         'Please specify it on the command line using --paths-to-mutate, '
         'or by adding "paths_to_mutate=code_dir" in pyproject.toml or setup.cfg to the [mutmut] '
         'section.')
 
 
-class Progress(object):
+class Progress:
     def __init__(self, total, output_legend, no_progress=False):
         self.total = total
         self.output_legend = output_legend
         self.progress = 0
         self.skipped = 0
         self.killed_mutants = 0
         self.surviving_mutants = 0
@@ -1005,32 +995,26 @@
 
 def get_mutations_by_file_from_cache(mutation_pk):
     from mutmut.cache import filename_and_mutation_id_from_pk
     filename, mutation_id = filename_and_mutation_id_from_pk(int(mutation_pk))
     return {filename: [mutation_id]}
 
 
-def popen_streaming_output(cmd, callback, timeout=None):
+def popen_streaming_output(
+    cmd: str, callback: Callable[[str], None], timeout: Optional[float] = None
+) -> int:
     """Open a subprocess and stream its output without hard-blocking.
 
     :param cmd: the command to execute within the subprocess
-    :type cmd: str
-
     :param callback: function that intakes the subprocess' stdout line by line.
         It is called for each line received from the subprocess' stdout stream.
-    :type callback: Callable[[Context], bool]
-
     :param timeout: the timeout time of the subprocess
-    :type timeout: float
-
     :raises TimeoutError: if the subprocess' execution time exceeds
         the timeout time
-
     :return: the return code of the executed subprocess
-    :rtype: int
     """
     if os.name == 'nt':  # pragma: no cover
         process = subprocess.Popen(
             cmd,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             shell=True,
@@ -1084,15 +1068,15 @@
 
     # we have returned from the subprocess cancel the timer if it is running
     timer.cancel()
 
     return process.returncode
 
 
-def hammett_tests_pass(config, callback):
+def hammett_tests_pass(config: Config, callback) -> bool:
     # noinspection PyUnresolvedReferences
     from hammett import main_cli
     modules_before = set(sys.modules.keys())
 
     # set up timeout
     import _thread
     from threading import (
@@ -1139,20 +1123,20 @@
         if any(module_name.startswith(x) for x in modules_to_force_unload) or module_name.startswith('tests') or module_name.startswith('django'):
             del sys.modules[module_name]
 
     return returncode == 0
 
 CYCLE_PROCESS_AFTER = 100
 
-def run_mutation_tests(config, progress, mutations_by_file):
-    """
-    :type config: Config
-    :type progress: Progress
-    :type mutations_by_file: dict[str, list[RelativeMutationID]]
-    """
+
+def run_mutation_tests(
+    config: Config,
+    progress: Progress,
+    mutations_by_file: Dict[str, List[RelativeMutationID]],
+):
     from mutmut.cache import update_mutant_status
 
     # Need to explicitly use the spawn method for python < 3.8 on macOS
     mp_ctx = multiprocessing.get_context('spawn')
 
     mutants_queue = mp_ctx.Queue(maxsize=100)
     add_to_active_queues(mutants_queue)
@@ -1207,84 +1191,84 @@
             assert command == 'status'
 
             progress.register(status)
 
             update_mutant_status(file_to_mutate=filename, mutation_id=mutation_id, status=status, tests_hash=config.hash_of_tests)
 
 
-def read_coverage_data():
+def read_coverage_data() -> Dict[str, Dict[int, List[str]]]:
     """
     Reads the coverage database and returns a dictionary which maps the filenames to the covered lines and their contexts.
-    :rtype: dict[str, dict[int, list[str]]]
     """
     try:
         # noinspection PyPackageRequirements,PyUnresolvedReferences
         from coverage import Coverage
     except ImportError as e:
         raise ImportError('The --use-coverage feature requires the coverage library. Run "pip install --force-reinstall mutmut[coverage]"') from e
     cov = Coverage('.coverage')
     cov.load()
     data = cov.get_data()
     return {filepath: data.contexts_by_lineno(filepath) for filepath in data.measured_files()}
 
 
-def read_patch_data(patch_file_path):
+def read_patch_data(patch_file_path: str):
     try:
         # noinspection PyPackageRequirements
         import whatthepatch
     except ImportError as e:
         raise ImportError('The --use-patch feature requires the whatthepatch library. Run "pip install --force-reinstall mutmut[patch]"') from e
     with open(patch_file_path) as f:
         diffs = whatthepatch.parse_patch(f.read())
 
     return {
         diff.header.new_path: {change.new for change in diff.changes if change.old is None}
         for diff in diffs if diff.changes
     }
 
 
-def add_mutations_by_file(mutations_by_file, filename, dict_synonyms, config):
-    """
-    :type mutations_by_file: dict[str, list[RelativeMutationID]]
-    :type filename: str
-    :type dict_synonyms: list[str]
-    """
+def add_mutations_by_file(
+    mutations_by_file: Dict[str, List[RelativeMutationID]],
+    filename: str,
+    dict_synonyms: List[str],
+    config: Optional[Config],
+):
     with open(filename) as f:
         source = f.read()
     context = Context(
         source=source,
         filename=filename,
         config=config,
         dict_synonyms=dict_synonyms,
     )
 
     try:
         mutations_by_file[filename] = list_mutations(context)
         from mutmut.cache import register_mutants
+
         register_mutants(mutations_by_file)
     except Exception as e:
-        raise RuntimeError('Failed while creating mutations for {}, for line "{}"'.format(context.filename, context.current_source_line)) from e
+        raise RuntimeError(
+            'Failed while creating mutations for {}, for line "{}"'.format(
+                context.filename, context.current_source_line
+            )
+        ) from e
 
 
-def python_source_files(path, tests_dirs, paths_to_exclude=None):
+def python_source_files(
+    path: str, tests_dirs: List[str], paths_to_exclude: Optional[List[str]] = None
+) -> Iterator[str]:
     """Attempt to guess where the python source files to mutate are and yield
     their paths
 
     :param path: path to a python source file or package directory
-    :type path: str
-
     :param tests_dirs: list of directory paths containing test files
         (we do not want to mutate these!)
-    :type tests_dirs: list[str]
-
     :param paths_to_exclude: list of UNIX filename patterns to exclude
-    :type paths_to_exclude: list[str]
 
     :return: generator listing the paths to the python source files to mutate
-    :rtype: Generator[str, None, None]
     """
     paths_to_exclude = paths_to_exclude or []
     if isdir(path):
         for root, dirs, files in os.walk(path, topdown=True):
             for exclude_pattern in paths_to_exclude:
                 dirs[:] = [d for d in dirs if not fnmatch.fnmatch(d, exclude_pattern)]
                 files[:] = [f for f in files if not fnmatch.fnmatch(f, exclude_pattern)]
@@ -1293,39 +1277,37 @@
             for filename in files:
                 if filename.endswith('.py'):
                     yield os.path.join(root, filename)
     else:
         yield path
 
 
-def compute_exit_code(progress, exception=None, ci=False):
+def compute_exit_code(
+    progress: Progress, exception: Optional[Exception] = None, ci: bool = False
+) -> int:
     """Compute an exit code for mutmut mutation testing
 
-    The following exit codes are available for mutmut:
+    The following exit codes are available for mutmut (as documented for the CLI run command):
      * 0 if all mutants were killed (OK_KILLED)
      * 1 if a fatal error occurred
      * 2 if one or more mutants survived (BAD_SURVIVED)
      * 4 if one or more mutants timed out (BAD_TIMEOUT)
      * 8 if one or more mutants caused tests to take twice as long (OK_SUSPICIOUS)
 
      Exit codes 1 to 8 will be bit-ORed so that it is possible to know what
      different mutant statuses occurred during mutation testing.
 
      When running with ci=True (--CI flag enabled), the exit code will always be
      1 for a fatal error or 0 for any other case.
 
     :param exception:
-    :type exception: Exception
     :param progress:
-    :type progress: Progress
     :param ci:
-    :type ci: bool
 
     :return: integer noting the exit code of the mutation tests.
-    :rtype: int
     """
     code = 0
     if exception is not None:
         code = code | 1
     if ci:
         return code
     if progress.surviving_mutants > 0:
```

### Comparing `mutmut-2.4.4/mutmut/__main__.py` & `mutmut-2.4.5/mutmut/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from io import (
     open,
 )
 from os.path import exists
 from pathlib import Path
 from shutil import copy
 from time import time
+from typing import List
 
 import click
 from glob2 import glob
 
 from mutmut import (
     mutate_file,
     MUTANT_STATUSES,
@@ -43,26 +44,21 @@
 )
 from mutmut.cache import print_result_cache, print_result_ids_cache, \
     hash_of_tests, \
     filename_and_mutation_id_from_pk, cached_test_time, set_cached_test_time, \
     update_line_numbers, print_result_cache_junitxml, get_unified_diff
 
 
-def do_apply(mutation_pk, dict_synonyms, backup):
+def do_apply(mutation_pk: str, dict_synonyms: List[str], backup: bool):
     """Apply a specified mutant to the source code
 
     :param mutation_pk: mutmut cache primary key of the mutant to apply
-    :type mutation_pk: str
-
     :param dict_synonyms: list of synonym keywords for a python dictionary
-    :type dict_synonyms: list[str]
-
     :param backup: if :obj:`True` create a backup of the source file
         before applying the mutation
-    :type backup: bool
     """
     filename, mutation_id = filename_and_mutation_id_from_pk(int(mutation_pk))
 
     update_line_numbers(filename)
 
     context = Context(
         mutation_id=mutation_id,
@@ -80,14 +76,24 @@
 DEFAULT_RUNNER = 'python -m pytest -x --assert=plain'
 
 
 @click.group(context_settings=dict(help_option_names=['-h', '--help']))
 def climain():
     """
     Mutation testing system for Python.
+
+    Getting started:
+
+    To run with pytest in test or tests folder: mutmut run
+
+    For more options: mutmut run --help
+
+    To show the results: mutmut results
+
+    To generate HTML report: mutmut html
     """
     pass
 
 
 @climain.command()
 def version():
     """Show the version and exit."""
@@ -128,14 +134,37 @@
 )
 def run(argument, paths_to_mutate, disable_mutation_types, enable_mutation_types, runner,
         tests_dir, test_time_multiplier, test_time_base, swallow_output, use_coverage,
         dict_synonyms, pre_mutation, post_mutation, use_patch_file, paths_to_exclude,
         simple_output, no_progress, ci, rerun_all):
     """
     Runs mutmut. You probably want to start with just trying this. If you supply a mutation ID mutmut will check just this mutant.
+
+    Runs pytest by default (or unittest if pytest is unavailable) on tests in the “tests” or “test” folder.
+
+    It is recommended to configure any non-default options needed in setup.cfg or pyproject.toml, as described in the documentation.
+
+    Exit codes:
+
+     * 0 - all mutants were killed
+
+    Otherwise any or sum of any of the following exit codes:
+
+     * 1 - if a fatal error occurred
+
+     * 2 - if one or more mutants survived
+
+     * 4 - if one or more mutants timed out
+
+     * 8 - if one or more mutants caused tests to take twice as long
+
+    (This is equivalent to a bit-OR combination of the exit codes that may apply.)
+
+    With --CI flag enabled, the exit code will always be
+    1 for a fatal error or 0 for any other case.
     """
     if test_time_base is None:  # click sets the default=0.0 to None
         test_time_base = 0.0
     if test_time_multiplier is None:  # click sets the default=0.0 to None
         test_time_multiplier = 0.0
 
     sys.exit(do_run(argument, paths_to_mutate, disable_mutation_types, enable_mutation_types, runner,
@@ -232,22 +261,38 @@
     """
     Generate a HTML report of surviving mutants.
     """
     create_html_report(dict_synonyms)
     sys.exit(0)
 
 
-def do_run(argument, paths_to_mutate, disable_mutation_types,
-           enable_mutation_types, runner, tests_dir, test_time_multiplier, test_time_base,
-           swallow_output, use_coverage, dict_synonyms, pre_mutation, post_mutation,
-           use_patch_file, paths_to_exclude, simple_output, no_progress, ci, rerun_all):
+def do_run(
+    argument,
+    paths_to_mutate,
+    disable_mutation_types,
+    enable_mutation_types,
+    runner,
+    tests_dir,
+    test_time_multiplier,
+    test_time_base,
+    swallow_output,
+    use_coverage,
+    dict_synonyms,
+    pre_mutation,
+    post_mutation,
+    use_patch_file,
+    paths_to_exclude,
+    simple_output,
+    no_progress,
+    ci,
+    rerun_all,
+) -> int:
     """return exit code, after performing an mutation test run.
 
-    :return: the exit code from executing the mutation tests
-    :rtype: int
+    :return: the exit code from executing the mutation tests for run command
     """
     if use_coverage and use_patch_file:
         raise click.BadArgumentUsage("You can't combine --use-coverage and --use-patch")
 
     if disable_mutation_types and enable_mutation_types:
         raise click.BadArgumentUsage("You can't combine --disable-mutation-types and --enable-mutation-types")
     if enable_mutation_types:
@@ -287,15 +332,20 @@
             '--paths-to-mutate',
             'You must specify a list of paths to mutate.'
             'Either as a command line argument, or by setting paths_to_mutate under the section [mutmut] in setup.cfg.'
             'To specify multiple paths, separate them with commas or colons (i.e: --paths-to-mutate=path1/,path2/path3/,path4/).'
         )
 
     tests_dirs = []
-    for p in split_paths(tests_dir):
+    test_paths = split_paths(tests_dir)
+    if test_paths is None:
+        raise FileNotFoundError(
+            'No test folders found in current folder. Run this where there is a "tests" or "test" folder.'
+        )
+    for p in test_paths:
         tests_dirs.extend(glob(p, recursive=True))
 
     for p in paths_to_mutate:
         for pt in split_paths(tests_dir):
             tests_dirs.extend(glob(p + '/**/' + pt, recursive=True))
     del tests_dir
     current_hash_of_tests = hash_of_tests(tests_dirs)
@@ -334,24 +384,24 @@
 """.format(**output_legend))
     if runner is DEFAULT_RUNNER:
         try:
             import pytest  # noqa
         except ImportError:
             runner = 'python -m unittest'
 
+    if hasattr(mutmut_config, 'init'):
+        mutmut_config.init()
+        
     baseline_time_elapsed = time_test_suite(
         swallow_output=not swallow_output,
         test_command=runner,
         using_testmon=using_testmon,
         current_hash_of_tests=current_hash_of_tests,
         no_progress=no_progress,
-    )
-
-    if hasattr(mutmut_config, 'init'):
-        mutmut_config.init()
+    )    
 
     if using_testmon:
         copy('.testmondata', '.testmondata-initial')
 
     # if we're running in a mode with externally whitelisted lines
     covered_lines_by_filename = None
     coverage_data = None
@@ -434,30 +484,30 @@
             return
 
         filename, mutation_id = filename_and_mutation_id_from_pk(int(argument))
         update_line_numbers(filename)
         mutations_by_file[filename] = [mutation_id]
 
 
-def time_test_suite(swallow_output, test_command, using_testmon, current_hash_of_tests, no_progress):
+def time_test_suite(
+    swallow_output: bool,
+    test_command: str,
+    using_testmon: bool,
+    current_hash_of_tests,
+    no_progress,
+) -> float:
     """Execute a test suite specified by ``test_command`` and record
     the time it took to execute the test suite as a floating point number
 
     :param swallow_output: if :obj:`True` test stdout will be not be printed
-    :type swallow_output: bool
-
     :param test_command: command to spawn the testing subprocess
-    :type test_command: str
-
     :param using_testmon: if :obj:`True` the test return code evaluation will
         accommodate for ``pytest-testmon``
-    :type using_testmon: bool
 
     :return: execution time of the test suite
-    :rtype: float
     """
     cached_time = cached_test_time()
     if cached_time is not None and current_hash_of_tests == cached_hash_of_tests():
         print('1. Using cached time for baseline tests, to run baseline again delete the cache file')
         return cached_time
 
     print('1. Running tests without mutations')
```

### Comparing `mutmut-2.4.4/mutmut/cache.py` & `mutmut-2.4.5/mutmut/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from functools import wraps
 from io import open
 from itertools import groupby, zip_longest
 from os.path import join, dirname
 from typing import Tuple
 
 
-from junit_xml import TestSuite, TestCase
+from junit_xml import TestSuite, TestCase, to_xml_report_string
 from pony.orm import Database, Required, db_session, Set, Optional, select, \
     PrimaryKey, RowNotFound, ERDiagramError, OperationalError
 
-from mutmut import MUTANT_STATUSES, BAD_TIMEOUT, OK_SUSPICIOUS, BAD_SURVIVED, UNTESTED, \
+from mutmut import MUTANT_STATUSES, BAD_TIMEOUT, OK_SUSPICIOUS, BAD_SURVIVED, SKIPPED, UNTESTED, \
     OK_KILLED, RelativeMutationID, Context, mutate
 
 db = Database()
 
 current_db_version = 4
 
 
@@ -179,15 +179,15 @@
                         print(get_unified_diff(x.id, dict_synonyms, update_cache=False, source=source))
                 else:
                     print(ranges([x.id for x in mutants]))
 
     print_stuff('Timed out ⏰', select(x for x in Mutant if x.status == BAD_TIMEOUT))
     print_stuff('Suspicious 🤔', select(x for x in Mutant if x.status == OK_SUSPICIOUS))
     print_stuff('Survived 🙁', select(x for x in Mutant if x.status == BAD_SURVIVED))
-    print_stuff('Untested/skipped', select(x for x in Mutant if x.status == UNTESTED))
+    print_stuff('Untested/skipped', select(x for x in Mutant if x.status == UNTESTED or x.status == SKIPPED))
 
 
 @init_db
 @db_session
 def print_result_ids_cache(desired_status):
     status = MUTANT_STATUSES[desired_status]
     mutant_query = select(x for x in Mutant if x.status == status)
@@ -251,30 +251,30 @@
                 if untested_policy != 'ignore':
                     func = getattr(tc, 'add_{}_info'.format(untested_policy))
                     func(message=mutant.status, output=get_unified_diff(mutant.id, dict_synonyms))
 
             test_cases.append(tc)
 
     ts = TestSuite("mutmut", test_cases)
-    return TestSuite.to_xml_string([ts])
+    return to_xml_report_string([ts])
 
 
 @init_db
 @db_session
 def create_html_report(dict_synonyms):
-    mutants = list(select(x for x in Mutant))
+    mutants = sorted(list(select(x for x in Mutant)), key=lambda x: x.line.sourcefile.filename)
 
     os.makedirs('html', exist_ok=True)
 
     with open('html/index.html', 'w') as index_file:
         index_file.write('<h1>Mutation testing report</h1>')
 
         index_file.write('Killed %s out of %s mutants' % (len([x for x in mutants if x.status == OK_KILLED]), len(mutants)))
 
-        index_file.write('<table><thead><tr><th>File</th><th>Total</th><th>Killed</th><th>% killed</th><th>Survived</th></thead>')
+        index_file.write('<table><thead><tr><th>File</th><th>Total</th><th>Skipped</th><th>Killed</th><th>% killed</th><th>Survived</th></thead>')
 
         for filename, mutants in groupby(mutants, key=lambda x: x.line.sourcefile.filename):
             report_filename = join('html', filename)
 
             mutants = list(mutants)
 
             with open(filename) as f:
@@ -289,18 +289,19 @@
                 f.write('<html><body>')
 
                 f.write('<h1>%s</h1>' % filename)
 
                 killed = len(mutants_by_status[OK_KILLED])
                 f.write('Killed %s out of %s mutants' % (killed, len(mutants)))
 
-                index_file.write('<tr><td><a href="%s.html">%s</a></td><td>%s</td><td>%s</td><td>%.2f</td><td>%s</td>' % (
+                index_file.write('<tr><td><a href="%s.html">%s</a></td><td>%s</td><td>%s</td><td>%s</td><td>%.2f</td><td>%s</td>' % (
                     filename,
                     filename,
                     len(mutants),
+                    len(mutants_by_status[SKIPPED]),
                     killed,
                     (killed / len(mutants) * 100),
                     len(mutants_by_status[BAD_SURVIVED]),
                 ))
 
                 def print_diffs(status):
                     mutants = mutants_by_status[status]
@@ -320,14 +321,19 @@
                     print_diffs(BAD_SURVIVED)
 
                 if mutants_by_status[OK_SUSPICIOUS]:
                     f.write('<h2>Suspicious</h2>')
                     f.write('Mutants that made the test suite take longer, but otherwise seemed ok')
                     print_diffs(OK_SUSPICIOUS)
 
+                if mutants_by_status[SKIPPED]:
+                    f.write('<h2>Skipped</h2>')
+                    f.write('Mutants that were skipped')
+                    print_diffs(SKIPPED)
+
                 f.write('</body></html>')
 
         index_file.write('</table></body></html>')
 
 
 def get_or_create(model, defaults=None, **params):
     if defaults is None:
```

### Comparing `mutmut-2.4.4/mutmut.egg-info/PKG-INFO` & `mutmut-2.4.5/mutmut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutmut
-Version: 2.4.4
+Version: 2.4.5
 Summary: mutation testing for Python 3
 Home-page: https://github.com/boxed/mutmut
 Author: Anders Hovmöller
 Author-email: boxed@killingar.net
 License: BSD
 Description: mutmut - python mutation tester
         ===============================
@@ -52,34 +52,50 @@
         .. code-block:: console
         
             pip install mutmut
             mutmut run
         
         This will by default run pytest (or unittest if pytest is unavailable)
         on tests in the "tests" or "test" folder and
-        it will try to figure out where the code to mutate lies. Run
+        it will try to figure out where the code to mutate lies.
+        
+        NOTE that mutmut will apply the mutations directly, one at a time;
+        it is **highly** recommended to add all changes to source control
+        before running.
+        
+        Enter
         
         .. code-block:: console
         
-            mutmut --help
+            mutmut run --help
         
         for the available flags, to use other runners, etc. The recommended way to use
-        mutmut if the defaults aren't working for you is to add a block in ``setup.cfg``.
+        mutmut if the defaults aren't working for you is to add a
+        block in ``setup.cfg`` or ``project.toml``.
         Then when you come back to mutmut weeks later you don't have to figure out the
-        flags again, just run ``mutmut run`` and it works. Like this:
+        flags again, just run ``mutmut run`` and it works.
+        Like this in ``setup.cfg``:
         
         .. code-block:: ini
         
             [mutmut]
             paths_to_mutate=src/
             backup=False
             runner=python -m hammett -x
             tests_dir=tests/
             dict_synonyms=Struct, NamedStruct
         
+        or like this in ``pyproject.toml``:
+        
+        .. code-block:: ini
+        
+            [tool.mutmut]
+            paths_to_mutate="src"
+            runner="python -m hammett -x"
+        
         To use multiple paths either in the ``paths_to_mutate`` or ``tests_dir`` option
         use a comma or colon separated list. For example:
         
         .. code-block:: ini
         
             [mutmut]
             paths_to_mutate=src/,src2/
@@ -90,19 +106,19 @@
         test suite changes.
         
         To print the results run ``mutmut show``. It will give you a list of the mutants
         grouped by file. You can now look at a specific mutant diff with ``mutmut show 3``,
         all mutants for a specific file with ``mutmut show path/to/file.py`` or all mutants
         with ``mutmut show all``.
         
-        
         You can also write a mutant to disk with ``mutmut apply 3``. You should **REALLY**
         have the file you mutate under source code control and committed before you apply
         a mutant!
         
+        To generate a HTML report for a web browser: ``mutmut html``
         
         Whitelisting
         ------------
         
         You can mark lines like this:
         
         .. code-block:: python
```

### Comparing `mutmut-2.4.4/setup.py` & `mutmut-2.4.5/setup.py`

 * *Files identical despite different names*

