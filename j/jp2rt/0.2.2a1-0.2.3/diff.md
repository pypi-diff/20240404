# Comparing `tmp/jp2rt-0.2.2a1.tar.gz` & `tmp/jp2rt-0.2.3.tar.gz`

## Comparing `jp2rt-0.2.2a1.tar` & `jp2rt-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/java/src/licenseHeaderFile.txt
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/java/src/overview.html
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsCalculator.java
--rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsWrapper.java
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/TSVRow.java
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/WrappedMolecularDescriptor.java
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/package-info.java
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/python/jp2rt/__init__.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/python/jp2rt/java.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/python/jp2rt/ml.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/python/jp2rt/scripts.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/.gitignore
--rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/LICENSE-CC.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/LICENSE-GPL.txt
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/README.md
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/pyproject.toml
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 jp2rt-0.2.2a1/PKG-INFO
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jp2rt-0.2.3/java/src/licenseHeaderFile.txt
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jp2rt-0.2.3/java/src/overview.html
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsCalculator.java
+-rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsWrapper.java
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/TSVRow.java
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/WrappedMolecularDescriptor.java
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/package-info.java
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 jp2rt-0.2.3/python/jp2rt/__init__.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 jp2rt-0.2.3/python/jp2rt/java.py
+-rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 jp2rt-0.2.3/python/jp2rt/ml.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 jp2rt-0.2.3/python/jp2rt/scripts.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jp2rt-0.2.3/.gitignore
+-rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 jp2rt-0.2.3/LICENSE-CC.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 jp2rt-0.2.3/LICENSE-GPL.txt
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 jp2rt-0.2.3/README.md
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 jp2rt-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 jp2rt-0.2.3/PKG-INFO
```

### Comparing `jp2rt-0.2.2a1/java/src/licenseHeaderFile.txt` & `jp2rt-0.2.3/java/src/licenseHeaderFile.txt`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsCalculator.java` & `jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsCalculator.java`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsWrapper.java` & `jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/MolecularDescriptorsWrapper.java`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/TSVRow.java` & `jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/TSVRow.java`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/WrappedMolecularDescriptor.java` & `jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/WrappedMolecularDescriptor.java`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/java/src/main/java/it/unimi/di/jp2rt/package-info.java` & `jp2rt-0.2.3/java/src/main/java/it/unimi/di/jp2rt/package-info.java`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/python/jp2rt/__init__.py` & `jp2rt-0.2.3/python/jp2rt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from importlib.util import find_spec
 
-__version__ = '0.2.2a1'
+__version__ = '0.2.3'
 
 HAS_PLOT = (find_spec('matplotlib') is not None) and (find_spec('seaborn') is not None)
 
 from jp2rt.java import (  # noqa: E402
   add_descriptors_via_tsv,
   compute_descriptors,
   compute_single_descriptor,
```

### Comparing `jp2rt-0.2.2a1/python/jp2rt/java.py` & `jp2rt-0.2.3/python/jp2rt/java.py`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/python/jp2rt/ml.py` & `jp2rt-0.2.3/python/jp2rt/ml.py`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/python/jp2rt/scripts.py` & `jp2rt-0.2.3/python/jp2rt/scripts.py`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/LICENSE-CC.txt` & `jp2rt-0.2.3/LICENSE-CC.txt`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/LICENSE-GPL.txt` & `jp2rt-0.2.3/LICENSE-GPL.txt`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/README.md` & `jp2rt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/pyproject.toml` & `jp2rt-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jp2rt-0.2.2a1/PKG-INFO` & `jp2rt-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jp2rt
-Version: 0.2.2a1
+Version: 0.2.3
 Summary: A Java and Python package for Predicting Retention Times
 Project-URL: Home, https://mapio.github.io/jp2rt/
 Project-URL: Issues, https://github.com/mapio/jp2rt/issues
 Project-URL: Source, https://github.com/mapio/jp2rt
 Author-email: Massimo Santini <santini@di.unimi.it>
 License-Expression: MIT
 License-File: LICENSE-CC.txt
```

