# Comparing `tmp/anyon-4.1.0-cp312-none-win_amd64.whl.zip` & `tmp/anyon-4.1.1-cp310-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 462859 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Mar-19 12:00 anyon-4.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2334 b- defN 24-Mar-19 12:00 anyon-4.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-19 12:00 anyon-4.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-19 12:00 anyon-4.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      376 b- defN 24-Mar-19 12:00 anyon-4.1.0.dist-info/RECORD
--rw-rw-rw-  2.0 fat    21504 b- defN 24-Mar-19 11:59 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    94208 b- defN 24-Mar-19 11:59 anyon/loader.pyd
--rw-rw-rw-  2.0 fat   122368 b- defN 24-Mar-19 11:59 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   211456 b- defN 24-Mar-19 11:59 anyon/server.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 24-Mar-19 12:00 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat   248832 b- defN 24-Mar-19 12:00 anyon/stage/assembler.pyd
--rw-rw-rw-  2.0 fat   101376 b- defN 24-Mar-19 12:00 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   140800 b- defN 24-Mar-19 12:00 anyon/stage/device.pyd
--rw-rw-rw-  2.0 fat    68096 b- defN 24-Mar-19 12:00 anyon/stage/processor.pyd
-14 files, 1034552 bytes uncompressed, 461099 bytes compressed:  55.4%
+Zip file size: 430792 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-04 09:20 anyon-4.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2344 b- defN 24-Apr-04 09:20 anyon-4.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-04 09:20 anyon-4.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-04 09:20 anyon-4.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      376 b- defN 24-Apr-04 09:20 anyon-4.1.1.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    20480 b- defN 24-Apr-04 09:20 anyon/__init__.pyd
+-rw-rw-rw-  2.0 fat    88064 b- defN 24-Apr-04 09:20 anyon/loader.pyd
+-rw-rw-rw-  2.0 fat   113152 b- defN 24-Apr-04 09:20 anyon/remote.pyd
+-rw-rw-rw-  2.0 fat   190464 b- defN 24-Apr-04 09:20 anyon/server.pyd
+-rw-rw-rw-  2.0 fat    20992 b- defN 24-Apr-04 09:20 anyon/stage/__init__.pyd
+-rw-rw-rw-  2.0 fat   228864 b- defN 24-Apr-04 09:20 anyon/stage/assembler.pyd
+-rw-rw-rw-  2.0 fat    91648 b- defN 24-Apr-04 09:20 anyon/stage/calculator.pyd
+-rw-rw-rw-  2.0 fat   131072 b- defN 24-Apr-04 09:20 anyon/stage/device.pyd
+-rw-rw-rw-  2.0 fat    62464 b- defN 24-Apr-04 09:20 anyon/stage/processor.pyd
+14 files, 951106 bytes uncompressed, 429032 bytes compressed:  54.9%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: anyon-4.1.0.dist-info/LICENSE
+Filename: anyon-4.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-4.1.0.dist-info/METADATA
+Filename: anyon-4.1.1.dist-info/METADATA
 Comment: 
 
-Filename: anyon-4.1.0.dist-info/WHEEL
+Filename: anyon-4.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-4.1.0.dist-info/top_level.txt
+Filename: anyon-4.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-4.1.0.dist-info/RECORD
+Filename: anyon-4.1.1.dist-info/RECORD
 Comment: 
 
 Filename: anyon/__init__.pyd
 Comment: 
 
 Filename: anyon/loader.pyd
 Comment:
```

## Comparing `anyon-4.1.0.dist-info/LICENSE` & `anyon-4.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anyon-4.1.0.dist-info/METADATA` & `anyon-4.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyon
-Version: 4.1.0
+Version: 4.1.1
 Summary: description
 Author-email: YL <fengyl@pku.edu.cn>
 License: MIT License
         
         Copyright (c) 2021 YL Feng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy >=1.20.0
-Requires-Dist: axion >=3.4.5
-Requires-Dist: srpc >=4.2.8
-Requires-Dist: zee >=0.0.3
-Requires-Dist: requests >=2.28.0
+Requires-Dist: numpy (>=1.20.0)
+Requires-Dist: axion (>=3.4.5)
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.3)
+Requires-Dist: requests (>=2.28.0)
 Requires-Dist: APScheduler
```

