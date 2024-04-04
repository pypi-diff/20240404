# Comparing `tmp/enum_with_dict-0.5.3.tar.gz` & `tmp/enum_with_dict-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.5.3.tar", last modified: Thu Apr  4 00:01:23 2024, max compression
+gzip compressed data, was "enum_with_dict-0.6.0.tar", last modified: Thu Apr  4 00:11:47 2024, max compression
```

## Comparing `enum_with_dict-0.5.3.tar` & `enum_with_dict-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.902319 enum_with_dict-0.5.3/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.5.3/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:01:23.902065 enum_with_dict-0.5.3/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4041 2024-04-03 23:58:28.000000 enum_with_dict-0.5.3/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.900256 enum_with_dict-0.5.3/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.5.3/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     4878 2024-04-03 23:58:58.000000 enum_with_dict-0.5.3/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.901139 enum_with_dict-0.5.3/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 00:01:23.902367 enum_with_dict-0.5.3/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 00:00:32.000000 enum_with_dict-0.5.3/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.901467 enum_with_dict-0.5.3/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.5.3/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5829 2024-04-03 23:50:18.000000 enum_with_dict-0.5.3/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.820879 enum_with_dict-0.6.0/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.6.0/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:11:47.820603 enum_with_dict-0.6.0/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4041 2024-04-03 23:58:28.000000 enum_with_dict-0.6.0/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.819461 enum_with_dict-0.6.0/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.6.0/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5177 2024-04-04 00:11:41.000000 enum_with_dict-0.6.0/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.820024 enum_with_dict-0.6.0/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 00:11:47.000000 enum_with_dict-0.6.0/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 00:11:47.820923 enum_with_dict-0.6.0/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 00:11:41.000000 enum_with_dict-0.6.0/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:11:47.820249 enum_with_dict-0.6.0/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.6.0/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5825 2024-04-04 00:11:41.000000 enum_with_dict-0.6.0/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.5.3/LICENSE` & `enum_with_dict-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.5.3/PKG-INFO` & `enum_with_dict-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.5.3
+Version: 0.6.0
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py_enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `enum_with_dict-0.5.3/README.md` & `enum_with_dict-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.5.3/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.6.0/enum_with_dict/enum_with_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,28 +73,38 @@
         if as_list:
             return list(values_view)
         else:
             return values_view
 
     @classmethod
     def validate_mapping_keys(cls, mapping: Dict[str, Any]) -> bool:
-        """Validate that every enum member has a mapping, raise error if any are missing."""
+        """Validate that every enum member has a mapping, raising a KeyError if any are missing.
+        
+        Args:
+            mapping (Dict[str, Any]): The mapping dictionary to validate.
+
+        Returns:
+            bool: True if the mapping is valid (raises `KeyError` otherwise).
+
+        Raises:
+            KeyError: If any enum members are missing in the provided mapping.
+        """
         # Check if the names of enum members are in the mapping's keys
         missing = [member.name for member in cls if member.name not in mapping]
         if missing:
             # missing now contains the names of the enum members that are not keys in the mapping
             missing_keys = ', '.join(missing)  # Joining missing member names directly
-            raise ValueError(f"Missing mappings for: {missing_keys}")
+            raise KeyError(f"Missing mappings for: {missing_keys}")
         
         # Check for extra keys in the mapping
         extra_keys = [key for key in mapping if key not in {member.name for member in cls}]
         if extra_keys:
             # extra_keys now contains the extra keys found in the mapping
             extra_keys_str = ', '.join(extra_keys)  # Joining extra keys for the error message
-            raise ValueError(f"Extra keys found in mapping: {extra_keys_str}")
+            raise KeyError(f"Extra keys found in mapping: {extra_keys_str}")
         
         return True
 
     @classmethod
     def map(cls, key_mapping: Dict[Enum, Any]) -> Dict[Enum, Any]:
         """Map enum members to values using the provided dictionary.
 
@@ -105,15 +115,15 @@
         Args:
             key_mapping (Dict[Enum, Any]): A dictionary mapping enum members to new values.
 
         Returns:
             Dict[Enum, Any]: A dictionary containing the mapped enum members with their corresponding new values.
 
         Raises:
-            ValueError: If any enum members are missing in the provided mapping.
+            KeyError: If any enum members are missing in the provided mapping.
         """
         # Validate the new mapping
         cls.validate_mapping_keys({**cls.to_dict(), **{member.name: value for member, value in key_mapping.items()}})
         
         # Map enum members to values
         mapped_values = {}
         for member in cls:
```

### Comparing `enum_with_dict-0.5.3/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.6.0/enum_with_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.5.3
+Version: 0.6.0
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/py_enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `enum_with_dict-0.5.3/setup.py` & `enum_with_dict-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.5.3',
+    version='0.6.0',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/py_enum_with_dict',
```

### Comparing `enum_with_dict-0.5.3/test/test_enum_with_dict.py` & `enum_with_dict-0.6.0/test/test_enum_with_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             C = 3  # C is not included in the mapping, should trigger validation failure
 
         incomplete_mapping = {
             'A': 1,
             'B': 2,
         }
 
-        with self.assertRaises(ValueError):
+        with self.assertRaises(KeyError):
             IncompleteEnum.validate_mapping_keys(incomplete_mapping)
 
     def test_validate_mapping_keys_extended(self):
         """Test validation fails with an extended mapping."""
 
         class ExtendEnum(EnumWithDict):
             A = 1
@@ -78,15 +78,15 @@
 
         dict_mapping = ExtendEnum.to_dict()
 
         # Add a new value that doesn't correspond to any enum member
         dict_mapping['UNDEFINED'] = 'undefined'
 
         # Now, validation should fail because of the extra key
-        with self.assertRaises(ValueError) as context:
+        with self.assertRaises(KeyError) as context:
             ExtendEnum.validate_mapping_keys(dict_mapping)
 
     def test_validate_self_mapping(self):
         """Test validation succeeds against self."""
 
         class Mixed(EnumWithDict):
             NUMBER = 1,
```

