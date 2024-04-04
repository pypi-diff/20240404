# Comparing `tmp/mo-dots-9.574.24078.tar.gz` & `tmp/mo-dots-9.578.24081.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-dots-9.574.24078.tar", last modified: Mon Mar 18 01:53:41 2024, max compression
+gzip compressed data, was "mo-dots-9.578.24081.tar", last modified: Thu Mar 21 02:15:17 2024, max compression
```

## Comparing `mo-dots-9.574.24078.tar` & `mo-dots-9.578.24081.tar`

### file list

```diff
@@ -1,33 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 01:53:41.750917 mo-dots-9.574.24078/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo-dots-9.574.24078/LICENSE
--rw-rw-rw-   0        0        0     5035 2024-03-18 01:53:41.750917 mo-dots-9.574.24078/PKG-INFO
--rw-rw-rw-   0        0        0     3527 2024-03-02 19:49:25.000000 mo-dots-9.574.24078/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 01:53:41.721615 mo-dots-9.574.24078/mo_dots/
--rw-rw-rw-   0        0        0    13887 2024-03-16 22:31:28.000000 mo-dots-9.574.24078/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16231 2024-03-18 01:53:34.000000 mo-dots-9.574.24078/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4284 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10290 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/mo_dots/lists.py
--rw-rw-rw-   0        0        0     6568 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5298 2024-03-16 19:13:23.000000 mo-dots-9.574.24078/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1424 2024-03-14 10:01:33.000000 mo-dots-9.574.24078/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-18 01:53:41.750917 mo-dots-9.574.24078/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5035 2024-03-18 01:53:41.000000 mo-dots-9.574.24078/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-03-18 01:53:41.000000 mo-dots-9.574.24078/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 01:53:41.000000 mo-dots-9.574.24078/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-18 01:53:41.000000 mo-dots-9.574.24078/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-03-18 01:53:41.000000 mo-dots-9.574.24078/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-18 01:53:41.000000 mo-dots-9.574.24078/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 01:53:41.750917 mo-dots-9.574.24078/setup.cfg
--rw-rw-rw-   0        0        0     4918 2024-03-18 01:53:36.000000 mo-dots-9.574.24078/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 01:53:41.750917 mo-dots-9.574.24078/tests/
--rw-rw-rw-   0        0        0    32328 2024-03-18 01:53:34.000000 mo-dots-9.574.24078/tests/test_dot.py
--rw-rw-rw-   0        0        0    11082 2024-03-15 11:37:19.000000 mo-dots-9.574.24078/tests/test_dot_from_addict.py
--rw-rw-rw-   0        0        0    10191 2024-03-16 22:31:28.000000 mo-dots-9.574.24078/tests/test_dot_speed.py
--rw-rw-rw-   0        0        0     6461 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/tests/test_dotty_api.py
--rw-rw-rw-   0        0        0     1886 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/tests/test_dotty_basics.py
--rw-rw-rw-   0        0        0     6117 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/tests/test_dotty_value_access.py
--rw-rw-rw-   0        0        0     3895 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/tests/test_fields.py
--rw-rw-rw-   0        0        0      788 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/tests/test_json.py
--rw-rw-rw-   0        0        0    14252 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/tests/test_list.py
--rw-rw-rw-   0        0        0     5266 2024-03-16 19:13:23.000000 mo-dots-9.574.24078/tests/test_object.py
--rw-rw-rw-   0        0        0     2480 2024-03-16 18:16:18.000000 mo-dots-9.574.24078/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:15:17.305091 mo-dots-9.578.24081/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo-dots-9.578.24081/LICENSE
+-rw-rw-rw-   0        0        0     5035 2024-03-21 02:15:17.304080 mo-dots-9.578.24081/PKG-INFO
+-rw-rw-rw-   0        0        0     3527 2024-03-02 19:49:25.000000 mo-dots-9.578.24081/README.md
+drwxrwxrwx   0        0        0        0 2024-03-21 02:15:17.292209 mo-dots-9.578.24081/mo_dots/
+-rw-rw-rw-   0        0        0    13942 2024-03-21 02:15:09.000000 mo-dots-9.578.24081/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16231 2024-03-18 01:53:34.000000 mo-dots-9.578.24081/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4284 2024-03-16 18:16:18.000000 mo-dots-9.578.24081/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10290 2024-03-16 18:16:18.000000 mo-dots-9.578.24081/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     6568 2024-03-16 18:16:18.000000 mo-dots-9.578.24081/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5298 2024-03-16 19:13:23.000000 mo-dots-9.578.24081/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1424 2024-03-14 10:01:33.000000 mo-dots-9.578.24081/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-21 02:15:17.302082 mo-dots-9.578.24081/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5035 2024-03-21 02:15:17.000000 mo-dots-9.578.24081/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-03-21 02:15:17.000000 mo-dots-9.578.24081/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-21 02:15:17.000000 mo-dots-9.578.24081/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo-dots-9.578.24081/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-03-21 02:15:17.000000 mo-dots-9.578.24081/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-03-21 02:15:17.000000 mo-dots-9.578.24081/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-21 02:15:17.305091 mo-dots-9.578.24081/setup.cfg
+-rw-rw-rw-   0        0        0     4918 2024-03-21 02:15:12.000000 mo-dots-9.578.24081/setup.py
```

### Comparing `mo-dots-9.574.24078/LICENSE` & `mo-dots-9.578.24081/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/PKG-INFO` & `mo-dots-9.578.24081/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.574.24078
+Version: 9.578.24081
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-dots-9.574.24078/README.md` & `mo-dots-9.578.24081/README.md`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/mo_dots/__init__.py` & `mo-dots-9.578.24081/mo_dots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,56 +15,59 @@
 from mo_dots.lists import *
 from mo_dots.nones import *
 from mo_dots.objects import DataObject, DataClass, object_to_data
 from mo_dots.utils import get_module, CLASS, get_logger, SLOT
 
 
 __all__ = [
+    "coalesce",
+    "concat_field",
     "Data",
-    "DataObject",
     "DataClass",
-    "FlatList",
-    "Null",
-    "NullType",
-    "coalesce",
+    "DataObject",
     "datawrap",
+    "dict_to_data",
+    "endswith_field",
+    "exists",
+    "FlatList",
     "from_data",
     "get_attr",
+    "hash_value",
+    "inverse",
+    "is_container",
+    "is_data",
+    "is_list",
+    "is_many",
+    "is_missing",
+    "is_not_null",
     "is_null",
+    "is_sequence",
+    "join_field",
+    "last",
+    "leaves",
+    "leaves_to_data",
+    "list_to_data",
     "listwrap",
+    "literal_field",
+    "missing",
+    "Null",
+    "NullType",
     "object_to_data",
+    "PATH_NOT_FOUND",
+    "relative_field",
     "set_attr",
     "set_default",
-    "to_data",
-    "unwrap",
-    "unwraplist",
-    "leaves_to_data",
-    "literal_field",
-    "join_field",
     "split_field",
     "startswith_field",
-    "endswith_field",
-    "is_missing",
-    "exists",
-    "leaves",
-    "PATH_NOT_FOUND",
-    "relative_field",
     "tail_field",
-    "unliteral_field",
-    "last",
-    "is_data",
-    "is_many",
-    "is_not_null",
+    "to_data",
     "tuplewrap",
-    "missing",
-    "hash_value",
-    "inverse",
-    "concat_field",
-    "list_to_data",
-    "is_container"
+    "unliteral_field",
+    "unwrap",
+    "unwraplist",
 ]
 
 
 _module_type = type(sys.modules[__name__])
 _builtin_zip = zip
 _get = object.__getattribute__
 _set = object.__setattr__
```

### Comparing `mo-dots-9.574.24078/mo_dots/datas.py` & `mo-dots-9.578.24081/mo_dots/datas.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/mo_dots/fields.py` & `mo-dots-9.578.24081/mo_dots/fields.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/mo_dots/lists.py` & `mo-dots-9.578.24081/mo_dots/lists.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/mo_dots/nones.py` & `mo-dots-9.578.24081/mo_dots/nones.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/mo_dots/objects.py` & `mo-dots-9.578.24081/mo_dots/objects.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/mo_dots/utils.py` & `mo-dots-9.578.24081/mo_dots/utils.py`

 * *Files identical despite different names*

### Comparing `mo-dots-9.574.24078/mo_dots.egg-info/PKG-INFO` & `mo-dots-9.578.24081/mo_dots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.574.24078
+Version: 9.578.24081
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo-dots-9.574.24078/setup.py` & `mo-dots-9.578.24081/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     install_requires=["mo-future==7.546.24057","mo-imports==7.546.24057"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, with additional features. \n\n    >>> from mo_dots import to_data, Data\n\n*See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`*\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\ta == {}\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    a == {}\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list ([]) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.574.24078',
+    version='9.578.24081',
     zip_safe=False
 )
```

