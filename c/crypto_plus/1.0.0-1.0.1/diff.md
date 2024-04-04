# Comparing `tmp/crypto_plus-1.0.0.tar.gz` & `tmp/crypto_plus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto_plus-1.0.0.tar", max compression
+gzip compressed data, was "crypto_plus-1.0.1.tar", max compression
```

## Comparing `crypto_plus-1.0.0.tar` & `crypto_plus-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.0/LICENSE
--rw-r--r--   0        0        0     1608 2024-02-17 15:08:01.020478 crypto_plus-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.0/README.md
--rw-r--r--   0        0        0      143 2024-02-17 14:52:13.394187 crypto_plus-1.0.0/src/crypto_plus/__init__.py
--rw-r--r--   0        0        0     7079 2024-01-08 14:46:42.081232 crypto_plus-1.0.0/src/crypto_plus/asymmetric.py
--rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.0/src/crypto_plus/base.py
--rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.0/src/crypto_plus/compatible.py
--rw-r--r--   0        0        0     4940 2024-01-08 14:46:42.082529 crypto_plus-1.0.0/src/crypto_plus/encrypt.py
--rw-r--r--   0        0        0     6077 2024-01-08 14:46:42.082529 crypto_plus-1.0.0/src/crypto_plus/key.py
--rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.0/src/crypto_plus/sign.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-08 14:46:42.078674 crypto_plus-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1608 2024-04-04 05:03:14.152968 crypto_plus-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      955 2024-01-08 14:46:42.078674 crypto_plus-1.0.1/README.md
+-rw-r--r--   0        0        0      143 2024-04-04 05:01:15.476028 crypto_plus-1.0.1/src/crypto_plus/__init__.py
+-rw-r--r--   0        0        0     7525 2024-04-04 04:57:32.396140 crypto_plus-1.0.1/src/crypto_plus/asymmetric.py
+-rw-r--r--   0        0        0      136 2024-01-08 14:46:42.081232 crypto_plus-1.0.1/src/crypto_plus/base.py
+-rw-r--r--   0        0        0     2705 2024-01-31 06:29:44.820443 crypto_plus-1.0.1/src/crypto_plus/compatible.py
+-rw-r--r--   0        0        0     4940 2024-01-08 14:46:42.082529 crypto_plus-1.0.1/src/crypto_plus/encrypt.py
+-rw-r--r--   0        0        0     6077 2024-01-08 14:46:42.082529 crypto_plus-1.0.1/src/crypto_plus/key.py
+-rw-r--r--   0        0        0     2813 2024-01-08 14:46:42.082529 crypto_plus-1.0.1/src/crypto_plus/sign.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 crypto_plus-1.0.1/PKG-INFO
```

### Comparing `crypto_plus-1.0.0/LICENSE` & `crypto_plus-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.0/pyproject.toml` & `crypto_plus-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crypto_plus"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Easy-to-use Crypto Tool"
 readme = "README.md"
 authors = ["wmymz <wmymz@icloud.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.12",
```

### Comparing `crypto_plus-1.0.0/README.md` & `crypto_plus-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.0/src/crypto_plus/asymmetric.py` & `crypto_plus-1.0.1/src/crypto_plus/asymmetric.py`

 * *Files 7% similar despite different names*

```diff
@@ -176,14 +176,27 @@
         builder = builder.serial_number(random_serial_number())
         builder = builder.public_key(self.raw_public_key)
         certificate = builder.sign(
             private_key=self.raw_private_key, algorithm=hashes.SHA256()
         )
         return certificate.public_bytes(serialization.Encoding.PEM)
 
+    # 非常规方法
+    def encrypt_by_private_key(self, message: bytes) -> bytes:
+        if not message:
+            return b""
+        if not self.private_key:
+            raise Exception("私钥缺失")
+        return encrypt_by_key(self.private_key, message)
+
+    def decrypt_by_public_key(self, message: bytes) -> bytes:
+        if not message:
+            return b""
+        return decrypt_by_key(self.public_key, message)
+
     # 常规方法
     def encrypt(self, message: bytes) -> bytes:
         if not message:
             return b""
         return encrypt_by_key(self.public_key, message)
 
     def decrypt(self, message: bytes) -> bytes:
```

### Comparing `crypto_plus-1.0.0/src/crypto_plus/compatible.py` & `crypto_plus-1.0.1/src/crypto_plus/compatible.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.0/src/crypto_plus/encrypt.py` & `crypto_plus-1.0.1/src/crypto_plus/encrypt.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.0/src/crypto_plus/key.py` & `crypto_plus-1.0.1/src/crypto_plus/key.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.0/src/crypto_plus/sign.py` & `crypto_plus-1.0.1/src/crypto_plus/sign.py`

 * *Files identical despite different names*

### Comparing `crypto_plus-1.0.0/PKG-INFO` & `crypto_plus-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto_plus
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Easy-to-use Crypto Tool
 License: MIT
 Author: wmymz
 Author-email: wmymz@icloud.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

