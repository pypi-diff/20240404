# Comparing `tmp/easy_encryption_tool-1.1.3-py3-none-any.whl.zip` & `tmp/easy_encryption_tool-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 34736 bytes, number of entries: 12
--rw-r--r--  2.0 unx    19949 b- defN 24-Apr-04 15:11 aes_command.py
+Zip file size: 34735 bytes, number of entries: 12
+-rw-r--r--  2.0 unx    19949 b- defN 24-Apr-04 15:14 aes_command.py
 -rw-r--r--  2.0 unx    12600 b- defN 24-Apr-04 15:09 ecc_command.py
 -rw-r--r--  2.0 unx     4033 b- defN 24-Apr-04 15:09 hmac_command.py
 -rw-r--r--  2.0 unx     2214 b- defN 24-Apr-04 15:09 main.py
 -rw-r--r--  2.0 unx     2655 b- defN 24-Apr-04 15:09 random_str.py
 -rw-r--r--  2.0 unx    17684 b- defN 24-Apr-04 15:09 rsa_command.py
 -rw-r--r--  2.0 unx      844 b- defN 24-Apr-04 15:09 tool_version.py
--rw-r--r--  2.0 unx    59150 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       78 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      952 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/RECORD
-12 files, 120313 bytes uncompressed, 33152 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx    59150 b- defN 24-Apr-04 15:15 easy_encryption_tool-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:15 easy_encryption_tool-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 15:15 easy_encryption_tool-1.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       78 b- defN 24-Apr-04 15:15 easy_encryption_tool-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      952 b- defN 24-Apr-04 15:15 easy_encryption_tool-1.1.4.dist-info/RECORD
+12 files, 120313 bytes uncompressed, 33151 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: rsa_command.py
 Comment: 
 
 Filename: tool_version.py
 Comment: 
 
-Filename: easy_encryption_tool-1.1.3.dist-info/METADATA
+Filename: easy_encryption_tool-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: easy_encryption_tool-1.1.3.dist-info/WHEEL
+Filename: easy_encryption_tool-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: easy_encryption_tool-1.1.3.dist-info/entry_points.txt
+Filename: easy_encryption_tool-1.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.3.dist-info/top_level.txt
+Filename: easy_encryption_tool-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.3.dist-info/RECORD
+Filename: easy_encryption_tool-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aes_command.py

 * *Ordering differences only*

```diff
@@ -9,17 +9,17 @@
 from typing import Tuple
 
 import click
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import padding
 from cryptography.hazmat.primitives.ciphers import algorithms, Cipher, modes
 
+import command_perf
 import common
 import random_str
-import command_perf
 
 algorithm: str = 'aes'
 
 aes_block_in_bytes = algorithms.AES.block_size // 8
 
 aes_key_len_256: int = 32  # 32字节
 aes_iv_len_128: int = 16  # 16字节
```

## Comparing `easy_encryption_tool-1.1.3.dist-info/METADATA` & `easy_encryption_tool-1.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-encryption-tool
-Version: 1.1.3
+Version: 1.1.4
 Home-page: https://cloud.tencent.com/developer/article/2155922
 Author: bowenerchen
 Author-email: bowener.chen@gmail.com
 License: MIT
 Keywords: encryption cli tool security aes hmac ecc rsa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `easy_encryption_tool-1.1.3.dist-info/RECORD` & `easy_encryption_tool-1.1.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-aes_command.py,sha256=mtlCkFOf9z22BjE0gEC1pj0zIF5RrsmBqIongBAmar4,19949
+aes_command.py,sha256=uD8zks4Q4FSs7nV7dBxa5qd7jHPLlHFkniUgdCtxLOA,19949
 ecc_command.py,sha256=HMFZpNOzTBzYrKlidZAi759e_71fPJN2vZfoahlamxY,12600
 hmac_command.py,sha256=qEF1MM7nIo8eq0W60IwR9Wz8NmHlNK7l22gLSOaEwUg,4033
 main.py,sha256=JbIKp9BbnNjN_rFiQTSHAMfo13S9_qp32W74-dES5r4,2214
 random_str.py,sha256=_pwixdXMppOEJCfXlATaXFHqLzhc6wVVyo_ezVCU1vY,2655
 rsa_command.py,sha256=Dlc4PQagXbWH1PsgfXuMh5_Kc0aQc4p3wDhz28cFUus,17684
 tool_version.py,sha256=2XtagEC0RJUr6AGU3cp3UG_HgInbfSNylcraubSgKis,844
-easy_encryption_tool-1.1.3.dist-info/METADATA,sha256=wJd0N-GqJEnN-1sZxhXjzIF_05hCS1iE-Au_nAB3ZiU,59150
-easy_encryption_tool-1.1.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-easy_encryption_tool-1.1.3.dist-info/entry_points.txt,sha256=PhqlR4Bl8hLdmVL11hpBv7XBL6oXeOA2fxOg_0PC5R8,62
-easy_encryption_tool-1.1.3.dist-info/top_level.txt,sha256=VrL6mzxpOyPrY3rdPaG8fWebkdOyE2154AoYveQpDio,78
-easy_encryption_tool-1.1.3.dist-info/RECORD,,
+easy_encryption_tool-1.1.4.dist-info/METADATA,sha256=wCPufAes738aGaesLh0wlisWef5U2LEQzzwCU6e8Qsw,59150
+easy_encryption_tool-1.1.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+easy_encryption_tool-1.1.4.dist-info/entry_points.txt,sha256=PhqlR4Bl8hLdmVL11hpBv7XBL6oXeOA2fxOg_0PC5R8,62
+easy_encryption_tool-1.1.4.dist-info/top_level.txt,sha256=VrL6mzxpOyPrY3rdPaG8fWebkdOyE2154AoYveQpDio,78
+easy_encryption_tool-1.1.4.dist-info/RECORD,,
```

