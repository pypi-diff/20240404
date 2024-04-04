# Comparing `tmp/enum_with_dict-0.5.2.tar.gz` & `tmp/enum_with_dict-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.5.2.tar", last modified: Wed Apr  3 23:59:30 2024, max compression
+gzip compressed data, was "enum_with_dict-0.5.3.tar", last modified: Thu Apr  4 00:01:23 2024, max compression
```

## Comparing `enum_with_dict-0.5.2.tar` & `enum_with_dict-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.788669 enum_with_dict-0.5.2/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.5.2/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     4952 2024-04-03 23:59:30.788399 enum_with_dict-0.5.2/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     4041 2024-04-03 23:58:28.000000 enum_with_dict-0.5.2/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.787097 enum_with_dict-0.5.2/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.5.2/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     4878 2024-04-03 23:58:58.000000 enum_with_dict-0.5.2/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.787652 enum_with_dict-0.5.2/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     4952 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 23:59:30.000000 enum_with_dict-0.5.2/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 23:59:30.788714 enum_with_dict-0.5.2/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 23:59:05.000000 enum_with_dict-0.5.2/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 23:59:30.787876 enum_with_dict-0.5.2/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.5.2/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5829 2024-04-03 23:50:18.000000 enum_with_dict-0.5.2/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.902319 enum_with_dict-0.5.3/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.5.3/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:01:23.902065 enum_with_dict-0.5.3/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     4041 2024-04-03 23:58:28.000000 enum_with_dict-0.5.3/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.900256 enum_with_dict-0.5.3/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.5.3/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     4878 2024-04-03 23:58:58.000000 enum_with_dict-0.5.3/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.901139 enum_with_dict-0.5.3/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     4955 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-04 00:01:23.000000 enum_with_dict-0.5.3/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-04 00:01:23.902367 enum_with_dict-0.5.3/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1077 2024-04-04 00:00:32.000000 enum_with_dict-0.5.3/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-04 00:01:23.901467 enum_with_dict-0.5.3/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.5.3/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5829 2024-04-03 23:50:18.000000 enum_with_dict-0.5.3/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.5.2/LICENSE` & `enum_with_dict-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.5.2/PKG-INFO` & `enum_with_dict-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.5.2
+Version: 0.5.3
 Summary: Enum with to_dict method.
-Home-page: https://github.com/jzombie/enum_with_dict
+Home-page: https://github.com/jzombie/py_enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `enum_with_dict-0.5.2/README.md` & `enum_with_dict-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.5.2/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.5.3/enum_with_dict/enum_with_dict.py`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.5.2/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.5.3/enum_with_dict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.5.2
+Version: 0.5.3
 Summary: Enum with to_dict method.
-Home-page: https://github.com/jzombie/enum_with_dict
+Home-page: https://github.com/jzombie/py_enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `enum_with_dict-0.5.2/setup.py` & `enum_with_dict-0.5.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.5.2',
+    version='0.5.3',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/jzombie/enum_with_dict',
+    url='https://github.com/jzombie/py_enum_with_dict',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `enum_with_dict-0.5.2/test/test_enum_with_dict.py` & `enum_with_dict-0.5.3/test/test_enum_with_dict.py`

 * *Files identical despite different names*

