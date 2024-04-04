# Comparing `tmp/crypto_plus-1.0.1.tar.gz` & `tmp/crypto_plus-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_plus-1.0.1.tar", max compression
+gzip compressed data, was "crypto_plus-1.0.2.tar", max compression
```

## Comparing `crypto_plus-1.0.1.tar` & `crypto_plus-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.1/LICENSE
--rw-r--r--   0        0        0     1608 2024-04-04 05:03:14.152968 crypto_plus-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.1/README.md
--rw-r--r--   0        0        0      143 2024-04-04 05:01:15.476028 crypto_plus-1.0.1/src/crypto_plus/__init__.py
--rw-r--r--   0        0        0     7525 2024-04-04 04:57:32.396140 crypto_plus-1.0.1/src/crypto_plus/asymmetric.py
--rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.1/src/crypto_plus/base.py
--rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.1/src/crypto_plus/compatible.py
--rw-r--r--   0        0        0     4940 2024-01-08 14:46:42.082529 crypto_plus-1.0.1/src/crypto_plus/encrypt.py
--rw-r--r--   0        0        0     6077 2024-01-08 14:46:42.082529 crypto_plus-1.0.1/src/crypto_plus/key.py
--rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.1/src/crypto_plus/sign.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1608 2024-04-04 13:52:52.933182 crypto_plus-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.2/README.md
+-rw-r--r--   0        0        0      143 2024-04-04 13:48:03.170202 crypto_plus-1.0.2/src/crypto_plus/__init__.py
+-rw-r--r--   0        0        0     7525 2024-04-04 04:57:32.396140 crypto_plus-1.0.2/src/crypto_plus/asymmetric.py
+-rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.2/src/crypto_plus/base.py
+-rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.2/src/crypto_plus/compatible.py
+-rw-r--r--   0        0        0     5284 2024-04-04 13:45:34.624509 crypto_plus-1.0.2/src/crypto_plus/encrypt.py
+-rw-r--r--   0        0        0     6077 2024-01-08 14:46:42.082529 crypto_plus-1.0.2/src/crypto_plus/key.py
+-rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.2/src/crypto_plus/sign.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.2/PKG-INFO
```

### Comparing `crypto_plus-1.0.1/LICENSE` & `crypto_plus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.1/pyproject.toml` & `crypto_plus-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crypto_plus"
-version = "1.0.1"
+version = "1.0.2"
 description = "A Easy-to-use Crypto Tool"
 readme = "README.md"
 authors = ["wmymz <wmymz@icloud.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.12",
```

### Comparing `crypto_plus-1.0.1/README.md` & `crypto_plus-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.1/src/crypto_plus/asymmetric.py` & `crypto_plus-1.0.2/src/crypto_plus/asymmetric.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.1/src/crypto_plus/compatible.py` & `crypto_plus-1.0.2/src/crypto_plus/compatible.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.1/src/crypto_plus/encrypt.py` & `crypto_plus-1.0.2/src/crypto_plus/encrypt.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,16 +86,23 @@
         for i in range(1 + (len(message) - 1) // max_segment_len):
             # 分段加密
             plaintext_part = message[
                 i * max_segment_len : (i + 1) * max_segment_len
             ]
             pad_len = key.size_in_bytes() - len(plaintext_part) - 3
             # 填充后加密
+            # 生成范围在1到255之间的随机数，确保非零字节
+            rand_pads = bytearray(pad_len)
+            for j in range(pad_len):
+                rand_pads[j] = random.randint(1, 255)
+
+            rand_pads = rand_pads[:pad_len]
             plaintext_part_padding = bytes_to_long(
-                bytes.fromhex(f'0001{"ff" * pad_len}00{plaintext_part.hex()}')
+                # bytes.fromhex(f'0001{"ff" * pad_len}00{plaintext_part.hex()}')
+                bytes.fromhex(f"0002{rand_pads.hex()}00{plaintext_part.hex()}")
             )
             ciphertext_part = _fast_pow(plaintext_part_padding)
 
             # encrypt_data = encrypt_data.to_bytes(1 + encrypt_data.bit_length() // 8)
             ciphertext_part = ciphertext_part.to_bytes(
                 key.public_key().size_in_bytes()
             )
```

### Comparing `crypto_plus-1.0.1/src/crypto_plus/key.py` & `crypto_plus-1.0.2/src/crypto_plus/key.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.1/src/crypto_plus/sign.py` & `crypto_plus-1.0.2/src/crypto_plus/sign.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.1/PKG-INFO` & `crypto_plus-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto_plus
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Easy-to-use Crypto Tool
 License: MIT
 Author: wmymz
 Author-email: wmymz@icloud.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

