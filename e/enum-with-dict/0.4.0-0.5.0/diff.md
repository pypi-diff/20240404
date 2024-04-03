# Comparing `tmp/enum_with_dict-0.4.0.tar.gz` & `tmp/enum_with_dict-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.4.0.tar", last modified: Wed Apr  3 21:14:05 2024, max compression
+gzip compressed data, was "enum_with_dict-0.5.0.tar", last modified: Wed Apr  3 23:50:22 2024, max compression
```

## Comparing `enum_with_dict-0.4.0.tar` & `enum_with_dict-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.925396 enum_with_dict-0.4.0/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.4.0/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     4835 2024-04-03 21:14:05.925166 enum_with_dict-0.4.0/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     3924 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.923592 enum_with_dict-0.4.0/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.4.0/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     4574 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.924417 enum_with_dict-0.4.0/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     4835 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 21:14:05.925438 enum_with_dict-0.4.0/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.924646 enum_with_dict-0.4.0/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.4.0/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5832 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:50:22.134287 enum_with_dict-0.5.0/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.5.0/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     4832 2024-04-03 23:50:22.134069 enum_with_dict-0.5.0/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     3921 2024-04-03 23:50:18.000000 enum_with_dict-0.5.0/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:50:22.133017 enum_with_dict-0.5.0/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.5.0/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     4717 2024-04-03 23:50:18.000000 enum_with_dict-0.5.0/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:50:22.133548 enum_with_dict-0.5.0/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     4832 2024-04-03 23:50:22.000000 enum_with_dict-0.5.0/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 23:50:22.000000 enum_with_dict-0.5.0/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 23:50:22.000000 enum_with_dict-0.5.0/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 23:50:22.000000 enum_with_dict-0.5.0/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 23:50:22.134328 enum_with_dict-0.5.0/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 23:50:18.000000 enum_with_dict-0.5.0/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:50:22.133757 enum_with_dict-0.5.0/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.5.0/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5829 2024-04-03 23:50:18.000000 enum_with_dict-0.5.0/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.4.0/LICENSE` & `enum_with_dict-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.4.0/PKG-INFO` & `enum_with_dict-0.5.0/enum_with_dict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enum_with_dict
-Version: 0.4.0
+Name: enum-with-dict
+Version: 0.5.0
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -129,17 +129,17 @@
 # Perform the mapping and validate
 mapped_values = TestEnum.map(key_mapping)
 
 # ----- The above is equivalent to the following: -----
 
 # Validate the mapped values
 expected_values = {
-    TestEnum.VALUE_1.value: "some_new_value",
-    TestEnum.VALUE_2.value: "another_new_value",
-    TestEnum.VALUE_3.value: "a new value"
+    TestEnum.VALUE_1.name: "some_new_value",
+    TestEnum.VALUE_2.name: "another_new_value",
+    TestEnum.VALUE_3.name: "a new value"
 }
 
 assert mapped_values == expected_values
 
 ```
 
 ## Retrieving Keys and Values with `keys()` and `values()`
```

### Comparing `enum_with_dict-0.4.0/README.md` & `enum_with_dict-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 # Perform the mapping and validate
 mapped_values = TestEnum.map(key_mapping)
 
 # ----- The above is equivalent to the following: -----
 
 # Validate the mapped values
 expected_values = {
-    TestEnum.VALUE_1.value: "some_new_value",
-    TestEnum.VALUE_2.value: "another_new_value",
-    TestEnum.VALUE_3.value: "a new value"
+    TestEnum.VALUE_1.name: "some_new_value",
+    TestEnum.VALUE_2.name: "another_new_value",
+    TestEnum.VALUE_3.name: "a new value"
 }
 
 assert mapped_values == expected_values
 
 ```
 
 ## Retrieving Keys and Values with `keys()` and `values()`
```

### Comparing `enum_with_dict-0.4.0/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.5.0/enum_with_dict/enum_with_dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,17 @@
         
         return True
 
     @classmethod
     def map(cls, key_mapping: Dict[Enum, Any]) -> Dict[Enum, Any]:
         """Map enum members to values based on the provided dictionary.
 
+        Note! This does not change the values in the Enum itself, but returns a
+        dictionary with the same keys and newly mapped values.
+
         Args:
             key_mapping (Dict[Enum, Any]): A dictionary mapping enum members to new values.
 
         Returns:
             Dict[Enum, Any]: A dictionary containing the mapped enum members with their corresponding new values.
 
         Raises:
@@ -110,9 +113,9 @@
         # Validate the new mapping
         cls.validate_mapping_keys({**cls.to_dict(), **{member.name: value for member, value in key_mapping.items()}})
         
         # Map enum members to values
         mapped_values = {}
         for member in cls:
             if member in key_mapping:
-                mapped_values[member.value] = key_mapping[member]
+                mapped_values[member.name] = key_mapping[member]
         return mapped_values
```

### Comparing `enum_with_dict-0.4.0/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enum-with-dict
-Version: 0.4.0
+Name: enum_with_dict
+Version: 0.5.0
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -129,17 +129,17 @@
 # Perform the mapping and validate
 mapped_values = TestEnum.map(key_mapping)
 
 # ----- The above is equivalent to the following: -----
 
 # Validate the mapped values
 expected_values = {
-    TestEnum.VALUE_1.value: "some_new_value",
-    TestEnum.VALUE_2.value: "another_new_value",
-    TestEnum.VALUE_3.value: "a new value"
+    TestEnum.VALUE_1.name: "some_new_value",
+    TestEnum.VALUE_2.name: "another_new_value",
+    TestEnum.VALUE_3.name: "a new value"
 }
 
 assert mapped_values == expected_values
 
 ```
 
 ## Retrieving Keys and Values with `keys()` and `values()`
```

### Comparing `enum_with_dict-0.4.0/setup.py` & `enum_with_dict-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.4.0',
+    version='0.5.0',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/enum_with_dict',
```

### Comparing `enum_with_dict-0.4.0/test/test_enum_with_dict.py` & `enum_with_dict-0.5.0/test/test_enum_with_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,17 @@
         key_mapping = {
             TestEnum.VALUE_1: "some_new_value",
             TestEnum.VALUE_2: "another_new_value",
             TestEnum.VALUE_3: "a new value"
         }
 
         self.assertEqual(TestEnum.map(key_mapping), {
-            TestEnum.VALUE_1.value: "some_new_value",
-            TestEnum.VALUE_2.value: "another_new_value",
-            TestEnum.VALUE_3.value: "a new value"
+            TestEnum.VALUE_1.name: "some_new_value",
+            TestEnum.VALUE_2.name: "another_new_value",
+            TestEnum.VALUE_3.name: "a new value"
         })
 
     def test_map_invalid_key(self):
         """Test mapping enum members to values with invalid keys."""
         class TestEnum(EnumWithDict):
             VALUE_1 = 1
             VALUE_2 = 2
```

