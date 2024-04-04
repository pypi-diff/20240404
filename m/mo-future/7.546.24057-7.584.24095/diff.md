# Comparing `tmp/mo-future-7.546.24057.tar.gz` & `tmp/mo-future-7.584.24095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-future-7.546.24057.tar", last modified: Mon Feb 26 03:47:15 2024, max compression
+gzip compressed data, was "mo-future-7.584.24095.tar", last modified: Thu Apr  4 12:22:38 2024, max compression
```

## Comparing `mo-future-7.546.24057.tar` & `mo-future-7.584.24095.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 03:47:15.976160 mo-future-7.546.24057/
--rw-rw-rw-   0        0        0    16725 2019-09-12 20:45:20.000000 mo-future-7.546.24057/LICENSE
--rw-rw-rw-   0        0        0     2018 2024-02-26 03:47:15.976160 mo-future-7.546.24057/PKG-INFO
--rw-rw-rw-   0        0        0     1109 2022-12-15 04:31:32.000000 mo-future-7.546.24057/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 03:47:15.969554 mo-future-7.546.24057/mo_future/
--rw-rw-rw-   0        0        0     5042 2024-02-26 03:47:07.000000 mo-future-7.546.24057/mo_future/__init__.py
--rw-rw-rw-   0        0        0     4242 2023-05-24 02:37:00.000000 mo-future-7.546.24057/mo_future/cache.py
-drwxrwxrwx   0        0        0        0 2024-02-26 03:47:15.976160 mo-future-7.546.24057/mo_future.egg-info/
--rw-rw-rw-   0        0        0     2018 2024-02-26 03:47:15.000000 mo-future-7.546.24057/mo_future.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-02-26 03:47:15.000000 mo-future-7.546.24057/mo_future.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 03:47:15.000000 mo-future-7.546.24057/mo_future.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-02-26 03:47:15.000000 mo-future-7.546.24057/mo_future.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 03:47:15.976160 mo-future-7.546.24057/setup.cfg
--rw-rw-rw-   0        0        0     2070 2024-02-26 03:47:10.000000 mo-future-7.546.24057/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 03:47:15.976160 mo-future-7.546.24057/tests/
--rw-rw-rw-   0        0        0      189 2023-01-06 02:52:44.000000 mo-future-7.546.24057/tests/test_basic.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:22:38.099506 mo-future-7.584.24095/
+-rw-rw-rw-   0        0        0    16725 2019-09-12 20:45:20.000000 mo-future-7.584.24095/LICENSE
+-rw-rw-rw-   0        0        0     2018 2024-04-04 12:22:38.098462 mo-future-7.584.24095/PKG-INFO
+-rw-rw-rw-   0        0        0     1109 2022-12-15 04:31:32.000000 mo-future-7.584.24095/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:22:38.092220 mo-future-7.584.24095/mo_future/
+-rw-rw-rw-   0        0        0     5067 2024-04-04 12:22:30.000000 mo-future-7.584.24095/mo_future/__init__.py
+-rw-rw-rw-   0        0        0     4242 2023-05-24 02:37:00.000000 mo-future-7.584.24095/mo_future/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:22:38.098462 mo-future-7.584.24095/mo_future.egg-info/
+-rw-rw-rw-   0        0        0     2018 2024-04-04 12:22:38.000000 mo-future-7.584.24095/mo_future.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-04-04 12:22:38.000000 mo-future-7.584.24095/mo_future.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:22:38.000000 mo-future-7.584.24095/mo_future.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 12:22:38.000000 mo-future-7.584.24095/mo_future.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:22:38.099506 mo-future-7.584.24095/setup.cfg
+-rw-rw-rw-   0        0        0     2070 2024-04-04 12:22:33.000000 mo-future-7.584.24095/setup.py
```

### Comparing `mo-future-7.546.24057/LICENSE` & `mo-future-7.584.24095/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-future-7.546.24057/PKG-INFO` & `mo-future-7.584.24095/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-future
-Version: 7.546.24057
+Version: 7.584.24095
 Summary: More future! Make Python 2/3 compatibility a bit easier
 Home-page: https://github.com/klahnakoski/mo-future
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-future-7.546.24057/README.md` & `mo-future-7.584.24095/README.md`

 * *Files identical despite different names*

### Comparing `mo-future-7.546.24057/mo_future/__init__.py` & `mo-future-7.584.24095/mo_future/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "decorate",
     "extend",
     "first",
     "flatten",
     "function_type",
     "generator_types",
     "get_function_arguments",
+    "get_function_name",
     "get_ident",
     "HTMLParser",
     "input",
     "integer_types",
     "interrupt_main",
     "is_binary",
     "is_text",
```

### Comparing `mo-future-7.546.24057/mo_future/cache.py` & `mo-future-7.584.24095/mo_future/cache.py`

 * *Files identical despite different names*

### Comparing `mo-future-7.546.24057/mo_future.egg-info/PKG-INFO` & `mo-future-7.584.24095/mo_future.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-future
-Version: 7.546.24057
+Version: 7.584.24095
 Summary: More future! Make Python 2/3 compatibility a bit easier
 Home-page: https://github.com/klahnakoski/mo-future
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-future-7.546.24057/setup.py` & `mo-future-7.584.24095/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     description='More future! Make Python 2/3 compatibility a bit easier',
     license='MPL 2.0',
     long_description='# More Future!\n\nFor old code written against Python2, plus some tiny useful functions\n\n## Recent Changes\n\n**December 2022** - No longer points to Python2 modules. \n\n\n## Description\n\n### Problem \n\n`future` or `six` are hard to use: It is easy to google how to import an object in Python2, or Python3, but finding the full path to the same in these compatibility libraries is difficult. \n\n## Solution\n\nAll the modules and types required for compatibility are put into the `mo-future` top-level module so they are  easy to find.\n\n\n### Flat namespace\n\nInstead of \n\n```python\n    from future.utils import text\n```\n\nyou get the same, but without having to discover what sub-module the `text` is hiding:  \n\n```python\n    from mo_future import text\n```\n\n\n### Simpler imports\n\nInstead of writing conditional imports like \n\n```python\n    try:\n        from io import StringIO\n    except:\n        from StringIO import StringIO\n```\n\nor \n\n```python\n    if PY3:\n        from io import StringIO\n    else:\n        from StringIO import StringIO\n```\n\nyou can use `mo-future`:\n\n```python\n    from mo_future import StringIO\n```\n\n\n',
     long_description_content_type='text/markdown',
     name='mo-future',
     packages=["mo_future"],
     url='https://github.com/klahnakoski/mo-future',
-    version='7.546.24057'
+    version='7.584.24095'
 )
```

