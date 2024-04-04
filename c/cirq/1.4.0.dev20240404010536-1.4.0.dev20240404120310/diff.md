# Comparing `tmp/cirq-1.4.0.dev20240404010536-py3-none-any.whl.zip` & `tmp/cirq-1.4.0.dev20240404120310-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8397 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 24-Apr-04 01:05 cirq-1.4.0.dev20240404010536.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-04 01:05 cirq-1.4.0.dev20240404010536.dist-info/LICENSE
--rw-r--r--  2.0 unx     7977 b- defN 24-Apr-04 01:05 cirq-1.4.0.dev20240404010536.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 01:05 cirq-1.4.0.dev20240404010536.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 01:05 cirq-1.4.0.dev20240404010536.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 24-Apr-04 01:05 cirq-1.4.0.dev20240404010536.dist-info/RECORD
-6 files, 20282 bytes uncompressed, 7359 bytes compressed:  63.7%
+Zip file size: 8341 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 24-Apr-04 12:03 cirq-1.4.0.dev20240404120310.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-04 12:03 cirq-1.4.0.dev20240404120310.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7832 b- defN 24-Apr-04 12:03 cirq-1.4.0.dev20240404120310.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 12:03 cirq-1.4.0.dev20240404120310.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 12:03 cirq-1.4.0.dev20240404120310.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 24-Apr-04 12:03 cirq-1.4.0.dev20240404120310.dist-info/RECORD
+6 files, 20137 bytes uncompressed, 7303 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.4.0.dev20240404010536.dist-info/AUTHORS
+Filename: cirq-1.4.0.dev20240404120310.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.4.0.dev20240404010536.dist-info/LICENSE
+Filename: cirq-1.4.0.dev20240404120310.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.4.0.dev20240404010536.dist-info/METADATA
+Filename: cirq-1.4.0.dev20240404120310.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.4.0.dev20240404010536.dist-info/WHEEL
+Filename: cirq-1.4.0.dev20240404120310.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.4.0.dev20240404010536.dist-info/top_level.txt
+Filename: cirq-1.4.0.dev20240404120310.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.4.0.dev20240404010536.dist-info/RECORD
+Filename: cirq-1.4.0.dev20240404120310.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.4.0.dev20240404010536.dist-info/LICENSE` & `cirq-1.4.0.dev20240404120310.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.4.0.dev20240404010536.dist-info/METADATA` & `cirq-1.4.0.dev20240404120310.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.4.0.dev20240404010536
+Version: 1.4.0.dev20240404120310
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Requires-Python: >=3.9.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt ==1.4.0.dev20240404010536
-Requires-Dist: cirq-core ==1.4.0.dev20240404010536
-Requires-Dist: cirq-ft ==1.4.0.dev20240404010536
-Requires-Dist: cirq-google ==1.4.0.dev20240404010536
-Requires-Dist: cirq-ionq ==1.4.0.dev20240404010536
-Requires-Dist: cirq-pasqal ==1.4.0.dev20240404010536
-Requires-Dist: cirq-rigetti ==1.4.0.dev20240404010536
-Requires-Dist: cirq-web ==1.4.0.dev20240404010536
+Requires-Dist: cirq-aqt ==1.4.0.dev20240404120310
+Requires-Dist: cirq-core ==1.4.0.dev20240404120310
+Requires-Dist: cirq-ft ==1.4.0.dev20240404120310
+Requires-Dist: cirq-google ==1.4.0.dev20240404120310
+Requires-Dist: cirq-ionq ==1.4.0.dev20240404120310
+Requires-Dist: cirq-pasqal ==1.4.0.dev20240404120310
+Requires-Dist: cirq-rigetti ==1.4.0.dev20240404120310
+Requires-Dist: cirq-web ==1.4.0.dev20240404120310
 Provides-Extra: dev_env
 Requires-Dist: mypy ==1.2.0 ; extra == 'dev_env'
 Requires-Dist: types-backports ==0.1.3 ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf ~=3.20 ; extra == 'dev_env'
 Requires-Dist: types-requests ==2.28.1 ; extra == 'dev_env'
 Requires-Dist: types-setuptools ==62.6.1 ; extra == 'dev_env'
@@ -160,16 +160,14 @@
 
 We welcome contributions! Before opening your first PR, a good place to start is to read our
 `guidelines <https://github.com/quantumlib/cirq/blob/main/CONTRIBUTING.md>`__.
 
 We are dedicated to cultivating an open and inclusive community to build software for near term quantum computers.
 Please read our `code of conduct <https://github.com/quantumlib/cirq/blob/main/CODE_OF_CONDUCT.md>`__ for the rules of engagement within our community.
 
-For real time informal discussions about Cirq, join our `cirqdev <https://gitter.im/cirqdev/community>`__ Gitter channel, come hangout with us!
-
 **Cirq Cynque** is our weekly meeting for contributors to discuss upcoming features, designs, issues, community and status of different efforts.
 To get an invitation please join the `cirq-dev email list <https://groups.google.com/forum/#!forum/cirq-dev>`__ which also serves as yet another platform to discuss contributions and design ideas.
 
 
 See Also
 --------
```

