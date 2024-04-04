# Comparing `tmp/easy_encryption_tool-1.1.2-py3-none-any.whl.zip` & `tmp/easy_encryption_tool-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 34843 bytes, number of entries: 12
--rw-r--r--  2.0 unx    20027 b- defN 24-Apr-04 14:56 aes_command.py
--rw-r--r--  2.0 unx    12652 b- defN 24-Apr-04 14:56 ecc_command.py
--rw-r--r--  2.0 unx     4111 b- defN 24-Apr-04 14:56 hmac_command.py
--rw-r--r--  2.0 unx     2210 b- defN 24-Apr-04 14:56 main.py
--rw-r--r--  2.0 unx     2675 b- defN 24-Apr-04 14:56 random_str.py
--rw-r--r--  2.0 unx    17736 b- defN 24-Apr-04 14:56 rsa_command.py
--rw-r--r--  2.0 unx      870 b- defN 24-Apr-04 14:19 tool_version.py
--rw-r--r--  2.0 unx    59150 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       78 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      952 b- defN 24-Apr-04 15:07 easy_encryption_tool-1.1.2.dist-info/RECORD
-12 files, 120615 bytes uncompressed, 33259 bytes compressed:  72.4%
+Zip file size: 34736 bytes, number of entries: 12
+-rw-r--r--  2.0 unx    19949 b- defN 24-Apr-04 15:11 aes_command.py
+-rw-r--r--  2.0 unx    12600 b- defN 24-Apr-04 15:09 ecc_command.py
+-rw-r--r--  2.0 unx     4033 b- defN 24-Apr-04 15:09 hmac_command.py
+-rw-r--r--  2.0 unx     2214 b- defN 24-Apr-04 15:09 main.py
+-rw-r--r--  2.0 unx     2655 b- defN 24-Apr-04 15:09 random_str.py
+-rw-r--r--  2.0 unx    17684 b- defN 24-Apr-04 15:09 rsa_command.py
+-rw-r--r--  2.0 unx      844 b- defN 24-Apr-04 15:09 tool_version.py
+-rw-r--r--  2.0 unx    59150 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       78 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      952 b- defN 24-Apr-04 15:11 easy_encryption_tool-1.1.3.dist-info/RECORD
+12 files, 120313 bytes uncompressed, 33152 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: rsa_command.py
 Comment: 
 
 Filename: tool_version.py
 Comment: 
 
-Filename: easy_encryption_tool-1.1.2.dist-info/METADATA
+Filename: easy_encryption_tool-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: easy_encryption_tool-1.1.2.dist-info/WHEEL
+Filename: easy_encryption_tool-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: easy_encryption_tool-1.1.2.dist-info/entry_points.txt
+Filename: easy_encryption_tool-1.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.2.dist-info/top_level.txt
+Filename: easy_encryption_tool-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.1.2.dist-info/RECORD
+Filename: easy_encryption_tool-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aes_command.py

```diff
@@ -9,17 +9,17 @@
 from typing import Tuple
 
 import click
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import padding
 from cryptography.hazmat.primitives.ciphers import algorithms, Cipher, modes
 
-from easy_encryption_tool import common
-from easy_encryption_tool import random_str
-from easy_encryption_tool import command_perf
+import common
+import random_str
+import command_perf
 
 algorithm: str = 'aes'
 
 aes_block_in_bytes = algorithms.AES.block_size // 8
 
 aes_key_len_256: int = 32  # 32字节
 aes_iv_len_128: int = 16  # 16字节
```

## ecc_command.py

```diff
@@ -6,16 +6,16 @@
 import click
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.kdf.hkdf import HKDF
 
-from easy_encryption_tool import command_perf
-from easy_encryption_tool import common
+import command_perf
+import common
 
 ecc_map = {
     ec.SECP256R1().name: ec.SECP256R1,
     ec.SECP384R1().name: ec.SECP384R1,
     ec.SECP521R1().name: ec.SECP521R1,
     ec.SECP256K1().name: ec.SECP256K1,
 }
```

## hmac_command.py

```diff
@@ -2,17 +2,17 @@
 # -*- coding: UTF-8 -*-
 # @Time: 2024-04-02 10:57:19
 import hashlib
 import hmac
 
 import click
 
-from easy_encryption_tool import common
-from easy_encryption_tool import random_str
-from easy_encryption_tool import command_perf
+import command_perf
+import common
+import random_str
 
 hash_maps = {
     hashlib.sha224().name: hashlib.sha384,
     hashlib.sha256().name: hashlib.sha256,
     hashlib.sha384().name: hashlib.sha384,
     hashlib.sha512().name: hashlib.sha512,
     hashlib.sha3_224().name: hashlib.sha3_224,
```

## main.py

```diff
@@ -1,14 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 # @Time: 2024-03-30 15:41:41
 
 import click
 
-from easy_encryption_tool import aes_command, ecc_command, hmac_command, random_str, rsa_command, tool_version
+import aes_command
+import ecc_command
+import hmac_command
+import random_str
+import rsa_command
+import tool_version
 
 """
 name (str): 命令组的名称。如果未提供，将使用装饰的函数的名称。
 
 commands (dict): 一个字典，其中键是命令名称，值是命令函数。这允许你在装饰器内部直接定义命令，而不是通过单独的 @click.command() 装饰器。
 
 invoke_without_command (bool): 如果为 True，则在没有提供子命令的情况下调用组时，将调用组函数本身。
```

## random_str.py

```diff
@@ -3,15 +3,16 @@
 # @Time: 2024-04-01 09:04:43
 import random
 import string
 import sys
 
 import click
 
-from easy_encryption_tool import command_perf, common
+import command_perf
+import common
 
 special_characters = '&=!@#$%^*()_+`'
 characters: str = string.ascii_lowercase + \
                   string.ascii_uppercase + \
                   string.digits + \
                   special_characters
```

## rsa_command.py

```diff
@@ -4,16 +4,16 @@
 import base64
 
 import click
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 
-from easy_encryption_tool import command_perf
-from easy_encryption_tool import common
+import command_perf
+import common
 
 rsa_key_size = ['2048', '3072', '4096']
 rsa_encryption_mode = ['oaep', 'pkcs1v15']
 rsa_sign_mode = ['pss', 'pkcs1v15']
 
 rsa_hash_map = {
     hashes.SHA256().name: hashes.SHA256,
```

## tool_version.py

```diff
@@ -4,15 +4,15 @@
 
 import platform
 import sys
 from typing import Dict
 
 import click
 
-from easy_encryption_tool import command_perf
+import command_perf
 
 
 def sys_info() -> Dict[str, str]:
     return {
         'PythonVersion': sys.version,
         'ApiVersion': sys.api_version,
         'OSPlatform': sys.platform,
```

## Comparing `easy_encryption_tool-1.1.2.dist-info/METADATA` & `easy_encryption_tool-1.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-encryption-tool
-Version: 1.1.2
+Version: 1.1.3
 Home-page: https://cloud.tencent.com/developer/article/2155922
 Author: bowenerchen
 Author-email: bowener.chen@gmail.com
 License: MIT
 Keywords: encryption cli tool security aes hmac ecc rsa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `easy_encryption_tool-1.1.2.dist-info/RECORD` & `easy_encryption_tool-1.1.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-aes_command.py,sha256=CbhUaS5d_5pRnsaZV7VSi6CAsAkzLP1k2ZUwcBWgCuc,20027
-ecc_command.py,sha256=g76LOqS-UILqXSgFZhqw_1qAXpXDZRUNslcmAQHmkpk,12652
-hmac_command.py,sha256=mQaZ9dDsh3q4KNEhkyht8bVPcT5LD0Oq8b2tEpqxWKg,4111
-main.py,sha256=e3YHOsFViRrS_TMd6Pv8wLu4EaZO4GFvuUPnDV0zLs8,2210
-random_str.py,sha256=Mz8QkU8w-TrKWxLKhevXtic9_EPryeYlJcrEhXaQcVA,2675
-rsa_command.py,sha256=QsAJUo69Yo8EpZ3mbu4mbIR50NGPoRXfzZPtHJAOIGg,17736
-tool_version.py,sha256=Gz2mCkhX1Ztrpr_TaTBkyVWs9Yk3gX8QxxlgkB4ga0A,870
-easy_encryption_tool-1.1.2.dist-info/METADATA,sha256=VWGGhemdYUuMaU1RJZim6gvetKC31XSsfO-jr5nU8ac,59150
-easy_encryption_tool-1.1.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-easy_encryption_tool-1.1.2.dist-info/entry_points.txt,sha256=PhqlR4Bl8hLdmVL11hpBv7XBL6oXeOA2fxOg_0PC5R8,62
-easy_encryption_tool-1.1.2.dist-info/top_level.txt,sha256=VrL6mzxpOyPrY3rdPaG8fWebkdOyE2154AoYveQpDio,78
-easy_encryption_tool-1.1.2.dist-info/RECORD,,
+aes_command.py,sha256=mtlCkFOf9z22BjE0gEC1pj0zIF5RrsmBqIongBAmar4,19949
+ecc_command.py,sha256=HMFZpNOzTBzYrKlidZAi759e_71fPJN2vZfoahlamxY,12600
+hmac_command.py,sha256=qEF1MM7nIo8eq0W60IwR9Wz8NmHlNK7l22gLSOaEwUg,4033
+main.py,sha256=JbIKp9BbnNjN_rFiQTSHAMfo13S9_qp32W74-dES5r4,2214
+random_str.py,sha256=_pwixdXMppOEJCfXlATaXFHqLzhc6wVVyo_ezVCU1vY,2655
+rsa_command.py,sha256=Dlc4PQagXbWH1PsgfXuMh5_Kc0aQc4p3wDhz28cFUus,17684
+tool_version.py,sha256=2XtagEC0RJUr6AGU3cp3UG_HgInbfSNylcraubSgKis,844
+easy_encryption_tool-1.1.3.dist-info/METADATA,sha256=wJd0N-GqJEnN-1sZxhXjzIF_05hCS1iE-Au_nAB3ZiU,59150
+easy_encryption_tool-1.1.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+easy_encryption_tool-1.1.3.dist-info/entry_points.txt,sha256=PhqlR4Bl8hLdmVL11hpBv7XBL6oXeOA2fxOg_0PC5R8,62
+easy_encryption_tool-1.1.3.dist-info/top_level.txt,sha256=VrL6mzxpOyPrY3rdPaG8fWebkdOyE2154AoYveQpDio,78
+easy_encryption_tool-1.1.3.dist-info/RECORD,,
```

