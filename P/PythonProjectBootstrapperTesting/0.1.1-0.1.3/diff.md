# Comparing `tmp/PythonProjectBootstrapperTesting-0.1.1-py3-none-any.whl.zip` & `tmp/PythonProjectBootstrapperTesting-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7565 bytes, number of entries: 10
--rw-r--r--  2.0 unx     3427 b- defN 24-Mar-28 14:08 BuildBinary.py
--rw-r--r--  2.0 unx     2460 b- defN 24-Mar-28 14:08 PythonProjectBootstrapperTesting/EntryPoint.py
--rw-r--r--  2.0 unx      808 b- defN 24-Mar-28 14:08 PythonProjectBootstrapperTesting/Math.py
--rw-r--r--  2.0 unx      598 b- defN 24-Mar-28 14:10 PythonProjectBootstrapperTesting/__init__.py
--rw-r--r--  2.0 unx     1070 b- defN 24-Mar-28 14:10 PythonProjectBootstrapperTesting-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5964 b- defN 24-Mar-28 14:10 PythonProjectBootstrapperTesting-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-28 14:10 PythonProjectBootstrapperTesting-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      101 b- defN 24-Mar-28 14:10 PythonProjectBootstrapperTesting-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       45 b- defN 24-Mar-28 14:10 PythonProjectBootstrapperTesting-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1006 b- defN 24-Mar-28 14:10 PythonProjectBootstrapperTesting-0.1.1.dist-info/RECORD
-10 files, 15571 bytes uncompressed, 5789 bytes compressed:  62.8%
+Zip file size: 7567 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     3427 b- defN 24-Apr-04 19:11 BuildBinary.py
+-rw-r--r--  2.0 unx     2460 b- defN 24-Apr-04 19:11 PythonProjectBootstrapperTesting/EntryPoint.py
+-rw-r--r--  2.0 unx      808 b- defN 24-Apr-04 19:11 PythonProjectBootstrapperTesting/Math.py
+-rw-r--r--  2.0 unx      598 b- defN 24-Apr-04 19:12 PythonProjectBootstrapperTesting/__init__.py
+-rw-r--r--  2.0 unx     1070 b- defN 24-Apr-04 19:12 PythonProjectBootstrapperTesting-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5964 b- defN 24-Apr-04 19:12 PythonProjectBootstrapperTesting-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 19:12 PythonProjectBootstrapperTesting-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      101 b- defN 24-Apr-04 19:12 PythonProjectBootstrapperTesting-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       45 b- defN 24-Apr-04 19:12 PythonProjectBootstrapperTesting-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1006 b- defN 24-Apr-04 19:12 PythonProjectBootstrapperTesting-0.1.3.dist-info/RECORD
+10 files, 15571 bytes uncompressed, 5791 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: PythonProjectBootstrapperTesting/Math.py
 Comment: 
 
 Filename: PythonProjectBootstrapperTesting/__init__.py
 Comment: 
 
-Filename: PythonProjectBootstrapperTesting-0.1.1.dist-info/LICENSE.txt
+Filename: PythonProjectBootstrapperTesting-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PythonProjectBootstrapperTesting-0.1.1.dist-info/METADATA
+Filename: PythonProjectBootstrapperTesting-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: PythonProjectBootstrapperTesting-0.1.1.dist-info/WHEEL
+Filename: PythonProjectBootstrapperTesting-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: PythonProjectBootstrapperTesting-0.1.1.dist-info/entry_points.txt
+Filename: PythonProjectBootstrapperTesting-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: PythonProjectBootstrapperTesting-0.1.1.dist-info/top_level.txt
+Filename: PythonProjectBootstrapperTesting-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: PythonProjectBootstrapperTesting-0.1.1.dist-info/RECORD
+Filename: PythonProjectBootstrapperTesting-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PythonProjectBootstrapperTesting/__init__.py

```diff
@@ -5,10 +5,10 @@
 # |
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.1.1"
+__version__ = "0.1.3"
 
 from .Math import Add, Sub, Mult, Div
```

## Comparing `PythonProjectBootstrapperTesting-0.1.1.dist-info/LICENSE.txt` & `PythonProjectBootstrapperTesting-0.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PythonProjectBootstrapperTesting-0.1.1.dist-info/METADATA` & `PythonProjectBootstrapperTesting-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonProjectBootstrapperTesting
-Version: 0.1.1
+Version: 0.1.3
 Summary: Python project bootstrapper test output
 Author-email: Varun Narayan <varun646@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/varun646/PythonProjectBootstrapperTest
 Project-URL: Documentation, https://github.com/varun646/PythonProjectBootstrapperTest
 Project-URL: Repository, https://github.com/varun646/PythonProjectBootstrapperTest
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `PythonProjectBootstrapperTesting-0.1.1.dist-info/RECORD` & `PythonProjectBootstrapperTesting-0.1.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BuildBinary.py,sha256=rQShgIe6RTSi_DFoCa-cdFvms21kN_mGa-xGqX_9dXw,3427
 PythonProjectBootstrapperTesting/EntryPoint.py,sha256=oZ8TnBhSVBMvwlsAuDixWUIxrQd7yeHpU3nc5x7GJ6Y,2460
 PythonProjectBootstrapperTesting/Math.py,sha256=aUm0KDTRFx9IYqr79V5Atn8ga4oxejw463BkUhbBZFA,808
-PythonProjectBootstrapperTesting/__init__.py,sha256=VfixXIBmvc9xRWuttpUbc6zg0Ua9cnOmQR0g-ADWdeA,598
-PythonProjectBootstrapperTesting-0.1.1.dist-info/LICENSE.txt,sha256=WBlSW4Qvbeslvep-aQSsmd1PQkBmkLRs3JBQXUePkNU,1070
-PythonProjectBootstrapperTesting-0.1.1.dist-info/METADATA,sha256=VPiivTvZ6GIo48cFmqOsiBZ4uRhoP_oBPJ2-dvsPhP0,5964
-PythonProjectBootstrapperTesting-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-PythonProjectBootstrapperTesting-0.1.1.dist-info/entry_points.txt,sha256=1gt4J9yQiimDALt4IqP_aGDLeNSUMOBIwLkEmp4BQIs,101
-PythonProjectBootstrapperTesting-0.1.1.dist-info/top_level.txt,sha256=MFuqP5vjEVddpulYfiPlnu7MPr7x_jRuo-tdkiTjrfY,45
-PythonProjectBootstrapperTesting-0.1.1.dist-info/RECORD,,
+PythonProjectBootstrapperTesting/__init__.py,sha256=XUFAIOQg6tkL_sU-1xvF8M2RAsaDa-_MZ2d2g97hf0s,598
+PythonProjectBootstrapperTesting-0.1.3.dist-info/LICENSE.txt,sha256=WBlSW4Qvbeslvep-aQSsmd1PQkBmkLRs3JBQXUePkNU,1070
+PythonProjectBootstrapperTesting-0.1.3.dist-info/METADATA,sha256=LQbAgWerQDwVw1HghQZA1_eD6q0chXI7ruMgTk4ngBk,5964
+PythonProjectBootstrapperTesting-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+PythonProjectBootstrapperTesting-0.1.3.dist-info/entry_points.txt,sha256=1gt4J9yQiimDALt4IqP_aGDLeNSUMOBIwLkEmp4BQIs,101
+PythonProjectBootstrapperTesting-0.1.3.dist-info/top_level.txt,sha256=MFuqP5vjEVddpulYfiPlnu7MPr7x_jRuo-tdkiTjrfY,45
+PythonProjectBootstrapperTesting-0.1.3.dist-info/RECORD,,
```

