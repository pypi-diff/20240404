# Comparing `tmp/enum_with_dict-0.7.0.tar.gz` & `tmp/enum_with_dict-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.7.0.tar", last modified: Thu Apr  4 10:45:41 2024, max compression
+gzip compressed data, was "enum_with_dict-0.7.1.tar", last modified: Thu Apr  4 11:07:21 2024, max compression
```

## Comparing `enum_with_dict-0.7.0.tar` & `enum_with_dict-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.104351 enum_with_dict-0.7.0/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.7.0/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 10:45:41.104143 enum_with_dict-0.7.0/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4675 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.103036 enum_with_dict-0.7.0/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.7.0/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     6048 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.103602 enum_with_dict-0.7.0/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 10:45:41.000000 enum_with_dict-0.7.0/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 10:45:41.104391 enum_with_dict-0.7.0/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 10:45:41.103816 enum_with_dict-0.7.0/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.7.0/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     8006 2024-04-04 10:45:17.000000 enum_with_dict-0.7.0/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.927370 enum_with_dict-0.7.1/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.7.1/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 11:07:21.927124 enum_with_dict-0.7.1/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4675 2024-04-04 10:45:17.000000 enum_with_dict-0.7.1/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.926004 enum_with_dict-0.7.1/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.7.1/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     6533 2024-04-04 11:07:13.000000 enum_with_dict-0.7.1/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.926570 enum_with_dict-0.7.1/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     5589 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 11:07:21.000000 enum_with_dict-0.7.1/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 11:07:21.927416 enum_with_dict-0.7.1/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 11:07:13.000000 enum_with_dict-0.7.1/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 11:07:21.926794 enum_with_dict-0.7.1/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.7.1/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     8057 2024-04-04 11:07:13.000000 enum_with_dict-0.7.1/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.7.0/LICENSE` & `enum_with_dict-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.7.0/PKG-INFO` & `enum_with_dict-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.7.0
+Version: 0.7.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py-enum-with-dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `enum_with_dict-0.7.0/README.md` & `enum_with_dict-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.7.0/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.7.1/enum_with_dict/enum_with_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,29 @@
 
 
 class EnumWithDict(Enum):
     @classmethod
     def to_dict(cls) -> Dict[str, Any]:
         """Return a dictionary representation of the enum."""
         return {member.name: member.value for member in cls}
+    
+    @classmethod
+    def get_initial_key(cls) -> Any:
+        """Get the first key from the enum dictionary."""
+        return next(iter(cls.to_dict().keys()))
 
     @classmethod
-    def get_initial(cls) -> Any:
+    def get_initial_value(cls) -> Any:
         """Get the first value from the enum dictionary."""
         return next(iter(cls.to_dict().values()))
+    
+    @classmethod
+    def get_initial(cls) -> Any:
+        """Alias to `get_initial_value`."""
+        return cls.get_initial_value()
 
     @classmethod
     def get(cls, key: str, default: Any = None, mapping: Dict[str, Any] = None) -> Any:
         """
         Get the value for the given key from the optional mapping or the enum,
         return default or initial value if not found.
         
@@ -26,24 +36,29 @@
             mapping (Dict[str, Any], optional): An optional mapping of keys to custom values.
         
         Returns:
             Any: The value associated with the key, either from the mapping or the enum's default values.
         """
         # Use the initial value as the default if no default is provided
         if default is None:
-            default = cls.get_initial()
+            default_key = cls.get_initial_key()
+
+            if mapping is not None:
+                default = mapping[default_key]
+            else:
+                default = cls.to_dict()[default_key]
         
         # If a mapping is provided, try to get the value from it
         if mapping is not None:
             cls.validate_mapping_keys(mapping)
 
             return mapping.get(key, default)
-        
-        # Fallback to the enum's default values if no mapping is provided or the key is not in the mapping
-        return cls.to_dict().get(key, default)
+        else:
+            # Fallback to the enum's default values if no mapping is provided or the key is not in the mapping
+            return cls.to_dict().get(key, default)
     
     @classmethod
     def keys(cls, as_list = True) -> Union[List[str], KeysView[str]]:
         """
         Return a view of the keys of the enum class as a list or as a `KeysView`.
 
         Parameters:
```

### Comparing `enum_with_dict-0.7.0/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.7.1/enum_with_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.7.0
+Version: 0.7.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py-enum-with-dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `enum_with_dict-0.7.0/setup.py` & `enum_with_dict-0.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.7.0',
+    version='0.7.1',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/py-enum-with-dict',
```

### Comparing `enum_with_dict-0.7.0/test/test_enum_with_dict.py` & `enum_with_dict-0.7.1/test/test_enum_with_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,17 +195,17 @@
 
         # Test getting a value without custom mapping
         self.assertEqual(TestEnum.get('VALUE_3'), 3)
 
         # Test getting a value with a default specified, when the key is not in the custom mapping or enum
         self.assertEqual(TestEnum.get('VALUE_4', default='Default', mapping=custom_mapping), 'Default')
 
-        # Test getting a value without a default specified, when the key is not in the custom mapping or enum
-        # It should fall back to the initial value of the enum
-        self.assertEqual(TestEnum.get('VALUE_4', mapping=custom_mapping), 1)  # Initial value
+        # Test getting a mapped value without a default specified, when the key is not in the custom mapping or enum
+        # It should fall back to the custom mapping value with the initial key of the enum
+        self.assertEqual(TestEnum.get('VALUE_4', mapping=custom_mapping), 'Mapped 1')  # Initial mapped value
 
         # Validation should fail because of incomplete mapping
         with self.assertRaises(KeyError) as context:
             TestEnum.get('VALUE_2', mapping={
                 'VALUE_2': 'Mapped 2',
             })
```

