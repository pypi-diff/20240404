# Comparing `tmp/enum_with_dict-0.5.1.tar.gz` & `tmp/enum_with_dict-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.5.1.tar", last modified: Wed Apr  3 23:57:31 2024, max compression
+gzip compressed data, was "enum_with_dict-0.5.2.tar", last modified: Wed Apr  3 23:59:30 2024, max compression
```

## Comparing `enum_with_dict-0.5.1.tar` & `enum_with_dict-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:57:31.629250 enum_with_dict-0.5.1/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.5.1/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     4950 2024-04-03 23:57:31.628946 enum_with_dict-0.5.1/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4039 2024-04-03 23:56:18.000000 enum_with_dict-0.5.1/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:57:31.627134 enum_with_dict-0.5.1/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.5.1/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     4876 2024-04-03 23:56:42.000000 enum_with_dict-0.5.1/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:57:31.627833 enum_with_dict-0.5.1/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     4950 2024-04-03 23:57:31.000000 enum_with_dict-0.5.1/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 23:57:31.000000 enum_with_dict-0.5.1/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 23:57:31.000000 enum_with_dict-0.5.1/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 23:57:31.000000 enum_with_dict-0.5.1/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 23:57:31.629314 enum_with_dict-0.5.1/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 23:53:48.000000 enum_with_dict-0.5.1/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:57:31.628094 enum_with_dict-0.5.1/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.5.1/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5829 2024-04-03 23:50:18.000000 enum_with_dict-0.5.1/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.788669 enum_with_dict-0.5.2/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.5.2/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     4952 2024-04-03 23:59:30.788399 enum_with_dict-0.5.2/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4041 2024-04-03 23:58:28.000000 enum_with_dict-0.5.2/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.787097 enum_with_dict-0.5.2/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.5.2/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     4878 2024-04-03 23:58:58.000000 enum_with_dict-0.5.2/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.787652 enum_with_dict-0.5.2/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     4952 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 23:59:30.788714 enum_with_dict-0.5.2/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 23:59:05.000000 enum_with_dict-0.5.2/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.787876 enum_with_dict-0.5.2/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.5.2/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5829 2024-04-03 23:50:18.000000 enum_with_dict-0.5.2/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.5.1/LICENSE` & `enum_with_dict-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.5.1/PKG-INFO` & `enum_with_dict-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.5.1
+Version: 0.5.2
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -113,15 +113,15 @@
 
 ### Mapping Enum Members with `map`
 
 Map enum members to values using the provided dictionary.
 
 This mapping operation does not alter the values within the Enum itself; instead, it generates a new dictionary with the same keys and updated values.
 
-Internally, validate_mapping_keys is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
+Internally, `validate_mapping_keys` is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
 
 ```python
 # Define the key mapping
 key_mapping = {
     TestEnum.VALUE_1: "some_new_value",
     TestEnum.VALUE_2: "another_new_value",
     TestEnum.VALUE_3: "a new value"
```

### Comparing `enum_with_dict-0.5.1/README.md` & `enum_with_dict-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 ### Mapping Enum Members with `map`
 
 Map enum members to values using the provided dictionary.
 
 This mapping operation does not alter the values within the Enum itself; instead, it generates a new dictionary with the same keys and updated values.
 
-Internally, validate_mapping_keys is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
+Internally, `validate_mapping_keys` is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
 
 ```python
 # Define the key mapping
 key_mapping = {
     TestEnum.VALUE_1: "some_new_value",
     TestEnum.VALUE_2: "another_new_value",
     TestEnum.VALUE_3: "a new value"
```

### Comparing `enum_with_dict-0.5.1/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.5.2/enum_with_dict/enum_with_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     @classmethod
     def map(cls, key_mapping: Dict[Enum, Any]) -> Dict[Enum, Any]:
         """Map enum members to values using the provided dictionary.
 
         This mapping operation does not alter the values within the Enum itself; instead, it generates a new dictionary with the same keys and updated values.
 
-        Internally, validate_mapping_keys is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
+        Internally, `validate_mapping_keys` is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
 
         Args:
             key_mapping (Dict[Enum, Any]): A dictionary mapping enum members to new values.
 
         Returns:
             Dict[Enum, Any]: A dictionary containing the mapped enum members with their corresponding new values.
```

### Comparing `enum_with_dict-0.5.1/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.5.2/enum_with_dict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.5.1
+Version: 0.5.2
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -113,15 +113,15 @@
 
 ### Mapping Enum Members with `map`
 
 Map enum members to values using the provided dictionary.
 
 This mapping operation does not alter the values within the Enum itself; instead, it generates a new dictionary with the same keys and updated values.
 
-Internally, validate_mapping_keys is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
+Internally, `validate_mapping_keys` is invoked to confirm that the keys align with the Enum members, but the value types remain arbitrary.
 
 ```python
 # Define the key mapping
 key_mapping = {
     TestEnum.VALUE_1: "some_new_value",
     TestEnum.VALUE_2: "another_new_value",
     TestEnum.VALUE_3: "a new value"
```

### Comparing `enum_with_dict-0.5.1/setup.py` & `enum_with_dict-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.5.1',
+    version='0.5.2',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/enum_with_dict',
```

### Comparing `enum_with_dict-0.5.1/test/test_enum_with_dict.py` & `enum_with_dict-0.5.2/test/test_enum_with_dict.py`

 * *Files identical despite different names*

