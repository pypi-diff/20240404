# Comparing `tmp/enum_with_dict-0.6.2.tar.gz` & `tmp/enum_with_dict-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.6.2.tar", last modified: Thu Apr  4 04:19:12 2024, max compression
+gzip compressed data, was "enum_with_dict-0.7.0.tar", last modified: Thu Apr  4 10:45:41 2024, max compression
```

## Comparing `enum_with_dict-0.6.2.tar` & `enum_with_dict-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.579190 enum_with_dict-0.6.2/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.6.2/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 04:19:12.578939 enum_with_dict-0.6.2/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4114 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.577849 enum_with_dict-0.6.2/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.6.2/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5144 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.578349 enum_with_dict-0.6.2/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 04:19:12.579234 enum_with_dict-0.6.2/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.578585 enum_with_dict-0.6.2/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.6.2/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     6320 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.104351 enum_with_dict-0.7.0/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.7.0/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 10:45:41.104143 enum_with_dict-0.7.0/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4675 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.103036 enum_with_dict-0.7.0/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.7.0/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     6048 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.103602 enum_with_dict-0.7.0/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 10:45:41.104391 enum_with_dict-0.7.0/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.103816 enum_with_dict-0.7.0/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.7.0/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     8006 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.6.2/LICENSE` & `enum_with_dict-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.6.2/PKG-INFO` & `enum_with_dict-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,16 @@
-Metadata-Version: 2.1
-Name: enum_with_dict
-Version: 0.6.2
-Summary: Enum with to_dict method.
-Home-page: https://github.com/jzombie/py-enum-with-dict
-Author: Jeremy Harris
-Author-email: jeremy.harris@zenosmosis.com
-License: MIT
-Keywords: enum python utilities enum-to-dict enum-with-dict
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # EnumWithDict
 
 `EnumWithDict` is a Python package that extends the standard library's Enum class to include `to_dict`, `get_initial`, and other class methods. This enhancement allows for the straightforward conversion of enum classes to dictionaries, easy access to the initial enum value, and additional functionalities such as retrieving enum values with a fallback option, validating mappings, and more.
 
 ## Extends Enum with the Following Methods:
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
-- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
+- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback. Additionally, it supports an optional custom mapping dictionary for dynamically mapped value retrieval.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
 - **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
 - **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
@@ -72,15 +48,15 @@
 initial_color = Color.get_initial()
 print(initial_color)
 # Output: 'red'
 ```
 
 ### Using the `get` Method
 
-Retrieve an enum value by its name, with an option to specify a default value if the name does not exist.
+Retrieve an enum value by its name, with an option to specify a default value if the name does not exist. Additionally, you can pass a custom mapping dictionary to retrieve a mapped value instead of the enum's default value.
 
 #### Get a value for an existing key
 
 ```python
 print(Color.get('RED'))  # Output: 'red'
 ```
 
@@ -92,14 +68,23 @@
 
 ### Get a value for a non-existing key, falling back to the initial value
 
 ```python
 print(Color.get('PURPLE'))  # Output: 'red'
 ```
 
+### Get a value using a custom mapping
+
+You can also use a custom mapping dictionary to retrieve a value. This is useful when you need to map enum members to different values dynamically.
+
+```python
+custom_mapping = {'RED': 'Rouge', 'GREEN': 'Vert', 'BLUE': 'Bleu'}
+print(Color.get('RED', mapping=custom_mapping))  # Output: 'Rouge'
+```
+
 ## Ensuring Completeness of Mappings with `validate_mapping_keys`
 
 Validate that a provided mapping covers all enum members.
 
 ```python
 # Assuming a partial mapping for demonstration
 partial_mapping = {'RED': 'Rouge', 'GREEN': 'Vert'}
```

### Comparing `enum_with_dict-0.6.2/README.md` & `enum_with_dict-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,40 @@
+Metadata-Version: 2.1
+Name: enum_with_dict
+Version: 0.7.0
+Summary: Enum with to_dict method.
+Home-page: https://github.com/jzombie/py-enum-with-dict
+Author: Jeremy Harris
+Author-email: jeremy.harris@zenosmosis.com
+License: MIT
+Keywords: enum python utilities enum-to-dict enum-with-dict
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # EnumWithDict
 
 `EnumWithDict` is a Python package that extends the standard library's Enum class to include `to_dict`, `get_initial`, and other class methods. This enhancement allows for the straightforward conversion of enum classes to dictionaries, easy access to the initial enum value, and additional functionalities such as retrieving enum values with a fallback option, validating mappings, and more.
 
 ## Extends Enum with the Following Methods:
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
-- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
+- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback. Additionally, it supports an optional custom mapping dictionary for dynamically mapped value retrieval.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
 - **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
 - **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
@@ -48,15 +72,15 @@
 initial_color = Color.get_initial()
 print(initial_color)
 # Output: 'red'
 ```
 
 ### Using the `get` Method
 
-Retrieve an enum value by its name, with an option to specify a default value if the name does not exist.
+Retrieve an enum value by its name, with an option to specify a default value if the name does not exist. Additionally, you can pass a custom mapping dictionary to retrieve a mapped value instead of the enum's default value.
 
 #### Get a value for an existing key
 
 ```python
 print(Color.get('RED'))  # Output: 'red'
 ```
 
@@ -68,14 +92,23 @@
 
 ### Get a value for a non-existing key, falling back to the initial value
 
 ```python
 print(Color.get('PURPLE'))  # Output: 'red'
 ```
 
+### Get a value using a custom mapping
+
+You can also use a custom mapping dictionary to retrieve a value. This is useful when you need to map enum members to different values dynamically.
+
+```python
+custom_mapping = {'RED': 'Rouge', 'GREEN': 'Vert', 'BLUE': 'Bleu'}
+print(Color.get('RED', mapping=custom_mapping))  # Output: 'Rouge'
+```
+
 ## Ensuring Completeness of Mappings with `validate_mapping_keys`
 
 Validate that a provided mapping covers all enum members.
 
 ```python
 # Assuming a partial mapping for demonstration
 partial_mapping = {'RED': 'Rouge', 'GREEN': 'Vert'}
```

### Comparing `enum_with_dict-0.6.2/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.7.0/enum_with_dict/enum_with_dict.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,39 @@
 
     @classmethod
     def get_initial(cls) -> Any:
         """Get the first value from the enum dictionary."""
         return next(iter(cls.to_dict().values()))
 
     @classmethod
-    def get(cls, key: str, default: Any = None) -> Any:
-        """Get the value for the given key or return default or initial value."""
-        # If default is not provided, use the initial value
+    def get(cls, key: str, default: Any = None, mapping: Dict[str, Any] = None) -> Any:
+        """
+        Get the value for the given key from the optional mapping or the enum,
+        return default or initial value if not found.
+        
+        Args:
+            key (str): The key to look for.
+            default (Any, optional): The default value to return if the key is not found. 
+                                    If not provided, the initial enum value is used.
+            mapping (Dict[str, Any], optional): An optional mapping of keys to custom values.
+        
+        Returns:
+            Any: The value associated with the key, either from the mapping or the enum's default values.
+        """
+        # Use the initial value as the default if no default is provided
         if default is None:
             default = cls.get_initial()
+        
+        # If a mapping is provided, try to get the value from it
+        if mapping is not None:
+            cls.validate_mapping_keys(mapping)
+
+            return mapping.get(key, default)
+        
+        # Fallback to the enum's default values if no mapping is provided or the key is not in the mapping
         return cls.to_dict().get(key, default)
     
     @classmethod
     def keys(cls, as_list = True) -> Union[List[str], KeysView[str]]:
         """
         Return a view of the keys of the enum class as a list or as a `KeysView`.
```

### Comparing `enum_with_dict-0.6.2/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.7.0/enum_with_dict.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.6.2
+Version: 0.7.0
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py-enum-with-dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -26,15 +26,15 @@
 
 `EnumWithDict` is a Python package that extends the standard library's Enum class to include `to_dict`, `get_initial`, and other class methods. This enhancement allows for the straightforward conversion of enum classes to dictionaries, easy access to the initial enum value, and additional functionalities such as retrieving enum values with a fallback option, validating mappings, and more.
 
 ## Extends Enum with the Following Methods:
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
-- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
+- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback. Additionally, it supports an optional custom mapping dictionary for dynamically mapped value retrieval.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
 - **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
 - **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
@@ -72,15 +72,15 @@
 initial_color = Color.get_initial()
 print(initial_color)
 # Output: 'red'
 ```
 
 ### Using the `get` Method
 
-Retrieve an enum value by its name, with an option to specify a default value if the name does not exist.
+Retrieve an enum value by its name, with an option to specify a default value if the name does not exist. Additionally, you can pass a custom mapping dictionary to retrieve a mapped value instead of the enum's default value.
 
 #### Get a value for an existing key
 
 ```python
 print(Color.get('RED'))  # Output: 'red'
 ```
 
@@ -92,14 +92,23 @@
 
 ### Get a value for a non-existing key, falling back to the initial value
 
 ```python
 print(Color.get('PURPLE'))  # Output: 'red'
 ```
 
+### Get a value using a custom mapping
+
+You can also use a custom mapping dictionary to retrieve a value. This is useful when you need to map enum members to different values dynamically.
+
+```python
+custom_mapping = {'RED': 'Rouge', 'GREEN': 'Vert', 'BLUE': 'Bleu'}
+print(Color.get('RED', mapping=custom_mapping))  # Output: 'Rouge'
+```
+
 ## Ensuring Completeness of Mappings with `validate_mapping_keys`
 
 Validate that a provided mapping covers all enum members.
 
 ```python
 # Assuming a partial mapping for demonstration
 partial_mapping = {'RED': 'Rouge', 'GREEN': 'Vert'}
```

### Comparing `enum_with_dict-0.6.2/setup.py` & `enum_with_dict-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.6.2',
+    version='0.7.0',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/py-enum-with-dict',
```

### Comparing `enum_with_dict-0.6.2/test/test_enum_with_dict.py` & `enum_with_dict-0.7.0/test/test_enum_with_dict.py`

 * *Files 11% similar despite different names*

```diff
@@ -174,9 +174,52 @@
             VALUE_3 = 3
 
         self.assertEqual(TestEnum.values(), [1,2,3])
 
         self.assertNotEqual(TestEnum.values(as_list = False), [1,2,3])
         self.assertEqual(list(TestEnum.values(as_list = False)), [1,2,3])
 
+    def test_get_with_mapping(self):
+        class TestEnum(EnumWithDict):
+            VALUE_1 = 1
+            VALUE_2 = 2
+            VALUE_3 = 3
+
+        custom_mapping = {
+            'VALUE_1': 'Mapped 1',
+            'VALUE_2': 'Mapped 2',
+            'VALUE_3': 'Mapped 3'
+        }
+
+        # Test getting a value from custom mapping
+        self.assertEqual(TestEnum.get('VALUE_1', mapping=custom_mapping), 'Mapped 1')
+
+        # Test getting a value without custom mapping
+        self.assertEqual(TestEnum.get('VALUE_3'), 3)
+
+        # Test getting a value with a default specified, when the key is not in the custom mapping or enum
+        self.assertEqual(TestEnum.get('VALUE_4', default='Default', mapping=custom_mapping), 'Default')
+
+        # Test getting a value without a default specified, when the key is not in the custom mapping or enum
+        # It should fall back to the initial value of the enum
+        self.assertEqual(TestEnum.get('VALUE_4', mapping=custom_mapping), 1)  # Initial value
+
+        # Validation should fail because of incomplete mapping
+        with self.assertRaises(KeyError) as context:
+            TestEnum.get('VALUE_2', mapping={
+                'VALUE_2': 'Mapped 2',
+            })
+
+        # Validation should fail because of empty mapping
+        with self.assertRaises(KeyError) as context:
+            TestEnum.get('VALUE_2', mapping={})
+
+        # Validation should fail because of empty mapping
+        with self.assertRaises(KeyError) as context:
+            invalid_custom_mapping = custom_mapping
+            invalid_custom_mapping['VALUE_4'] = 'Mapped 4'
+
+            TestEnum.get('VALUE_2', mapping=invalid_custom_mapping)
+
+
 if __name__ == '__main__':
     unittest.main()
```

