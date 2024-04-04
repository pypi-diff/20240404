# Comparing `tmp/secret_key_database-0.1.1.tar.gz` & `tmp/secret_key_database-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_key_database-0.1.1.tar", last modified: Thu Apr  4 08:42:47 2024, max compression
+gzip compressed data, was "secret_key_database-0.1.2.tar", last modified: Thu Apr  4 17:32:53 2024, max compression
```

## Comparing `secret_key_database-0.1.1.tar` & `secret_key_database-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:42:47.620575 secret_key_database-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-04 08:42:47.620575 secret_key_database-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:42:47.620575 secret_key_database-0.1.1/secret_key_database/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/secret_key_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/secret_key_database/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/secret_key_database/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/secret_key_database/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:42:47.620575 secret_key_database-0.1.1/secret_key_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-04 08:42:47.000000 secret_key_database-0.1.1/secret_key_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 08:42:47.000000 secret_key_database-0.1.1/secret_key_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:42:47.000000 secret_key_database-0.1.1/secret_key_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 08:42:47.000000 secret_key_database-0.1.1/secret_key_database.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 08:42:47.000000 secret_key_database-0.1.1/secret_key_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 08:42:47.620575 secret_key_database-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:42:47.620575 secret_key_database-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-04-04 08:42:41.000000 secret_key_database-0.1.1/tests/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:32:53.229721 secret_key_database-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-04 17:32:53.229721 secret_key_database-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:32:53.229721 secret_key_database-0.1.2/secret_key_database/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/secret_key_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/secret_key_database/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/secret_key_database/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/secret_key_database/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:32:53.229721 secret_key_database-0.1.2/secret_key_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-04 17:32:53.000000 secret_key_database-0.1.2/secret_key_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 17:32:53.000000 secret_key_database-0.1.2/secret_key_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:32:53.000000 secret_key_database-0.1.2/secret_key_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 17:32:53.000000 secret_key_database-0.1.2/secret_key_database.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 17:32:53.000000 secret_key_database-0.1.2/secret_key_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 17:32:53.229721 secret_key_database-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:32:53.229721 secret_key_database-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-04-04 17:32:50.000000 secret_key_database-0.1.2/tests/test_encryption.py
```

### Comparing `secret_key_database-0.1.1/PKG-INFO` & `secret_key_database-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: secret_key_database
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python package for encrypting and decrypting secret keys.
 Home-page: https://github.com/RichieHakim/secret_key_database
 Author: Richard Hakim
 License: LICENSE
 Keywords: cryptography,encryption,security,secret_key_database
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 Requires-Dist: pytest
 Requires-Dist: hypothesis
 
 # secret_key_database
-This is a very simple library to encrypt and store secret keys (or any text) locally.
-<br>
+This is a very simple library to encrypt and store secret keys (or any text)
+locally. <br>
 The keys are stored in a local sqlite database. The keys are encrypted using
 AES-GCM. That's it. In theory, the database file can be shared publicly since
-they are encrypted and require a password to decrypt, but it's best to keep it
-private.
-<br>
+the keys are encrypted and require a password to decrypt, but it's best to keep
+it private. <br>
 This approach works great when:
 - Number of keys is small
 - The keys are not very sensitive (e.g. low risk API keys)
 - You store the database in a semi-secure location (computer with a password,
   private repository, etc.)
 - You don't want to use an external or cloud service as a key/password manager
 - You need a simple API to store and retrieve keys
@@ -41,21 +40,21 @@
 
 ## Demo
 ```
 import secret_key_database as skd
 
 # Create a new database
 path_db = 'path/to/database.db'
-db = skd.Database(path_db)
+db = skd.database.create_database(path_db)
 
 # Add a new key
-skd.database.append_encrypted_key_to_database(
+skd.user.add_key_to_database(
     path_db=path_db,
     name='key_name',
 )
 
 # Get a key
-key = skd.database.get_decrypted_key_from_database(
+key = skd.user.get_key_from_database(
     path_db=path_db,
     name='key_name',
 )
 ```
```

### Comparing `secret_key_database-0.1.1/README.md` & `secret_key_database-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # secret_key_database
-This is a very simple library to encrypt and store secret keys (or any text) locally.
-<br>
+This is a very simple library to encrypt and store secret keys (or any text)
+locally. <br>
 The keys are stored in a local sqlite database. The keys are encrypted using
 AES-GCM. That's it. In theory, the database file can be shared publicly since
-they are encrypted and require a password to decrypt, but it's best to keep it
-private.
-<br>
+the keys are encrypted and require a password to decrypt, but it's best to keep
+it private. <br>
 This approach works great when:
 - Number of keys is small
 - The keys are not very sensitive (e.g. low risk API keys)
 - You store the database in a semi-secure location (computer with a password,
   private repository, etc.)
 - You don't want to use an external or cloud service as a key/password manager
 - You need a simple API to store and retrieve keys
@@ -28,21 +27,21 @@
 
 ## Demo
 ```
 import secret_key_database as skd
 
 # Create a new database
 path_db = 'path/to/database.db'
-db = skd.Database(path_db)
+db = skd.database.create_database(path_db)
 
 # Add a new key
-skd.database.append_encrypted_key_to_database(
+skd.user.add_key_to_database(
     path_db=path_db,
     name='key_name',
 )
 
 # Get a key
-key = skd.database.get_decrypted_key_from_database(
+key = skd.user.get_key_from_database(
     path_db=path_db,
     name='key_name',
 )
 ```
```

### Comparing `secret_key_database-0.1.1/secret_key_database/database.py` & `secret_key_database-0.1.2/secret_key_database/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,18 @@
             The name of the encrypted key. Must be provided if ID is not
             provided. Defaults to None.
         id (str, optional): 
             The unique ID of the encrypted key. Must be provided if name is not
             provided. Supersedes name if both are provided. Defaults to None.
     """
     _assert_type(path_db, str)  ## Check types: str
-    [_assert_type(var, str) for var in [name, id]]  ## Check types: str
+    if name is not None:
+        _assert_type(name, str)
+    if id is not None:
+        _assert_type(id, str)
 
     # Delete the encrypted key from the database
     with sqlite3.connect(path_db) as conn:
         if id is not None:
             query = f"DELETE FROM encrypted_keys WHERE id = '{id}'"
         elif name is not None:
             query = f"DELETE FROM encrypted_keys WHERE name = '{name}'"
```

### Comparing `secret_key_database-0.1.1/secret_key_database/encryption.py` & `secret_key_database-0.1.2/secret_key_database/encryption.py`

 * *Files identical despite different names*

### Comparing `secret_key_database-0.1.1/secret_key_database/user.py` & `secret_key_database-0.1.2/secret_key_database/user.py`

 * *Files identical despite different names*

### Comparing `secret_key_database-0.1.1/secret_key_database.egg-info/PKG-INFO` & `secret_key_database-0.1.2/secret_key_database.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: secret_key_database
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python package for encrypting and decrypting secret keys.
 Home-page: https://github.com/RichieHakim/secret_key_database
 Author: Richard Hakim
 License: LICENSE
 Keywords: cryptography,encryption,security,secret_key_database
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 Requires-Dist: pytest
 Requires-Dist: hypothesis
 
 # secret_key_database
-This is a very simple library to encrypt and store secret keys (or any text) locally.
-<br>
+This is a very simple library to encrypt and store secret keys (or any text)
+locally. <br>
 The keys are stored in a local sqlite database. The keys are encrypted using
 AES-GCM. That's it. In theory, the database file can be shared publicly since
-they are encrypted and require a password to decrypt, but it's best to keep it
-private.
-<br>
+the keys are encrypted and require a password to decrypt, but it's best to keep
+it private. <br>
 This approach works great when:
 - Number of keys is small
 - The keys are not very sensitive (e.g. low risk API keys)
 - You store the database in a semi-secure location (computer with a password,
   private repository, etc.)
 - You don't want to use an external or cloud service as a key/password manager
 - You need a simple API to store and retrieve keys
@@ -41,21 +40,21 @@
 
 ## Demo
 ```
 import secret_key_database as skd
 
 # Create a new database
 path_db = 'path/to/database.db'
-db = skd.Database(path_db)
+db = skd.database.create_database(path_db)
 
 # Add a new key
-skd.database.append_encrypted_key_to_database(
+skd.user.add_key_to_database(
     path_db=path_db,
     name='key_name',
 )
 
 # Get a key
-key = skd.database.get_decrypted_key_from_database(
+key = skd.user.get_key_from_database(
     path_db=path_db,
     name='key_name',
 )
 ```
```

### Comparing `secret_key_database-0.1.1/setup.py` & `secret_key_database-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `secret_key_database-0.1.1/tests/test_encryption.py` & `secret_key_database-0.1.2/tests/test_encryption.py`

 * *Files identical despite different names*

