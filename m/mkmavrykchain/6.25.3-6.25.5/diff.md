# Comparing `tmp/mkmavrykchain-6.25.3-py3-none-any.whl.zip` & `tmp/mkmavrykchain-6.25.5-py3-none-any.whl.zip`

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
+-rw-r--r--  2.0 unx      498 b- defN 24-Apr-04 10:03 mavrykchain/_version.py
+-rw-r--r--  2.0 unx     1916 b- defN 24-Apr-04 10:03 mavrykchain/keys.py
+-rw-r--r--  2.0 unx    12374 b- defN 24-Apr-04 10:03 mavrykchain/mkmavrykchain.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-Apr-04 10:03 mavrykchain/parameters.yaml
+-rw-r--r--  2.0 unx     5164 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      753 b- defN 24-Apr-04 10:03 mkmavrykchain-6.25.5.dist-info/RECORD
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
+Filename: mkmavrykchain-6.25.5.dist-info/METADATA
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/WHEEL
+Filename: mkmavrykchain-6.25.5.dist-info/WHEEL
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/entry_points.txt
+Filename: mkmavrykchain-6.25.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/top_level.txt
+Filename: mkmavrykchain-6.25.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.3.dist-info/RECORD
+Filename: mkmavrykchain-6.25.5.dist-info/RECORD
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
+ "date": "2024-04-04T11:52:15+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "3ab6bc2177e3977314c8aae6390903c2b121c887",
- "version": "6.25.3"
+ "full-revisionid": "78188ae4e7ffb221b0b7f96b61635ea918c13c82",
+ "version": "6.25.5"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `mkmavrykchain-6.25.3.dist-info/METADATA` & `mkmavrykchain-6.25.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkmavrykchain
-Version: 6.25.3
+Version: 6.25.5
 Summary: A utility to generate k8s configs for a Mavryk blockchain
 Home-page: https://github.com/mavryk-network/mavryk-k8s
 Author: MavrykDynamics
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `mkmavrykchain-6.25.3.dist-info/RECORD` & `mkmavrykchain-6.25.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-mavrykchain/_version.py,sha256=cWsTE_a2UlC0cZv-KddWnmMhdlMyFiCWfNJCv4qeqjE,498
+mavrykchain/_version.py,sha256=vDyA_X5BqullEilFuLRyXKjOoDAzk4gXoQe29_o0NMI,498
 mavrykchain/keys.py,sha256=i_WucWcLv2XoKd-z63Ki4BWis_64VsL-OVrj2hu-Gv0,1916
 mavrykchain/mkmavrykchain.py,sha256=TDBG5gKgusS_o43NV7cC0BDlfWkwakySefIq35P-YSM,12374
 mavrykchain/parameters.yaml,sha256=7bLg5OtDeWjgTTijnNir2V-nGyFC2aaLJQpQCIRgK90,2580
-mkmavrykchain-6.25.3.dist-info/METADATA,sha256=m6ZuRQG5SJbG7HITlcFhFyth_sYpa139jHXrafE27hg,5164
-mkmavrykchain-6.25.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-mkmavrykchain-6.25.3.dist-info/entry_points.txt,sha256=RaUjd8-SPBeldKrftLUDs1jh1XlxOqk_Gvm3VFviv3A,66
-mkmavrykchain-6.25.3.dist-info/top_level.txt,sha256=Xs8ZuCG2QSYUYjjR3gAebOqJE79DyahLQca0YZjKzMk,12
-mkmavrykchain-6.25.3.dist-info/RECORD,,
+mkmavrykchain-6.25.5.dist-info/METADATA,sha256=OF5sLcLdWOUZBQ03VdEEN4vdAK22a4fapk9IUHnht6Y,5164
+mkmavrykchain-6.25.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mkmavrykchain-6.25.5.dist-info/entry_points.txt,sha256=RaUjd8-SPBeldKrftLUDs1jh1XlxOqk_Gvm3VFviv3A,66
+mkmavrykchain-6.25.5.dist-info/top_level.txt,sha256=Xs8ZuCG2QSYUYjjR3gAebOqJE79DyahLQca0YZjKzMk,12
+mkmavrykchain-6.25.5.dist-info/RECORD,,
```

