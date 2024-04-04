# Comparing `tmp/mo-dots-9.582.24095.tar.gz` & `tmp/mo-dots-9.584.24095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-dots-9.582.24095.tar", last modified: Thu Apr  4 03:46:54 2024, max compression
+gzip compressed data, was "mo-dots-9.584.24095.tar", last modified: Thu Apr  4 12:26:40 2024, max compression
```

## Comparing `mo-dots-9.582.24095.tar` & `mo-dots-9.584.24095.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 03:46:54.933671 mo-dots-9.582.24095/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo-dots-9.582.24095/LICENSE
--rw-rw-rw-   0        0        0     5055 2024-04-04 03:46:54.933671 mo-dots-9.582.24095/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo-dots-9.582.24095/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 03:46:54.913897 mo-dots-9.582.24095/mo_dots/
--rw-rw-rw-   0        0        0    13942 2024-03-21 02:15:09.000000 mo-dots-9.582.24095/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16231 2024-03-18 01:53:34.000000 mo-dots-9.582.24095/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4284 2024-03-16 18:16:18.000000 mo-dots-9.582.24095/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10290 2024-03-16 18:16:18.000000 mo-dots-9.582.24095/mo_dots/lists.py
--rw-rw-rw-   0        0        0     6568 2024-03-16 18:16:18.000000 mo-dots-9.582.24095/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5298 2024-03-16 19:13:23.000000 mo-dots-9.582.24095/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1424 2024-03-14 10:01:33.000000 mo-dots-9.582.24095/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:46:54.929659 mo-dots-9.582.24095/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5055 2024-04-04 03:46:54.000000 mo-dots-9.582.24095/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-04 03:46:54.000000 mo-dots-9.582.24095/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 03:46:54.000000 mo-dots-9.582.24095/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo-dots-9.582.24095/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-04 03:46:54.000000 mo-dots-9.582.24095/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 03:46:54.000000 mo-dots-9.582.24095/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 03:46:54.933671 mo-dots-9.582.24095/setup.cfg
--rw-rw-rw-   0        0        0     4937 2024-04-04 03:46:49.000000 mo-dots-9.582.24095/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:26:40.693418 mo-dots-9.584.24095/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo-dots-9.584.24095/LICENSE
+-rw-rw-rw-   0        0        0     5055 2024-04-04 12:26:40.692339 mo-dots-9.584.24095/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo-dots-9.584.24095/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:26:40.680857 mo-dots-9.584.24095/mo_dots/
+-rw-rw-rw-   0        0        0    13942 2024-03-21 02:15:09.000000 mo-dots-9.584.24095/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16231 2024-03-18 01:53:34.000000 mo-dots-9.584.24095/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4284 2024-03-16 18:16:18.000000 mo-dots-9.584.24095/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10290 2024-03-16 18:16:18.000000 mo-dots-9.584.24095/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     6568 2024-03-16 18:16:18.000000 mo-dots-9.584.24095/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5298 2024-03-16 19:13:23.000000 mo-dots-9.584.24095/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1424 2024-03-14 10:01:33.000000 mo-dots-9.584.24095/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:26:40.690250 mo-dots-9.584.24095/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5055 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo-dots-9.584.24095/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 12:26:40.000000 mo-dots-9.584.24095/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:26:40.693418 mo-dots-9.584.24095/setup.cfg
+-rw-rw-rw-   0        0        0     4937 2024-04-04 12:26:35.000000 mo-dots-9.584.24095/setup.py
```

### Comparing `mo-dots-9.582.24095/LICENSE` & `mo-dots-9.584.24095/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/PKG-INFO` & `mo-dots-9.584.24095/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.582.24095
+Version: 9.584.24095
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-imports==7.546.24057
+Requires-Dist: mo-future==7.584.24095
+Requires-Dist: mo-imports==7.584.24095
 Provides-Extra: tests
 Requires-Dist: mo-logs>=8.562.24075; extra == "tests"
 Requires-Dist: mo-json>=6.562.24075; extra == "tests"
 Requires-Dist: mo-threads>=6.562.24075; extra == "tests"
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 Requires-Dist: pyLibrary>=3.264.22338; extra == "tests"
 Requires-Dist: mo-math>=7.562.24075; extra == "tests"
```

### Comparing `mo-dots-9.582.24095/README.md` & `mo-dots-9.584.24095/README.md`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots/__init__.py` & `mo-dots-9.584.24095/mo_dots/__init__.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots/datas.py` & `mo-dots-9.584.24095/mo_dots/datas.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots/fields.py` & `mo-dots-9.584.24095/mo_dots/fields.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots/lists.py` & `mo-dots-9.584.24095/mo_dots/lists.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots/nones.py` & `mo-dots-9.584.24095/mo_dots/nones.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots/objects.py` & `mo-dots-9.584.24095/mo_dots/objects.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots/utils.py` & `mo-dots-9.584.24095/mo_dots/utils.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.582.24095/mo_dots.egg-info/PKG-INFO` & `mo-dots-9.584.24095/mo_dots.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.582.24095
+Version: 9.584.24095
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-imports==7.546.24057
+Requires-Dist: mo-future==7.584.24095
+Requires-Dist: mo-imports==7.584.24095
 Provides-Extra: tests
 Requires-Dist: mo-logs>=8.562.24075; extra == "tests"
 Requires-Dist: mo-json>=6.562.24075; extra == "tests"
 Requires-Dist: mo-threads>=6.562.24075; extra == "tests"
 Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
 Requires-Dist: pyLibrary>=3.264.22338; extra == "tests"
 Requires-Dist: mo-math>=7.562.24075; extra == "tests"
```

### Comparing `mo-dots-9.582.24095/setup.py` & `mo-dots-9.584.24095/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 5 - Production/Stable","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Dots! Dot-access to Python dicts like Javascript',
     extras_require={"tests":["mo-logs>=8.562.24075","mo-json>=6.562.24075","mo-threads>=6.562.24075","mo-testing>=7.562.24075","pyLibrary>=3.264.22338","mo-math>=7.562.24075","mo-times>=5.562.24075","jx-elasticsearch>=3.99.20292"]},
     include_package_data=True,
-    install_requires=["mo-future==7.546.24057","mo-imports==7.546.24057"],
+    install_requires=["mo-future==7.584.24095","mo-imports==7.584.24095"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, and acts much like a null-safe dataclass.\n\n> See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> from mo_dots import Data\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> from mo_dots import to_data\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list (`[]`) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.582.24095',
+    version='9.584.24095',
     zip_safe=False
 )
```

