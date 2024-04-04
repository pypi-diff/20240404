# Comparing `tmp/enum_with_dict-0.6.0.tar.gz` & `tmp/enum_with_dict-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.6.0.tar", last modified: Thu Apr  4 00:11:47 2024, max compression
+gzip compressed data, was "enum_with_dict-0.6.1.tar", last modified: Thu Apr  4 03:55:00 2024, max compression
```

## Comparing `enum_with_dict-0.6.0.tar` & `enum_with_dict-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.820879 enum_with_dict-0.6.0/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.6.0/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:11:47.820603 enum_with_dict-0.6.0/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4041 2024-04-03 23:58:28.000000 enum_with_dict-0.6.0/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.819461 enum_with_dict-0.6.0/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.6.0/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5177 2024-04-04 00:11:41.000000 enum_with_dict-0.6.0/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.820024 enum_with_dict-0.6.0/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 00:11:47.820923 enum_with_dict-0.6.0/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 00:11:41.000000 enum_with_dict-0.6.0/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.820249 enum_with_dict-0.6.0/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.6.0/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5825 2024-04-04 00:11:41.000000 enum_with_dict-0.6.0/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.035317 enum_with_dict-0.6.1/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.6.1/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 03:55:00.035043 enum_with_dict-0.6.1/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4114 2024-04-04 00:26:57.000000 enum_with_dict-0.6.1/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.033413 enum_with_dict-0.6.1/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.6.1/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5177 2024-04-04 00:11:41.000000 enum_with_dict-0.6.1/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.034260 enum_with_dict-0.6.1/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 03:55:00.035371 enum_with_dict-0.6.1/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 03:54:58.000000 enum_with_dict-0.6.1/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.034573 enum_with_dict-0.6.1/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.6.1/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5819 2024-04-04 03:54:58.000000 enum_with_dict-0.6.1/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.6.0/LICENSE` & `enum_with_dict-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.6.0/PKG-INFO` & `enum_with_dict-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.6.0
+Version: 0.6.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py_enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -20,17 +20,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EnumWithDict
 
-`EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
+`EnumWithDict` is a Python package that extends the standard library's Enum class to include `to_dict`, `get_initial`, and other class methods. This enhancement allows for the straightforward conversion of enum classes to dictionaries, easy access to the initial enum value, and additional functionalities such as retrieving enum values with a fallback option, validating mappings, and more.
 
-## Features
+## Extends Enum with the Following Methods:
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
 - **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
 - **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
```

### Comparing `enum_with_dict-0.6.0/README.md` & `enum_with_dict-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # EnumWithDict
 
-`EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
+`EnumWithDict` is a Python package that extends the standard library's Enum class to include `to_dict`, `get_initial`, and other class methods. This enhancement allows for the straightforward conversion of enum classes to dictionaries, easy access to the initial enum value, and additional functionalities such as retrieving enum values with a fallback option, validating mappings, and more.
 
-## Features
+## Extends Enum with the Following Methods:
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
 - **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
 - **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
```

### Comparing `enum_with_dict-0.6.0/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.6.1/enum_with_dict/enum_with_dict.py`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.6.0/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.6.1/enum_with_dict.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.6.0
+Version: 0.6.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py_enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -20,17 +20,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EnumWithDict
 
-`EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
+`EnumWithDict` is a Python package that extends the standard library's Enum class to include `to_dict`, `get_initial`, and other class methods. This enhancement allows for the straightforward conversion of enum classes to dictionaries, easy access to the initial enum value, and additional functionalities such as retrieving enum values with a fallback option, validating mappings, and more.
 
-## Features
+## Extends Enum with the Following Methods:
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
 - **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
 - **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
```

### Comparing `enum_with_dict-0.6.0/setup.py` & `enum_with_dict-0.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.6.0',
+    version='0.6.1',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/py_enum_with_dict',
```

### Comparing `enum_with_dict-0.6.0/test/test_enum_with_dict.py` & `enum_with_dict-0.6.1/test/test_enum_with_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,20 @@
         with self.assertRaises(KeyError) as context:
             ExtendEnum.validate_mapping_keys(dict_mapping)
 
     def test_validate_self_mapping(self):
         """Test validation succeeds against self."""
 
         class Mixed(EnumWithDict):
-            NUMBER = 1,
-            ZERO = 0,
-            STRING = "string",
-            TRUE = True,
-            FALSE = False,
-            FUNCTION = len,
+            NUMBER = 1
+            ZERO = 0
+            STRING = "string"
+            TRUE = True
+            FALSE = False
+            FUNCTION = len
             NONE = None
 
         # Convert enum to dict and validate
         dict_mapping = Mixed.to_dict()
         self.assertTrue(Mixed.validate_mapping_keys(dict_mapping))
 
     def test_map(self):
```

