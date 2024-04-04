# Comparing `tmp/evtx-0.8.3-cp37-abi3-win_amd64.whl.zip` & `tmp/evtx-0.8.4-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 735948 bytes, number of entries: 5
--rw-r--r--  4.6 unx     3234 b- defN 23-Nov-05 14:22 evtx-0.8.3.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Nov-05 14:22 evtx-0.8.3.dist-info/WHEEL
--rw-r--r--  4.6 unx       99 b- defN 23-Nov-05 14:22 evtx/__init__.py
--rwxr-xr-x  4.6 unx  1522176 b- defN 23-Nov-05 14:22 evtx/evtx.pyd
--rw-r--r--  4.6 unx      341 b- defN 23-Nov-05 14:22 evtx-0.8.3.dist-info/RECORD
-5 files, 1525944 bytes uncompressed, 735324 bytes compressed:  51.8%
+Zip file size: 731004 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     3234 b- defN 24-Apr-04 10:01 evtx-0.8.4.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-Apr-04 10:01 evtx-0.8.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx       99 b- defN 24-Apr-04 10:01 evtx/__init__.py
+-rwxr-xr-x  4.6 unx  1525760 b- defN 24-Apr-04 10:01 evtx/evtx.pyd
+-rw-r--r--  4.6 unx      341 b- defN 24-Apr-04 10:01 evtx-0.8.4.dist-info/RECORD
+5 files, 1529528 bytes uncompressed, 730380 bytes compressed:  52.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: evtx-0.8.3.dist-info/METADATA
+Filename: evtx-0.8.4.dist-info/METADATA
 Comment: 
 
-Filename: evtx-0.8.3.dist-info/WHEEL
+Filename: evtx-0.8.4.dist-info/WHEEL
 Comment: 
 
 Filename: evtx/__init__.py
 Comment: 
 
 Filename: evtx/evtx.pyd
 Comment: 
 
-Filename: evtx-0.8.3.dist-info/RECORD
+Filename: evtx-0.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `evtx-0.8.3.dist-info/METADATA` & `evtx-0.8.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: evtx
-Version: 0.8.3
+Version: 0.8.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evtx Version: 0.8.3 Classifier: Development Status
+Metadata-Version: 2.3 Name: evtx Version: 0.8.4 Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust Requires-Dist: pytest ; extra ==
 'test' Provides-Extra: test Summary: Python bindings for https://github.com/
```

