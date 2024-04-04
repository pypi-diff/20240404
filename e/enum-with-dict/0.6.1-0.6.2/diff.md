# Comparing `tmp/enum_with_dict-0.6.1.tar.gz` & `tmp/enum_with_dict-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.6.1.tar", last modified: Thu Apr  4 03:55:00 2024, max compression
+gzip compressed data, was "enum_with_dict-0.6.2.tar", last modified: Thu Apr  4 04:19:12 2024, max compression
```

## Comparing `enum_with_dict-0.6.1.tar` & `enum_with_dict-0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.035317 enum_with_dict-0.6.1/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.6.1/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 03:55:00.035043 enum_with_dict-0.6.1/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4114 2024-04-04 00:26:57.000000 enum_with_dict-0.6.1/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.033413 enum_with_dict-0.6.1/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.6.1/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5177 2024-04-04 00:11:41.000000 enum_with_dict-0.6.1/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.034260 enum_with_dict-0.6.1/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 03:55:00.000000 enum_with_dict-0.6.1/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 03:55:00.035371 enum_with_dict-0.6.1/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 03:54:58.000000 enum_with_dict-0.6.1/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 03:55:00.034573 enum_with_dict-0.6.1/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.6.1/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5819 2024-04-04 03:54:58.000000 enum_with_dict-0.6.1/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.579190 enum_with_dict-0.6.2/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.6.2/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 04:19:12.578939 enum_with_dict-0.6.2/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4114 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.577849 enum_with_dict-0.6.2/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.6.2/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5144 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.578349 enum_with_dict-0.6.2/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     5028 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 04:19:12.000000 enum_with_dict-0.6.2/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 04:19:12.579234 enum_with_dict-0.6.2/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 04:19:12.578585 enum_with_dict-0.6.2/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.6.2/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     6320 2024-04-04 04:19:06.000000 enum_with_dict-0.6.2/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.6.1/LICENSE` & `enum_with_dict-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.6.1/PKG-INFO` & `enum_with_dict-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.6.1
+Version: 0.6.2
 Summary: Enum with to_dict method.
-Home-page: https://github.com/jzombie/py_enum_with_dict
+Home-page: https://github.com/jzombie/py-enum-with-dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -37,15 +37,15 @@
 - **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
-pip install enum_with_dict
+pip install enum-with-dict
 ```
 
 ## Usage
 
 ### Defining an Enum with `EnumWithDict`
 
 ```python
```

### Comparing `enum_with_dict-0.6.1/README.md` & `enum_with_dict-0.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
-pip install enum_with_dict
+pip install enum-with-dict
 ```
 
 ## Usage
 
 ### Defining an Enum with `EnumWithDict`
 
 ```python
```

### Comparing `enum_with_dict-0.6.1/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.6.2/enum_with_dict/enum_with_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,18 @@
 
         Returns:
             Dict[Enum, Any]: A dictionary containing the mapped enum members with their corresponding new values.
 
         Raises:
             KeyError: If any enum members are missing in the provided mapping.
         """
-        # Validate the new mapping
-        cls.validate_mapping_keys({**cls.to_dict(), **{member.name: value for member, value in key_mapping.items()}})
-        
+       
         # Map enum members to values
         mapped_values = {}
         for member in cls:
             if member in key_mapping:
                 mapped_values[member.name] = key_mapping[member]
+
+        # Validate the provided key mapping contains all enum members
+        cls.validate_mapping_keys(mapped_values)
+
         return mapped_values
```

### Comparing `enum_with_dict-0.6.1/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.6.2/enum_with_dict.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.6.1
+Version: 0.6.2
 Summary: Enum with to_dict method.
-Home-page: https://github.com/jzombie/py_enum_with_dict
+Home-page: https://github.com/jzombie/py-enum-with-dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -37,15 +37,15 @@
 - **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
-pip install enum_with_dict
+pip install enum-with-dict
 ```
 
 ## Usage
 
 ### Defining an Enum with `EnumWithDict`
 
 ```python
```

### Comparing `enum_with_dict-0.6.1/setup.py` & `enum_with_dict-0.6.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.6.1',
+    version='0.6.2',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/jzombie/py_enum_with_dict',
+    url='https://github.com/jzombie/py-enum-with-dict',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `enum_with_dict-0.6.1/test/test_enum_with_dict.py` & `enum_with_dict-0.6.2/test/test_enum_with_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,32 @@
         key_mapping = {
             TestEnum.VALUE_1: "some_new_value",
             TestEnum.VALUE_2: "another_new_value",
             TestEnum.VALUE_3.value: "a new value"
         }
 
         # Perform the mapping and validate
-        with self.assertRaises(AttributeError):
+        with self.assertRaises(KeyError):
+            TestEnum.map(key_mapping)
+
+    def test_incomplete_map(self):
+        """Test incomplete mapping enum members to values."""
+        class TestEnum(EnumWithDict):
+            VALUE_1 = 1
+            VALUE_2 = 2
+            VALUE_3 = 3
+        
+        # Define the key mapping
+        key_mapping = {
+            TestEnum.VALUE_1: "some_new_value",
+            TestEnum.VALUE_2: "another_new_value",
+        }
+
+        # Perform the mapping and validate
+        with self.assertRaises(KeyError):
             TestEnum.map(key_mapping)
 
     def test_keys_retrieval(self):
         class TestEnum(EnumWithDict):
             VALUE_1 = 1
             VALUE_2 = 2
             VALUE_3 = 3
```

