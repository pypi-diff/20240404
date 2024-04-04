# Comparing `tmp/easy_encryption_tool-1.0.2-py3-none-any.whl.zip` & `tmp/easy_encryption_tool-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,20 @@
-Zip file size: 19186 bytes, number of entries: 5
--rw-r--r--  2.0 unx    58305 b- defN 24-Apr-04 09:09 easy_encryption_tool-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 09:09 easy_encryption_tool-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 24-Apr-04 09:09 easy_encryption_tool-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-04 09:09 easy_encryption_tool-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      458 b- defN 24-Apr-04 09:09 easy_encryption_tool-1.0.2.dist-info/RECORD
-5 files, 58939 bytes uncompressed, 18318 bytes compressed:  68.9%
+Zip file size: 41158 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-04 09:43 easy_encryption_tool/__init__.py
+-rw-r--r--  2.0 unx    19921 b- defN 24-Apr-04 08:28 easy_encryption_tool/aes_command.py
+-rw-r--r--  2.0 unx    18230 b- defN 24-Apr-04 08:28 easy_encryption_tool/aes_command_test.py
+-rw-r--r--  2.0 unx      702 b- defN 24-Apr-04 08:28 easy_encryption_tool/command_perf.py
+-rw-r--r--  2.0 unx     7394 b- defN 24-Apr-04 08:28 easy_encryption_tool/common.py
+-rw-r--r--  2.0 unx      758 b- defN 24-Apr-04 08:28 easy_encryption_tool/common_test.py
+-rw-r--r--  2.0 unx    12609 b- defN 24-Apr-04 08:28 easy_encryption_tool/ecc_command.py
+-rw-r--r--  2.0 unx     4017 b- defN 24-Apr-04 08:28 easy_encryption_tool/hmac_command.py
+-rw-r--r--  2.0 unx     2301 b- defN 24-Apr-04 09:46 easy_encryption_tool/main.py
+-rw-r--r--  2.0 unx     2526 b- defN 24-Apr-04 08:28 easy_encryption_tool/random_str.py
+-rw-r--r--  2.0 unx      532 b- defN 24-Apr-04 08:28 easy_encryption_tool/random_str_test.py
+-rw-r--r--  2.0 unx    17702 b- defN 24-Apr-04 08:28 easy_encryption_tool/rsa_command.py
+-rw-r--r--  2.0 unx      811 b- defN 24-Apr-04 08:28 easy_encryption_tool/tool_version.py
+-rw-r--r--  2.0 unx    58305 b- defN 24-Apr-04 09:47 easy_encryption_tool-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 09:47 easy_encryption_tool-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 24-Apr-04 09:47 easy_encryption_tool-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-04 09:47 easy_encryption_tool-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1649 b- defN 24-Apr-04 09:47 easy_encryption_tool-1.0.3.dist-info/RECORD
+18 files, 147730 bytes uncompressed, 38400 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -1,16 +1,55 @@
-Filename: easy_encryption_tool-1.0.2.dist-info/METADATA
+Filename: easy_encryption_tool/__init__.py
 Comment: 
 
-Filename: easy_encryption_tool-1.0.2.dist-info/WHEEL
+Filename: easy_encryption_tool/aes_command.py
 Comment: 
 
-Filename: easy_encryption_tool-1.0.2.dist-info/entry_points.txt
+Filename: easy_encryption_tool/aes_command_test.py
 Comment: 
 
-Filename: easy_encryption_tool-1.0.2.dist-info/top_level.txt
+Filename: easy_encryption_tool/command_perf.py
 Comment: 
 
-Filename: easy_encryption_tool-1.0.2.dist-info/RECORD
+Filename: easy_encryption_tool/common.py
+Comment: 
+
+Filename: easy_encryption_tool/common_test.py
+Comment: 
+
+Filename: easy_encryption_tool/ecc_command.py
+Comment: 
+
+Filename: easy_encryption_tool/hmac_command.py
+Comment: 
+
+Filename: easy_encryption_tool/main.py
+Comment: 
+
+Filename: easy_encryption_tool/random_str.py
+Comment: 
+
+Filename: easy_encryption_tool/random_str_test.py
+Comment: 
+
+Filename: easy_encryption_tool/rsa_command.py
+Comment: 
+
+Filename: easy_encryption_tool/tool_version.py
+Comment: 
+
+Filename: easy_encryption_tool-1.0.3.dist-info/METADATA
+Comment: 
+
+Filename: easy_encryption_tool-1.0.3.dist-info/WHEEL
+Comment: 
+
+Filename: easy_encryption_tool-1.0.3.dist-info/entry_points.txt
+Comment: 
+
+Filename: easy_encryption_tool-1.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: easy_encryption_tool-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `easy_encryption_tool-1.0.2.dist-info/METADATA` & `easy_encryption_tool-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: easy-encryption-tool
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://cloud.tencent.com/developer/article/2155922
 Author: bowenerchen
-Author-email: your-email@example.com
+Author-email: bowener.chen@gmail.com
 License: MIT
 Keywords: encryption cli tool security aes hmac ecc rsa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: click
```

