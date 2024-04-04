# Comparing `tmp/mkmavrykchain-6.25.3-py3-none-any.whl.zip` & `tmp/mkmavrykchain-6.25.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9475 bytes, number of entries: 9
--rw-r--r--  2.0 unx      498 b- defN 24-Feb-27 08:11 mavrykchain/_version.py
--rw-r--r--  2.0 unx     1916 b- defN 24-Feb-27 08:11 mavrykchain/keys.py
--rw-r--r--  2.0 unx    12374 b- defN 24-Feb-27 08:11 mavrykchain/mkmavrykchain.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Feb-27 08:11 mavrykchain/parameters.yaml
--rw-r--r--  2.0 unx     5164 b- defN 24-Feb-27 08:11 mkmavrykchain-6.25.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-27 08:11 mkmavrykchain-6.25.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 24-Feb-27 08:11 mkmavrykchain-6.25.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Feb-27 08:11 mkmavrykchain-6.25.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      753 b- defN 24-Feb-27 08:11 mkmavrykchain-6.25.3.dist-info/RECORD
-9 files, 23455 bytes uncompressed, 8169 bytes compressed:  65.2%
+Zip file size: 9476 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      498 b- defN 24-Apr-04 09:33 mavrykchain/_version.py
+-rw-r--r--  2.0 unx     1916 b- defN 24-Apr-04 09:33 mavrykchain/keys.py
+-rw-r--r--  2.0 unx    12374 b- defN 24-Apr-04 09:33 mavrykchain/mkmavrykchain.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-Apr-04 09:33 mavrykchain/parameters.yaml
+-rw-r--r--  2.0 unx     5164 b- defN 24-Apr-04 09:33 mkmavrykchain-6.25.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 09:33 mkmavrykchain-6.25.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-04 09:33 mkmavrykchain-6.25.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 09:33 mkmavrykchain-6.25.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      753 b- defN 24-Apr-04 09:33 mkmavrykchain-6.25.4.dist-info/RECORD
+9 files, 23455 bytes uncompressed, 8170 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mavrykchain/mkmavrykchain.py
 Comment: 
 
 Filename: mavrykchain/parameters.yaml
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/METADATA
+Filename: mkmavrykchain-6.25.4.dist-info/METADATA
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/WHEEL
+Filename: mkmavrykchain-6.25.4.dist-info/WHEEL
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/entry_points.txt
+Filename: mkmavrykchain-6.25.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/top_level.txt
+Filename: mkmavrykchain-6.25.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/RECORD
+Filename: mkmavrykchain-6.25.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mavrykchain/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-02-27T09:08:49+0100",
+ "date": "2024-04-04T11:18:54+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "3ab6bc2177e3977314c8aae6390903c2b121c887",
- "version": "6.25.3"
+ "full-revisionid": "380e58ecd0082e713bddd2a4c9b0e9c6284d81b2",
+ "version": "6.25.4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `mkmavrykchain-6.25.3.dist-info/METADATA` & `mkmavrykchain-6.25.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkmavrykchain
-Version: 6.25.3
+Version: 6.25.4
 Summary: A utility to generate k8s configs for a Mavryk blockchain
 Home-page: https://github.com/mavryk-network/mavryk-k8s
 Author: MavrykDynamics
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

