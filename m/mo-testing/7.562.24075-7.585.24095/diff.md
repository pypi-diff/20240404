# Comparing `tmp/mo-testing-7.562.24075.tar.gz` & `tmp/mo-testing-7.585.24095.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-testing-7.562.24075.tar", last modified: Fri Mar 15 11:57:58 2024, max compression
+gzip compressed data, was "mo-testing-7.585.24095.tar", last modified: Thu Apr  4 12:52:10 2024, max compression
```

## Comparing `mo-testing-7.562.24075.tar` & `mo-testing-7.585.24095.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 11:57:58.167331 mo-testing-7.562.24075/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo-testing-7.562.24075/LICENSE
--rw-rw-rw-   0        0        0     2047 2024-03-15 11:57:58.165187 mo-testing-7.562.24075/PKG-INFO
--rw-rw-rw-   0        0        0      946 2020-05-12 21:52:10.000000 mo-testing-7.562.24075/README.md
-drwxrwxrwx   0        0        0        0 2024-03-15 11:57:58.149424 mo-testing-7.562.24075/mo_testing/
--rw-rw-rw-   0        0        0      317 2024-03-11 07:12:55.000000 mo-testing-7.562.24075/mo_testing/__init__.py
--rw-rw-rw-   0        0        0    11510 2024-03-15 11:57:51.000000 mo-testing-7.562.24075/mo_testing/fuzzytestcase.py
-drwxrwxrwx   0        0        0        0 2024-03-15 11:57:58.163823 mo-testing-7.562.24075/mo_testing.egg-info/
--rw-rw-rw-   0        0        0     2047 2024-03-15 11:57:58.000000 mo-testing-7.562.24075/mo_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-03-15 11:57:58.000000 mo-testing-7.562.24075/mo_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 11:57:58.000000 mo-testing-7.562.24075/mo_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2024-03-15 11:57:58.000000 mo-testing-7.562.24075/mo_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-15 11:57:58.000000 mo-testing-7.562.24075/mo_testing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-15 11:57:58.167331 mo-testing-7.562.24075/setup.cfg
--rw-rw-rw-   0        0        0     2092 2024-03-15 11:57:53.000000 mo-testing-7.562.24075/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-15 11:57:58.162585 mo-testing-7.562.24075/tests/
--rw-rw-rw-   0        0        0      822 2023-05-30 12:10:20.000000 mo-testing-7.562.24075/tests/test_assert_raises.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:52:10.315884 mo-testing-7.585.24095/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo-testing-7.585.24095/LICENSE
+-rw-rw-rw-   0        0        0     2047 2024-04-04 12:52:10.315884 mo-testing-7.585.24095/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2020-05-12 21:52:10.000000 mo-testing-7.585.24095/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:52:10.306527 mo-testing-7.585.24095/mo_testing/
+-rw-rw-rw-   0        0        0      449 2024-04-04 12:52:03.000000 mo-testing-7.585.24095/mo_testing/__init__.py
+-rw-rw-rw-   0        0        0    11718 2024-04-04 12:52:03.000000 mo-testing-7.585.24095/mo_testing/fuzzytestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:52:10.314832 mo-testing-7.585.24095/mo_testing.egg-info/
+-rw-rw-rw-   0        0        0     2047 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-04 12:52:10.000000 mo-testing-7.585.24095/mo_testing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:52:10.315884 mo-testing-7.585.24095/setup.cfg
+-rw-rw-rw-   0        0        0     2092 2024-04-04 12:52:06.000000 mo-testing-7.585.24095/setup.py
```

### Comparing `mo-testing-7.562.24075/LICENSE` & `mo-testing-7.585.24095/LICENSE`

 * *Files identical despite different names*

### Comparing `mo-testing-7.562.24075/PKG-INFO` & `mo-testing-7.585.24095/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 7.562.24075
+Version: 7.585.24095
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -12,20 +12,20 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.562.24075
-Requires-Dist: mo-dots==9.562.24075
-Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-logs==8.562.24075
-Requires-Dist: mo-math==7.562.24075
-Requires-Dist: mo-threads==6.562.24075
+Requires-Dist: mo-collections==5.584.24095
+Requires-Dist: mo-dots==9.584.24095
+Requires-Dist: mo-future==7.584.24095
+Requires-Dist: mo-logs==8.584.24095
+Requires-Dist: mo-math==7.584.24095
+Requires-Dist: mo-threads==6.585.24095
 Provides-Extra: tests
 
 # More Testing
 
 `FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.
```

### Comparing `mo-testing-7.562.24075/README.md` & `mo-testing-7.585.24095/README.md`

 * *Files identical despite different names*

### Comparing `mo-testing-7.562.24075/mo_testing/fuzzytestcase.py` & `mo-testing-7.585.24095/mo_testing/fuzzytestcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 
 import datetime
 import types
 import unittest
 from unittest import SkipTest, TestCase
 
-from mo_collections.unique_index import UniqueIndex
 import mo_dots
-from mo_dots import coalesce, is_container, is_list, literal_field, from_data, to_data, is_data, is_many
+import mo_math
+from mo_collections.unique_index import UniqueIndex
+from mo_dots import coalesce, is_list, literal_field, from_data, to_data, is_data, is_many
 from mo_future import is_text, zip_longest, first, get_function_name
 from mo_logs import Except, Log, suppress_exception
 from mo_logs.strings import expand_template, quote
-import mo_math
 from mo_math import is_number, log10
 from mo_times import dates
 
 
 class FuzzyTestCase(unittest.TestCase):
     """
     COMPARE STRUCTURE AND NUMBERS!
@@ -202,14 +202,20 @@
             dates.Date(expected).unix,
             msg=msg,
             digits=digits,
             places=places,
             delta=delta
         )
 
+    if not is_many(expected) and is_list(test) and len(test) == 1:
+        try:
+            return assertAlmostEqual(test[0], expected, msg=msg, digits=digits, places=places, delta=delta)
+        except:
+            pass
+
     if not is_number(expected):
         # SOME SPECIAL CASES, EXPECTING EMPTY CONTAINERS IS THE SAME AS EXPECTING NULL
         if is_list(expected) and len(expected) == 0 and test == None:
             return
         if is_data(expected) and not expected.keys() and test == None:
             return
         if test != expected:
```

### Comparing `mo-testing-7.562.24075/mo_testing.egg-info/PKG-INFO` & `mo-testing-7.585.24095/mo_testing.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 7.562.24075
+Version: 7.585.24095
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -12,20 +12,20 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-collections==5.562.24075
-Requires-Dist: mo-dots==9.562.24075
-Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-logs==8.562.24075
-Requires-Dist: mo-math==7.562.24075
-Requires-Dist: mo-threads==6.562.24075
+Requires-Dist: mo-collections==5.584.24095
+Requires-Dist: mo-dots==9.584.24095
+Requires-Dist: mo-future==7.584.24095
+Requires-Dist: mo-logs==8.584.24095
+Requires-Dist: mo-math==7.584.24095
+Requires-Dist: mo-threads==6.585.24095
 Provides-Extra: tests
 
 # More Testing
 
 `FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.
```

### Comparing `mo-testing-7.562.24075/setup.py` & `mo-testing-7.585.24095/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons',
     extras_require={"tests":[]},
     include_package_data=True,
-    install_requires=["mo-collections==5.562.24075","mo-dots==9.562.24075","mo-future==7.546.24057","mo-logs==8.562.24075","mo-math==7.562.24075","mo-threads==6.562.24075"],
+    install_requires=["mo-collections==5.584.24095","mo-dots==9.584.24095","mo-future==7.584.24095","mo-logs==8.584.24095","mo-math==7.584.24095","mo-threads==6.585.24095"],
     license='MPL 2.0',
     long_description='# More Testing\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertEqual` method with the following parameters:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n\n',
     long_description_content_type='text/markdown',
     name='mo-testing',
     packages=["mo_testing"],
     url='https://github.com/klahnakoski/mo-testing',
-    version='7.562.24075'
+    version='7.585.24095'
 )
```

