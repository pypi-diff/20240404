# Comparing `tmp/easy_encryption_tool-1.1.1-py3-none-any.whl.zip` & `tmp/easy_encryption_tool-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 34847 bytes, number of entries: 12
+Zip file size: 34843 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    20027 b- defN 24-Apr-04 14:56 aes_command.py
 -rw-r--r--  2.0 unx    12652 b- defN 24-Apr-04 14:56 ecc_command.py
 -rw-r--r--  2.0 unx     4111 b- defN 24-Apr-04 14:56 hmac_command.py
 -rw-r--r--  2.0 unx     2210 b- defN 24-Apr-04 14:56 main.py
 -rw-r--r--  2.0 unx     2675 b- defN 24-Apr-04 14:56 random_str.py
 -rw-r--r--  2.0 unx    17736 b- defN 24-Apr-04 14:56 rsa_command.py
 -rw-r--r--  2.0 unx      870 b- defN 24-Apr-04 14:19 tool_version.py
--rw-r--r--  2.0 unx    59150 b- defN 24-Apr-04 15:04 easy_encryption_tool-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:04 easy_encryption_tool-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 24-Apr-04 15:04 easy_encryption_tool-1.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       78 b- defN 24-Apr-04 15:04 easy_encryption_tool-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      952 b- defN 24-Apr-04 15:04 easy_encryption_tool-1.1.1.dist-info/RECORD
-12 files, 120636 bytes uncompressed, 33263 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx    59150 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       78 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      952 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/RECORD
+12 files, 120615 bytes uncompressed, 33259 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: rsa_command.py
 Comment: 
 
 Filename: tool_version.py
 Comment: 
 
-Filename: easy_encryption_tool-1.1.1.dist-info/METADATA
+Filename: easy_encryption_tool-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: easy_encryption_tool-1.1.1.dist-info/WHEEL
+Filename: easy_encryption_tool-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: easy_encryption_tool-1.1.1.dist-info/entry_points.txt
+Filename: easy_encryption_tool-1.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.1.dist-info/top_level.txt
+Filename: easy_encryption_tool-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.1.dist-info/RECORD
+Filename: easy_encryption_tool-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `easy_encryption_tool-1.1.1.dist-info/METADATA` & `easy_encryption_tool-1.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-encryption-tool
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://cloud.tencent.com/developer/article/2155922
 Author: bowenerchen
 Author-email: bowener.chen@gmail.com
 License: MIT
 Keywords: encryption cli tool security aes hmac ecc rsa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `easy_encryption_tool-1.1.1.dist-info/RECORD` & `easy_encryption_tool-1.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 aes_command.py,sha256=CbhUaS5d_5pRnsaZV7VSi6CAsAkzLP1k2ZUwcBWgCuc,20027
 ecc_command.py,sha256=g76LOqS-UILqXSgFZhqw_1qAXpXDZRUNslcmAQHmkpk,12652
 hmac_command.py,sha256=mQaZ9dDsh3q4KNEhkyht8bVPcT5LD0Oq8b2tEpqxWKg,4111
 main.py,sha256=e3YHOsFViRrS_TMd6Pv8wLu4EaZO4GFvuUPnDV0zLs8,2210
 random_str.py,sha256=Mz8QkU8w-TrKWxLKhevXtic9_EPryeYlJcrEhXaQcVA,2675
 rsa_command.py,sha256=QsAJUo69Yo8EpZ3mbu4mbIR50NGPoRXfzZPtHJAOIGg,17736
 tool_version.py,sha256=Gz2mCkhX1Ztrpr_TaTBkyVWs9Yk3gX8QxxlgkB4ga0A,870
-easy_encryption_tool-1.1.1.dist-info/METADATA,sha256=zkpM15gre7VZfXi6fHb_Kp8wJy53lXURT4O21GVUM6Q,59150
-easy_encryption_tool-1.1.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-easy_encryption_tool-1.1.1.dist-info/entry_points.txt,sha256=qrNi4Ml3z53yoZNoOEQFVofyZCmLG_sUQSytiejkJYY,83
-easy_encryption_tool-1.1.1.dist-info/top_level.txt,sha256=VrL6mzxpOyPrY3rdPaG8fWebkdOyE2154AoYveQpDio,78
-easy_encryption_tool-1.1.1.dist-info/RECORD,,
+easy_encryption_tool-1.1.2.dist-info/METADATA,sha256=VWGGhemdYUuMaU1RJZim6gvetKC31XSsfO-jr5nU8ac,59150
+easy_encryption_tool-1.1.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+easy_encryption_tool-1.1.2.dist-info/entry_points.txt,sha256=PhqlR4Bl8hLdmVL11hpBv7XBL6oXeOA2fxOg_0PC5R8,62
+easy_encryption_tool-1.1.2.dist-info/top_level.txt,sha256=VrL6mzxpOyPrY3rdPaG8fWebkdOyE2154AoYveQpDio,78
+easy_encryption_tool-1.1.2.dist-info/RECORD,,
```

