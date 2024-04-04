# Comparing `tmp/faker-commerce-1.0.3.tar.gz` & `tmp/faker-commerce-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-faker-commerce/python-faker-commerce/dist/tmpv2pazja7/faker-commerce-1.0.3.tar", last modified: Thu Nov 26 01:03:16 2020, max compression
+gzip compressed data, was "/home/runner/work/python-faker-commerce/python-faker-commerce/dist/tmppe_arq12/faker-commerce-1.0.4.tar", last modified: Thu Apr  4 10:34:37 2024, max compression
```

## Comparing `faker-commerce-1.0.3.tar` & `faker-commerce-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-26 01:03:16.000000 faker-commerce-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (116)       30 2020-11-26 01:03:09.000000 faker-commerce-1.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-26 01:03:16.000000 faker-commerce-1.0.3/faker_commerce/
--rw-r--r--   0 runner    (1001) docker     (116)     2378 2020-11-26 01:03:09.000000 faker-commerce-1.0.3/faker_commerce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      686 2020-11-26 01:03:09.000000 faker-commerce-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-26 01:03:16.000000 faker-commerce-1.0.3/faker_commerce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-11-26 01:03:15.000000 faker-commerce-1.0.3/faker_commerce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-26 01:03:15.000000 faker-commerce-1.0.3/faker_commerce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      249 2020-11-26 01:03:16.000000 faker-commerce-1.0.3/faker_commerce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2020-11-26 01:03:15.000000 faker-commerce-1.0.3/faker_commerce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      758 2020-11-26 01:03:15.000000 faker-commerce-1.0.3/faker_commerce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-26 01:03:16.000000 faker-commerce-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1199 2020-11-26 01:03:09.000000 faker-commerce-1.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      758 2020-11-26 01:03:16.000000 faker-commerce-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 10:34:25.000000 faker-commerce-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/faker_commerce/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-04 10:34:25.000000 faker-commerce-1.0.4/faker_commerce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 10:34:25.000000 faker-commerce-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 10:34:25.000000 faker-commerce-1.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/faker_commerce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/faker_commerce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/faker_commerce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/faker_commerce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/faker_commerce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/faker_commerce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 10:34:25.000000 faker-commerce-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 10:34:37.000000 faker-commerce-1.0.4/PKG-INFO
```

### Comparing `faker-commerce-1.0.3/faker_commerce/__init__.py` & `faker-commerce-1.0.4/faker_commerce/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Provider for Faker which adds fake microservice names."""
 
 import random
+from typing import Union, List, Dict
 
-import faker.providers
+from faker.providers import BaseProvider
 
-CATEGORIES = [
+CATEGORIES: List = [
   "Books",
   "Movies",
   "Music",
   "Games",
   "Electronics",
   "Computers",
   "Home",
@@ -25,28 +25,30 @@
   "Jewelery",
   "Sports",
   "Outdoors",
   "Automotive",
   "Industrial"
 ]
 
-PRODUCT_DATA = {
-    'material': [
-        "Steel",
-        "Wooden",
-        "Concrete",
-        "Plastic",
-        "Cotton",
-        "Granite",
-        "Rubber",
-        "Metal",
-        "Soft",
-        "Fresh",
-        "Frozen"
-    ],
+MATERIALS: List = [
+  "Steel",
+  "Wooden",
+  "Concrete",
+  "Plastic",
+  "Cotton",
+  "Granite",
+  "Rubber",
+  "Metal",
+  "Soft",
+  "Fresh",
+  "Frozen"
+]
+
+PRODUCT_DATA: Dict[str, List] = {
+    'material': MATERIALS,
     'product': [
         "Chair",
         "Car",
         "Computer",
         "Keyboard",
         "Mouse",
         "Bike",
@@ -91,18 +93,18 @@
         "Gently Used",
         "Used",
         "For repair"
     ]
 }
 
 
-class Provider(faker.providers.BaseProvider):
-    """Provider for Faker which adds fake microservice names."""
+class Provider(BaseProvider):
+    """Provider for Faker which adds fake ecommerce product information."""
 
-    def ecommerce_name(self):
+    def ecommerce_name(self) -> str:
         """Fake product names."""
         product = self.random_element(PRODUCT_DATA['product'])
         adjective = self.random_element(PRODUCT_DATA['adjective'])
         material = self.random_element(PRODUCT_DATA['material'])
 
         choices = [
             product,
@@ -110,13 +112,16 @@
             " ".join([material, product]),
             " ".join([adjective, material, product]),
         ]
 
         names = random.choices(choices, k=1)
         return names[0]
 
-    def ecommerce_category(self):
+    def ecommerce_material(self) -> str:
+        return self.random_element(MATERIALS)
+
+    def ecommerce_category(self) -> str:
         return self.random_element(CATEGORIES)
 
-    def ecommerce_price(self, as_int: bool = True):
+    def ecommerce_price(self, as_int: bool = True) -> Union[int, float]:
         n = self.random_int(min=100, max=99999999)
         return round(n, 2) if as_int else n / 100
```

### Comparing `faker-commerce-1.0.3/README.md` & `faker-commerce-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `faker-commerce-1.0.3/faker_commerce.egg-info/PKG-INFO` & `faker-commerce-1.0.4/faker_commerce.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: faker-commerce
-Version: 1.0.3
+Version: 1.0.4
 Summary: Provider for Faker which adds fake commerce product names, prices, categories and descriptions.
 Home-page: https://github.com/nicobritos/python-faker-commerce
 Author: Nicolas Ignacio Britos
 Author-email: nicbritos@hotmail.com
 License: UNKNOWN
-Description: Provider for [Faker](https://faker.readthedocs.io/) which adds fake commerce product names, prices, categories and descriptions.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Provider for [Faker](https://faker.readthedocs.io/) which adds fake commerce product names, prices, categories and descriptions.
+
```

### Comparing `faker-commerce-1.0.3/setup.py` & `faker-commerce-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = (
         "Provider for [Faker](https://faker.readthedocs.io/) which adds fake "
         "commerce product names, prices, categories and descriptions."
     )
 
 setuptools.setup(
     name="faker-commerce",
-    version="1.0.3",
+    version="1.0.4",
     author="Nicolas Ignacio Britos",
     author_email="nicbritos@hotmail.com",
     description="Provider for Faker which adds fake commerce product names, prices, categories and descriptions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nicobritos/python-faker-commerce",
     packages=setuptools.find_packages(),
```

### Comparing `faker-commerce-1.0.3/PKG-INFO` & `faker-commerce-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: faker-commerce
-Version: 1.0.3
+Version: 1.0.4
 Summary: Provider for Faker which adds fake commerce product names, prices, categories and descriptions.
 Home-page: https://github.com/nicobritos/python-faker-commerce
 Author: Nicolas Ignacio Britos
 Author-email: nicbritos@hotmail.com
 License: UNKNOWN
-Description: Provider for [Faker](https://faker.readthedocs.io/) which adds fake commerce product names, prices, categories and descriptions.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Provider for [Faker](https://faker.readthedocs.io/) which adds fake commerce product names, prices, categories and descriptions.
+
```

