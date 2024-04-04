# Comparing `tmp/muko-1.61-py3-none-any.whl.zip` & `tmp/muko-1.69-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1559115 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
--rw-rw-rw-  2.0 fat   282112 b- defN 24-Mar-21 05:45 muko/cmuko.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Mar-21 05:45 muko-1.61.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1006 b- defN 24-Mar-21 05:45 muko-1.61.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-21 05:45 muko-1.61.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-21 05:45 muko-1.61.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Mar-21 05:45 muko-1.61.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      696 b- defN 24-Mar-21 05:45 muko-1.61.dist-info/RECORD
-9 files, 2367989 bytes uncompressed, 1557927 bytes compressed:  34.2%
+Zip file size: 1559156 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-01 07:17 muko/__init__.py
+-rw-rw-rw-  2.0 fat   282112 b- defN 24-Apr-01 07:17 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  2082964 b- defN 24-Apr-01 07:17 muko/font/default.otf
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-04 06:19 muko-1.69.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1111 b- defN 24-Apr-04 06:19 muko-1.69.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 06:19 muko-1.69.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-04 06:19 muko-1.69.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-04 06:19 muko-1.69.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      696 b- defN 24-Apr-04 06:19 muko-1.69.dist-info/RECORD
+9 files, 2368094 bytes uncompressed, 1557968 bytes compressed:  34.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: muko/cmuko.cp38-win_amd64.pyd
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-1.61.dist-info/LICENSE
+Filename: muko-1.69.dist-info/LICENSE
 Comment: 
 
-Filename: muko-1.61.dist-info/METADATA
+Filename: muko-1.69.dist-info/METADATA
 Comment: 
 
-Filename: muko-1.61.dist-info/WHEEL
+Filename: muko-1.69.dist-info/WHEEL
 Comment: 
 
-Filename: muko-1.61.dist-info/entry_points.txt
+Filename: muko-1.69.dist-info/entry_points.txt
 Comment: 
 
-Filename: muko-1.61.dist-info/top_level.txt
+Filename: muko-1.69.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-1.61.dist-info/RECORD
+Filename: muko-1.69.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-1.61.dist-info/LICENSE` & `muko-1.69.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-1.61.dist-info/METADATA` & `muko-1.69.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 1.61
+Version: 1.69
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests >=2.31.0
 Requires-Dist: moviepy >=1.0.3
 Requires-Dist: pillow ==9.5.0
 Requires-Dist: diskcache >=5.6.3
+Requires-Dist: retrying >=1.3.3
+Requires-Dist: numpy >=1.24.4
+Requires-Dist: opencv-python >=4.9.0.80
 
 # Muko：加速实现AIGC、自动办公的中文编程工具
 
 ## 安装方式
     pip install muko
 
 ## 使用方法
```

