# Comparing `tmp/sysyphus-0.1.1.tar.gz` & `tmp/sysyphus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysyphus-0.1.1.tar", last modified: Sun Mar 31 13:43:42 2024, max compression
+gzip compressed data, was "sysyphus-0.1.2.tar", last modified: Thu Apr  4 17:04:52 2024, max compression
```

## Comparing `sysyphus-0.1.1.tar` & `sysyphus-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-03-31 13:43:42.714037 sysyphus-0.1.1/
--rw-r--r--   0 psemp      (501) staff       (20)     1073 2024-02-29 12:29:58.000000 sysyphus-0.1.1/LICENSE
--rw-r--r--   0 psemp      (501) staff       (20)     8210 2024-03-31 13:43:42.713655 sysyphus-0.1.1/PKG-INFO
--rw-r--r--   0 psemp      (501) staff       (20)     7545 2024-03-30 15:46:30.000000 sysyphus-0.1.1/README.md
--rw-r--r--   0 psemp      (501) staff       (20)       38 2024-03-31 13:43:42.714081 sysyphus-0.1.1/setup.cfg
--rw-r--r--   0 psemp      (501) staff       (20)      836 2024-03-31 13:42:50.000000 sysyphus-0.1.1/setup.py
-drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-03-31 13:43:42.701892 sysyphus-0.1.1/sysyphus/
--rw-r--r--   0 psemp      (501) staff       (20)       83 2024-03-17 09:13:45.000000 sysyphus-0.1.1/sysyphus/__init__.py
-drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-03-31 13:43:42.706663 sysyphus-0.1.1/sysyphus/models/
--rw-r--r--   0 psemp      (501) staff       (20)        0 2024-03-11 22:40:07.000000 sysyphus-0.1.1/sysyphus/models/__init__.py
--rw-r--r--   0 psemp      (501) staff       (20)    11974 2024-03-30 15:46:30.000000 sysyphus-0.1.1/sysyphus/models/boulder.py
--rw-r--r--   0 psemp      (501) staff       (20)     5398 2024-03-30 15:46:30.000000 sysyphus-0.1.1/sysyphus/models/meteorite.py
-drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-03-31 13:43:42.710225 sysyphus-0.1.1/sysyphus/scripts/
--rw-r--r--   0 psemp      (501) staff       (20)        0 2024-03-11 22:40:07.000000 sysyphus-0.1.1/sysyphus/scripts/__init__.py
--rw-r--r--   0 psemp      (501) staff       (20)     2812 2024-03-16 13:58:12.000000 sysyphus-0.1.1/sysyphus/scripts/preprocessing.py
--rw-r--r--   0 psemp      (501) staff       (20)     1339 2024-03-16 13:36:27.000000 sysyphus-0.1.1/sysyphus/scripts/remote_load.py
--rw-r--r--   0 psemp      (501) staff       (20)     2229 2024-03-31 13:14:27.000000 sysyphus-0.1.1/sysyphus/scripts/rendering.py
--rw-r--r--   0 psemp      (501) staff       (20)     6945 2024-03-31 13:42:13.000000 sysyphus-0.1.1/sysyphus/scripts/search.py
--rw-r--r--   0 psemp      (501) staff       (20)     2212 2024-03-16 13:35:41.000000 sysyphus-0.1.1/sysyphus/scripts/user_requests.py
-drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-03-31 13:43:42.713287 sysyphus-0.1.1/sysyphus.egg-info/
--rw-r--r--   0 psemp      (501) staff       (20)     8210 2024-03-31 13:43:42.000000 sysyphus-0.1.1/sysyphus.egg-info/PKG-INFO
--rw-r--r--   0 psemp      (501) staff       (20)      649 2024-03-31 13:43:42.000000 sysyphus-0.1.1/sysyphus.egg-info/SOURCES.txt
--rw-r--r--   0 psemp      (501) staff       (20)        1 2024-03-31 13:43:42.000000 sysyphus-0.1.1/sysyphus.egg-info/dependency_links.txt
--rw-r--r--   0 psemp      (501) staff       (20)       42 2024-03-31 13:43:42.000000 sysyphus-0.1.1/sysyphus.egg-info/requires.txt
--rw-r--r--   0 psemp      (501) staff       (20)        9 2024-03-31 13:43:42.000000 sysyphus-0.1.1/sysyphus.egg-info/top_level.txt
-drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-03-31 13:43:42.712934 sysyphus-0.1.1/tests/
--rw-r--r--   0 psemp      (501) staff       (20)     1040 2024-03-16 18:49:48.000000 sysyphus-0.1.1/tests/test_boulder.py
--rw-r--r--   0 psemp      (501) staff       (20)     1091 2024-03-16 14:17:00.000000 sysyphus-0.1.1/tests/test_meteorite.py
--rw-r--r--   0 psemp      (501) staff       (20)     1329 2024-03-16 14:00:17.000000 sysyphus-0.1.1/tests/test_preprocessing.py
--rw-r--r--   0 psemp      (501) staff       (20)      983 2024-03-16 14:14:03.000000 sysyphus-0.1.1/tests/test_remote_load.py
--rw-r--r--   0 psemp      (501) staff       (20)     1415 2024-03-16 14:42:11.000000 sysyphus-0.1.1/tests/test_rendering.py
--rw-r--r--   0 psemp      (501) staff       (20)     4427 2024-03-30 15:46:30.000000 sysyphus-0.1.1/tests/test_search.py
--rw-r--r--   0 psemp      (501) staff       (20)     2512 2024-03-16 14:12:16.000000 sysyphus-0.1.1/tests/test_user_requests.py
+drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-04-04 17:04:52.549915 sysyphus-0.1.2/
+-rw-r--r--   0 psemp      (501) staff       (20)     1073 2024-02-29 12:29:58.000000 sysyphus-0.1.2/LICENSE
+-rw-r--r--   0 psemp      (501) staff       (20)     8256 2024-04-04 17:04:52.549469 sysyphus-0.1.2/PKG-INFO
+-rw-r--r--   0 psemp      (501) staff       (20)     7591 2024-04-01 10:38:57.000000 sysyphus-0.1.2/README.md
+-rw-r--r--   0 psemp      (501) staff       (20)       38 2024-04-04 17:04:52.549961 sysyphus-0.1.2/setup.cfg
+-rw-r--r--   0 psemp      (501) staff       (20)      836 2024-04-04 17:04:26.000000 sysyphus-0.1.2/setup.py
+drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-04-04 17:04:52.537710 sysyphus-0.1.2/sysyphus/
+-rw-r--r--   0 psemp      (501) staff       (20)       83 2024-03-17 09:13:45.000000 sysyphus-0.1.2/sysyphus/__init__.py
+drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-04-04 17:04:52.541544 sysyphus-0.1.2/sysyphus/models/
+-rw-r--r--   0 psemp      (501) staff       (20)        0 2024-03-11 22:40:07.000000 sysyphus-0.1.2/sysyphus/models/__init__.py
+-rw-r--r--   0 psemp      (501) staff       (20)    12112 2024-04-04 17:03:16.000000 sysyphus-0.1.2/sysyphus/models/boulder.py
+-rw-r--r--   0 psemp      (501) staff       (20)     5398 2024-03-30 15:46:30.000000 sysyphus-0.1.2/sysyphus/models/meteorite.py
+drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-04-04 17:04:52.544625 sysyphus-0.1.2/sysyphus/scripts/
+-rw-r--r--   0 psemp      (501) staff       (20)        0 2024-03-11 22:40:07.000000 sysyphus-0.1.2/sysyphus/scripts/__init__.py
+-rw-r--r--   0 psemp      (501) staff       (20)     3487 2024-04-04 17:03:16.000000 sysyphus-0.1.2/sysyphus/scripts/preprocessing.py
+-rw-r--r--   0 psemp      (501) staff       (20)     1339 2024-03-16 13:36:27.000000 sysyphus-0.1.2/sysyphus/scripts/remote_load.py
+-rw-r--r--   0 psemp      (501) staff       (20)     2229 2024-03-31 13:14:27.000000 sysyphus-0.1.2/sysyphus/scripts/rendering.py
+-rw-r--r--   0 psemp      (501) staff       (20)     7035 2024-04-01 09:27:58.000000 sysyphus-0.1.2/sysyphus/scripts/search.py
+-rw-r--r--   0 psemp      (501) staff       (20)     2212 2024-04-04 16:48:42.000000 sysyphus-0.1.2/sysyphus/scripts/user_requests.py
+drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-04-04 17:04:52.549086 sysyphus-0.1.2/sysyphus.egg-info/
+-rw-r--r--   0 psemp      (501) staff       (20)     8256 2024-04-04 17:04:52.000000 sysyphus-0.1.2/sysyphus.egg-info/PKG-INFO
+-rw-r--r--   0 psemp      (501) staff       (20)      649 2024-04-04 17:04:52.000000 sysyphus-0.1.2/sysyphus.egg-info/SOURCES.txt
+-rw-r--r--   0 psemp      (501) staff       (20)        1 2024-04-04 17:04:52.000000 sysyphus-0.1.2/sysyphus.egg-info/dependency_links.txt
+-rw-r--r--   0 psemp      (501) staff       (20)       42 2024-04-04 17:04:52.000000 sysyphus-0.1.2/sysyphus.egg-info/requires.txt
+-rw-r--r--   0 psemp      (501) staff       (20)        9 2024-04-04 17:04:52.000000 sysyphus-0.1.2/sysyphus.egg-info/top_level.txt
+drwxr-xr-x   0 psemp      (501) staff       (20)        0 2024-04-04 17:04:52.548497 sysyphus-0.1.2/tests/
+-rw-r--r--   0 psemp      (501) staff       (20)     1040 2024-03-16 18:49:48.000000 sysyphus-0.1.2/tests/test_boulder.py
+-rw-r--r--   0 psemp      (501) staff       (20)     1091 2024-03-16 14:17:00.000000 sysyphus-0.1.2/tests/test_meteorite.py
+-rw-r--r--   0 psemp      (501) staff       (20)     1329 2024-03-16 14:00:17.000000 sysyphus-0.1.2/tests/test_preprocessing.py
+-rw-r--r--   0 psemp      (501) staff       (20)      983 2024-03-16 14:14:03.000000 sysyphus-0.1.2/tests/test_remote_load.py
+-rw-r--r--   0 psemp      (501) staff       (20)     1415 2024-03-16 14:42:11.000000 sysyphus-0.1.2/tests/test_rendering.py
+-rw-r--r--   0 psemp      (501) staff       (20)     4427 2024-03-30 15:46:30.000000 sysyphus-0.1.2/tests/test_search.py
+-rw-r--r--   0 psemp      (501) staff       (20)     2512 2024-03-16 14:12:16.000000 sysyphus-0.1.2/tests/test_user_requests.py
```

### Comparing `sysyphus-0.1.1/LICENSE` & `sysyphus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/PKG-INFO` & `sysyphus-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysyphus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Structured meteorite data access using MetBull: Query, filter, and analyze with ease.
 Home-page: https://github.com/Psemp/sysyphus.git
 Author: Pierre Sempéré
 Author-email: pierre.sempere.01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -115,15 +115,15 @@
 format = "csv"
 
 boulder.save_search(filepath=file_name, file_format=format)
 >>> file saved as csv at met_search  # extension added
 ```
 
 ## Advanced Features
-*Cf. Notebook that i'll try not to forget and link here*
+[Example notebook link](https://github.com/Psemp/sysyphus/blob/main/notebooks/sysyphus_examples.ipynb)
 
 ## Credits
 
 Sysyphus is made possible thanks to the data provided by MetBull and the contributions from our community. <br>I appreciate every piece of input, code, or feedback I've received.
 
 I am especially thankful to MetBull for allowing access to their meteorite data, which is essential for Sysyphus's functionality.
```

### Comparing `sysyphus-0.1.1/README.md` & `sysyphus-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 format = "csv"
 
 boulder.save_search(filepath=file_name, file_format=format)
 >>> file saved as csv at met_search  # extension added
 ```
 
 ## Advanced Features
-*Cf. Notebook that i'll try not to forget and link here*
+[Example notebook link](https://github.com/Psemp/sysyphus/blob/main/notebooks/sysyphus_examples.ipynb)
 
 ## Credits
 
 Sysyphus is made possible thanks to the data provided by MetBull and the contributions from our community. <br>I appreciate every piece of input, code, or feedback I've received.
 
 I am especially thankful to MetBull for allowing access to their meteorite data, which is essential for Sysyphus's functionality.
```

### Comparing `sysyphus-0.1.1/setup.py` & `sysyphus-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sysyphus",
-    version="0.1.1",
+    version="0.1.2",
     author="Pierre Sempéré",
     author_email="pierre.sempere.01@gmail.com",
     packages=find_packages(),
     install_requires=[
         "pandas",
         "numpy",
         "beautifulsoup4",
```

### Comparing `sysyphus-0.1.1/sysyphus/models/boulder.py` & `sysyphus-0.1.2/sysyphus/models/boulder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 import numpy as np
 
 import warnings
 
 from sysyphus.scripts import remote_load, search, rendering
 from sysyphus.scripts import user_requests as u_requests
+from sysyphus.scripts.preprocessing import handle_mass
 
 
 class Boulder:
     def __init__(self, use_json: bool = True) -> None:
         """
         Initializes the Boulder object for streamlined access to meteorite data. This object checks for an internet
         connection and loads the latest meteorite dataset, available as JSON or pickle.
@@ -180,14 +181,15 @@
             pd.DataFrame | dict: A pandas DataFrame or dictionary containing the collected meteorite properties,
                                 depending on the value of `as_pd`. Each meteorite is represented by a row (DataFrame)
                                 or a set of key-value pairs in the dictionary, with properties as columns/keys.
         """
 
         if hasattr(self, "met_list") and self.made_requests:
             self.df_searched = rendering.show_properties(meteorite_list=self.met_list, as_pd=as_pandas, ommit=ommit)
+            self.df_searched["mass"] = self.df_searched["mass"].apply(handle_mass)
             try:
                 self.df_searched["mass"] = self.df_searched["mass"].astype(np.float32)
             except AttributeError:
                 pass
             return self.df_searched
         elif hasattr(self, "met_list") and not self.made_requests:
             warnings.warn(message="Selection made but no requests have been made on metbull server")
```

### Comparing `sysyphus-0.1.1/sysyphus/models/meteorite.py` & `sysyphus-0.1.2/sysyphus/models/meteorite.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/sysyphus/scripts/preprocessing.py` & `sysyphus-0.1.2/sysyphus/scripts/preprocessing.py`

 * *Files 19% similar despite different names*

```diff
@@ -78,7 +78,27 @@
     match = re.match(r"[-+]?\d*\.?\d+", to_process)
 
     if match:
         value = match.group()
         return float(value.strip())
     else:
         return np.nan
+
+
+def handle_mass(mass):
+    """Handles mass : assume convert kg to g, handles non specified as g, returns a float"""
+
+    if isinstance(mass, str):
+        numeric_value = re.sub(r'[^\d.]', '', mass)
+
+        if 'kg' in mass.lower():
+            # Convert to grams if "kg" is in the string
+            return float(numeric_value) * 1000
+        elif 'g' in mass.lower() or numeric_value == '':
+            # Return as is if "g" is in the string or if no unit is specified
+            return float(numeric_value) if numeric_value else 0
+        else:
+            # Assume grams if no unit is specified
+            return float(numeric_value)
+
+    else:
+        return np.nan
```

### Comparing `sysyphus-0.1.1/sysyphus/scripts/remote_load.py` & `sysyphus-0.1.2/sysyphus/scripts/remote_load.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/sysyphus/scripts/rendering.py` & `sysyphus-0.1.2/sysyphus/scripts/rendering.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/sysyphus/scripts/search.py` & `sysyphus-0.1.2/sysyphus/scripts/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
 def validate_country(country: str, validation_file: str) -> tuple:
     """Checks if country is valid, returning the country and an error message, if relevant."""
     try:
         with open(file=validation_file, mode="r") as file:
             countries = json.load(file)
     except FileNotFoundError:
+        print("File not found, fetching from GH.")
         country_url = "https://raw.githubusercontent.com/Psemp/sysyphus/main/sysyphus/utils/country_validation.json"
         countries = requests.get(country_url).json()
 
     country = country.lower().strip()
     if len(country) > 0:
         if country.lower() in countries:
             return country, None
@@ -109,14 +110,15 @@
 
 def validate_mtype(mtype: str, validation_file: str) -> tuple:
     """Checks if meteorite type is valid, returning the mtype and an error message, if relevant."""
     try:
         with open(file=validation_file, mode="r") as file:
             types = json.load(file)
     except FileNotFoundError:
+        print("File not found, fetching from GH.")
         type_url = "https://raw.githubusercontent.com/Psemp/sysyphus/main/sysyphus/utils/type_validation.json"
         types = requests.get(type_url).json()
 
     mtype = mtype.lower().strip()
     if len(mtype) > 0:
         if mtype.lower() in types:
             return mtype.lower(), None
@@ -140,18 +142,18 @@
     """
     while True:
         user_input = input(prompt_message).strip()
         if not user_input:  # Skips
             return None
         if validation_function:
             if validation_function == validate_country:
-                validation_file = "sysyphus/utils/country_validation.json"
+                validation_file = "../utils/country_validation.json"
                 validation_result, error_message = validation_function(user_input, validation_file)
             elif validation_function == validate_mtype:
-                validation_file = "sysyphus/utils/type_validation.json"
+                validation_file = "../utils/type_validation.json"
                 validation_result, error_message = validation_function(user_input, validation_file)
             else:
                 validation_result, error_message = validation_function(user_input)
 
             if validation_result is not None:
                 return validation_result
             else:
```

### Comparing `sysyphus-0.1.1/sysyphus/scripts/user_requests.py` & `sysyphus-0.1.2/sysyphus/scripts/user_requests.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/sysyphus.egg-info/PKG-INFO` & `sysyphus-0.1.2/sysyphus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysyphus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Structured meteorite data access using MetBull: Query, filter, and analyze with ease.
 Home-page: https://github.com/Psemp/sysyphus.git
 Author: Pierre Sempéré
 Author-email: pierre.sempere.01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -115,15 +115,15 @@
 format = "csv"
 
 boulder.save_search(filepath=file_name, file_format=format)
 >>> file saved as csv at met_search  # extension added
 ```
 
 ## Advanced Features
-*Cf. Notebook that i'll try not to forget and link here*
+[Example notebook link](https://github.com/Psemp/sysyphus/blob/main/notebooks/sysyphus_examples.ipynb)
 
 ## Credits
 
 Sysyphus is made possible thanks to the data provided by MetBull and the contributions from our community. <br>I appreciate every piece of input, code, or feedback I've received.
 
 I am especially thankful to MetBull for allowing access to their meteorite data, which is essential for Sysyphus's functionality.
```

### Comparing `sysyphus-0.1.1/sysyphus.egg-info/SOURCES.txt` & `sysyphus-0.1.2/sysyphus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/tests/test_boulder.py` & `sysyphus-0.1.2/tests/test_boulder.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/tests/test_meteorite.py` & `sysyphus-0.1.2/tests/test_meteorite.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/tests/test_preprocessing.py` & `sysyphus-0.1.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/tests/test_remote_load.py` & `sysyphus-0.1.2/tests/test_remote_load.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/tests/test_rendering.py` & `sysyphus-0.1.2/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/tests/test_search.py` & `sysyphus-0.1.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `sysyphus-0.1.1/tests/test_user_requests.py` & `sysyphus-0.1.2/tests/test_user_requests.py`

 * *Files identical despite different names*

