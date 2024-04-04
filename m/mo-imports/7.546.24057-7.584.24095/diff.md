# Comparing `tmp/mo-imports-7.546.24057.tar.gz` & `tmp/mo-imports-7.584.24095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-imports-7.546.24057.tar", last modified: Mon Feb 26 03:48:28 2024, max compression
+gzip compressed data, was "mo-imports-7.584.24095.tar", last modified: Thu Apr  4 12:23:45 2024, max compression
```

## Comparing `mo-imports-7.546.24057.tar` & `mo-imports-7.584.24095.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 03:48:28.968541 mo-imports-7.546.24057/
--rw-rw-rw-   0        0        0    16725 2020-07-23 15:46:04.000000 mo-imports-7.546.24057/LICENSE
--rw-rw-rw-   0        0        0     6089 2024-02-26 03:48:28.968541 mo-imports-7.546.24057/PKG-INFO
--rw-rw-rw-   0        0        0     5012 2024-01-21 18:07:36.000000 mo-imports-7.546.24057/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 03:48:28.956540 mo-imports-7.546.24057/mo_imports/
--rw-rw-rw-   0        0        0     9823 2024-02-04 18:26:23.000000 mo-imports-7.546.24057/mo_imports/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-26 03:48:28.968541 mo-imports-7.546.24057/mo_imports.egg-info/
--rw-rw-rw-   0        0        0     6089 2024-02-26 03:48:28.000000 mo-imports-7.546.24057/mo_imports.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-02-26 03:48:28.000000 mo-imports-7.546.24057/mo_imports.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 03:48:28.000000 mo-imports-7.546.24057/mo_imports.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-02-26 03:48:28.000000 mo-imports-7.546.24057/mo_imports.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-26 03:48:28.000000 mo-imports-7.546.24057/mo_imports.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 03:48:28.968541 mo-imports-7.546.24057/setup.cfg
--rw-rw-rw-   0        0        0     6151 2024-02-26 03:48:22.000000 mo-imports-7.546.24057/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 03:48:28.964539 mo-imports-7.546.24057/tests/
--rw-rw-rw-   0        0        0      608 2023-09-22 00:42:25.000000 mo-imports-7.546.24057/tests/test_basic.py
--rw-rw-rw-   0        0        0      585 2024-01-21 17:30:52.000000 mo-imports-7.546.24057/tests/test_delay_import.py
--rw-rw-rw-   0        0        0     2100 2023-06-10 00:41:10.000000 mo-imports-7.546.24057/tests/test_export.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:23:45.581318 mo-imports-7.584.24095/
+-rw-rw-rw-   0        0        0    16725 2020-07-23 15:46:04.000000 mo-imports-7.584.24095/LICENSE
+-rw-rw-rw-   0        0        0     6089 2024-04-04 12:23:45.580215 mo-imports-7.584.24095/PKG-INFO
+-rw-rw-rw-   0        0        0     5058 2024-04-04 12:23:38.000000 mo-imports-7.584.24095/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:23:45.571935 mo-imports-7.584.24095/mo_imports/
+-rw-rw-rw-   0        0        0     9823 2024-02-04 18:26:23.000000 mo-imports-7.584.24095/mo_imports/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:23:45.579168 mo-imports-7.584.24095/mo_imports.egg-info/
+-rw-rw-rw-   0        0        0     6089 2024-04-04 12:23:45.000000 mo-imports-7.584.24095/mo_imports.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-04 12:23:45.000000 mo-imports-7.584.24095/mo_imports.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:23:45.000000 mo-imports-7.584.24095/mo_imports.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-04 12:23:45.000000 mo-imports-7.584.24095/mo_imports.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 12:23:45.000000 mo-imports-7.584.24095/mo_imports.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:23:45.581318 mo-imports-7.584.24095/setup.cfg
+-rw-rw-rw-   0        0        0     6151 2024-04-04 12:23:41.000000 mo-imports-7.584.24095/setup.py
```

### Comparing `mo-imports-7.546.24057/LICENSE` & `mo-imports-7.584.24095/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-imports-7.546.24057/PKG-INFO` & `mo-imports-7.584.24095/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mo-imports
-Version: 7.546.24057
+Version: 7.584.24095
 Summary: More Imports! - Delayed importing
 Home-page: https://github.com/klahnakoski/mo-imports
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-future==7.546.24057
+Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-logs>=8.538.24037; extra == "tests"
+Requires-Dist: mo-logs>=8.543.24046; extra == "tests"
 
 # More Imports! - Delayed importing 
 
 A few methods to make late importing cleaner
 
 
 |Branch      |Status   |
```

### Comparing `mo-imports-7.546.24057/README.md` & `mo-imports-7.584.24095/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # More Imports! - Delayed importing 
 
 A few methods to make late importing cleaner
 
 
 |Branch      |Status   |
 |------------|---------|
-|master      | [![Build Status](https://app.travis-ci.com/klahnakoski/mo-imports.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-imports) |
+|master      |  [![Build Status](https://github.com/klahnakoski/mo-imports/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-imports/actions/workflows/build.yml) |
 |dev         | [![Build Status](https://app.travis-ci.com/klahnakoski/mo-imports.svg?branch=dev)](https://travis-ci.com/github/klahnakoski/mo-imports)    |
 
 
 
 ## Problem
 
 Splitting code into modules is nice, but it can result in cyclic dependencies.
```

### Comparing `mo-imports-7.546.24057/mo_imports/__init__.py` & `mo-imports-7.584.24095/mo_imports/__init__.py`

 * *Files identical despite different names*

### Comparing `mo-imports-7.546.24057/mo_imports.egg-info/PKG-INFO` & `mo-imports-7.584.24095/mo_imports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mo-imports
-Version: 7.546.24057
+Version: 7.584.24095
 Summary: More Imports! - Delayed importing
 Home-page: https://github.com/klahnakoski/mo-imports
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-future==7.546.24057
+Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-logs>=8.538.24037; extra == "tests"
+Requires-Dist: mo-logs>=8.543.24046; extra == "tests"
 
 # More Imports! - Delayed importing 
 
 A few methods to make late importing cleaner
 
 
 |Branch      |Status   |
```

### Comparing `mo-imports-7.546.24057/setup.py` & `mo-imports-7.584.24095/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Imports! - Delayed importing',
-    extras_require={"tests":["mo-logs>=8.538.24037"]},
-    install_requires=["mo-future==7.546.24057"],
+    extras_require={"tests":["mo-logs>=8.543.24046"]},
+    install_requires=["mo-future==7.584.24095"],
     license='MPL 2.0',
     long_description='# More Imports! - Delayed importing \n\nA few methods to make late importing cleaner\n\n\n|Branch      |Status   |\n|------------|---------|\n|master      | [![Build Status](https://app.travis-ci.com/klahnakoski/mo-imports.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-imports) |\n|dev         | [![Build Status](https://app.travis-ci.com/klahnakoski/mo-imports.svg?branch=dev)](https://travis-ci.com/github/klahnakoski/mo-imports)    |\n\n\n\n## Problem\n\nSplitting code into modules is nice, but it can result in cyclic dependencies.  \n\n\n**foos.py**\n\n```python\nfrom bars import bar\n\ndef foo():\n    bar()\n```\n\n**bars.py**\n\n```python\nfrom foos import foo\n\ndef bar():\n    foo()\n```\n\n> We are not concerned with the infinite recursion; this is only for demonstrating cyclic dependencies. \n\n\n## More Imports!\n\n### Solution #1: Use `expect`/`export` pattern\n\nAll your cyclic dependencies are covered with this one pattern: Break cycles by `expect`ing a name in the first module, and let the second module `export` to the first when the value is available\n\n**foos.py**\n\n```python\nfrom mo_imports import expect\n\nbar = expect("bar")\n\ndef foo():\n    bar()\n```\n\n**bars.py**\n\n```python\nfrom mo_imports import export\nfrom foos import foo\n\ndef bar():\n    foo()\n\nexport("bars", bar)\n```\n\n**Benefits**\n  \n \n* every `expect` is verified to match with an `export` (and visa-versa)\n* using an expected variable before `export` raises an error     \n* code is run only once, at module load time, not later\n* methods do not run import code\n* all "imports" are at the top of the file\n\n\n### Solution #2: Use `delay_import`\n\nProvide a proxy which is responsible for import upon first use of the module variable.\n\n**foos.py**\n\n```python\nfrom mo_imports import delay_import\n\nbar = delay_import("bars.bar")\n\ndef foo():\n    bar()\n\n```\n\n**bars.py**\n\n```python\nfrom foos import foo\n\ndef bar():\n    foo()\n```\n\n\n**Benefits**\n  \n* cleaner code \n* costly imports are delayed until first use\n\n\n> WARNING\n> \n> Requires any of `__call__`, `__getitem__`, `__getattr__` to be called to trigger the\n> import.  This means sentinals, placeholders, and default values can NOT be imported \n> using `delay_import()`\n\n\n## Other solutions\n\nIf you do not use `mo-imports` your import cycles can be broken using one of the following common patterns:\n\n\n### Bad Solution: Keep in single file\n\nYou can declare yet-another-module that holds the cycles\n\n**foosbars.py**\n\n```python\n    def foo():\n        bar()\n\n    def bar():\n        foo()\n```\n\nbut this breaks the code modularity\n\n\n### Bad Solution: Use end-of-file imports\n\nDuring import, setup of the first module is paused while it imports a second. A bottom-of-file import will ensure the first module is mostly setup to be used by the second. \n\n**foos.py**\n\n```python\ndef foo():\n    bar()\n\nfrom bars import bar\n```\n\n**bars.py**\n\n```python\ndef bar():\n    foo()\n\nfrom foos import foo\n```\n\nLinters do not like this pattern: You may miss imports, since these are hiding at the bottom.\n    \n\n\n### Bad Solution: Inline import\n\nImport the name only when it is needed\n\n**foos.py**\n\n```python\ndef foo():\n    from bars import bar\n    bar()\n```\n    \n**bars.py**\n\n\n```python\ndef bar():\n    from foos import foo\n    foo()\n```\n\nThis is fine for rarely run code, but there is an undesirable overhead because import is checked everytime the method is run. You may miss imports because they are hiding inline rather than at the top of the file.\n  \n\n\n### Bad Solution: Use the `_late_import()` pattern\n\nWhen other bad solutions do not work work, then importing late is the remaining option\n\n**foos.py**\n\n```python\nfrom bars import bar\n\ndef foo():\n    bar()\n```\n\n**bars.py**\n\n```python\nfoo = None\n\ndef _late_import():\n    global foo\n    from foos import foo\n    _ = foo\n\ndef bar():\n    if not foo:\n        _late_import()\n    foo()\n```\n\nPlaceholders variables are added, which linters complain about type. There is the added `_late_import()` method. You risk it is not run everywhere as needed. This has less overhead than an inline import, but there is still a check.\n \n\n## More on importing\n\nImporting a complex modular library is still hard; the complexity comes from the the order *other modules* declare their imports; you have no control over which of your modules will be imported first.  For example, one module may \n\n```python\nfrom my_lib.bars import bar\nfrom my_lib.foos import foo\n```\n\nanother module may choose the opposite order\n\n```python\nfrom my_lib.foos import foo\nfrom my_lib.bars import bar\n```\n\n### Ordering imports\n\nWith cyclic dependencies, ordering the imports can get tricky.  Here are some rules \n\n* choose your principle modules and the order you want them imported.\n* your remaining modules are assumed to be imported in alphabetical order (as most linters prefer)\n* **use top level `__init__.py` to control the order of imports**\n* encourage third party modules to use this top level module.  for example\n  ```python\n  from my_lib import foo, bar\n  ```\n* finally, use `mo_imports` to break cycles\n',
     long_description_content_type='text/markdown',
     name='mo-imports',
     packages=["mo_imports"],
     url='https://github.com/klahnakoski/mo-imports',
-    version='7.546.24057'
+    version='7.584.24095'
 )
```
