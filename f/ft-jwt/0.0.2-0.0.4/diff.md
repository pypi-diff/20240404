# Comparing `tmp/ft_jwt-0.0.2.tar.gz` & `tmp/ft_jwt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_jwt-0.0.2.tar", last modified: Thu Apr  4 07:50:31 2024, max compression
+gzip compressed data, was "ft_jwt-0.0.4.tar", last modified: Thu Apr  4 07:57:27 2024, max compression
```

## Comparing `ft_jwt-0.0.2.tar` & `ft_jwt-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:50:31.730228 ft_jwt-0.0.2/
--rw-r--r--   0 minthe     (501) staff       (20)     1063 2024-04-04 07:43:46.000000 ft_jwt-0.0.2/LICENSE
--rw-r--r--   0 minthe     (501) staff       (20)     1560 2024-04-04 07:50:31.728231 ft_jwt-0.0.2/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)     1086 2024-04-04 07:49:39.000000 ft_jwt-0.0.2/README.md
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:50:31.724179 ft_jwt-0.0.2/ft_jwt/
--rw-r--r--   0 minthe     (501) staff       (20)        0 2024-04-04 07:32:01.000000 ft_jwt-0.0.2/ft_jwt/__init__.py
--rw-r--r--   0 minthe     (501) staff       (20)     3145 2024-04-04 07:24:14.000000 ft_jwt-0.0.2/ft_jwt/jwt.py
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:50:31.727399 ft_jwt-0.0.2/ft_jwt.egg-info/
--rw-r--r--   0 minthe     (501) staff       (20)     1560 2024-04-04 07:50:31.000000 ft_jwt-0.0.2/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)      179 2024-04-04 07:50:31.000000 ft_jwt-0.0.2/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 minthe     (501) staff       (20)        1 2024-04-04 07:50:31.000000 ft_jwt-0.0.2/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 minthe     (501) staff       (20)        7 2024-04-04 07:50:31.000000 ft_jwt-0.0.2/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 minthe     (501) staff       (20)       38 2024-04-04 07:50:31.730442 ft_jwt-0.0.2/setup.cfg
--rw-r--r--   0 minthe     (501) staff       (20)      634 2024-04-04 07:50:07.000000 ft_jwt-0.0.2/setup.py
+drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:57:27.117657 ft_jwt-0.0.4/
+-rw-r--r--   0 minthe     (501) staff       (20)     1063 2024-04-04 07:43:46.000000 ft_jwt-0.0.4/LICENSE
+-rw-r--r--   0 minthe     (501) staff       (20)     1548 2024-04-04 07:57:27.115499 ft_jwt-0.0.4/PKG-INFO
+-rw-r--r--   0 minthe     (501) staff       (20)     1074 2024-04-04 07:56:40.000000 ft_jwt-0.0.4/README.md
+drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:57:27.109885 ft_jwt-0.0.4/ft_jwt/
+-rw-r--r--   0 minthe     (501) staff       (20)        0 2024-04-04 07:32:01.000000 ft_jwt-0.0.4/ft_jwt/__init__.py
+-rw-r--r--   0 minthe     (501) staff       (20)     3145 2024-04-04 07:24:14.000000 ft_jwt-0.0.4/ft_jwt/jwt.py
+drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:57:27.114714 ft_jwt-0.0.4/ft_jwt.egg-info/
+-rw-r--r--   0 minthe     (501) staff       (20)     1548 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 minthe     (501) staff       (20)      179 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 minthe     (501) staff       (20)        1 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 minthe     (501) staff       (20)        7 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 minthe     (501) staff       (20)       38 2024-04-04 07:57:27.117821 ft_jwt-0.0.4/setup.cfg
+-rw-r--r--   0 minthe     (501) staff       (20)      634 2024-04-04 07:57:20.000000 ft_jwt-0.0.4/setup.py
```

### Comparing `ft_jwt-0.0.2/LICENSE` & `ft_jwt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.2/PKG-INFO` & `ft_jwt-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.2
+Version: 0.0.4
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,45 +15,45 @@
 
 A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 
 ## Features
 
 - Generate JWT tokens with customizable expiration times
 - Validate JWT tokens and verify their integrity using a symmetric secret key and HMAC-SHA256
-- Extract user information (such as user ID) from JWT tokens
+- Extract user information (such as user ID 'sub') from JWT tokens
 
 ## Installation
 
 You can install the package via pip:
 
-```pip install my_jwt```
+```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from my_jwt import JWT
+from ft_jwt import JWT
 
 # Create a JWT instance with your secret key
 secret_key = 'your_secret_key'
 jwt = JWT(secret_key)
 
 # Generate a token for a user
-user_id = 'user123'
-token = jwt.createToken(user_id)
+sub = '1'
+token = jwt.createToken(sub)
 
 # Validate a token
 is_valid, message = jwt.validateToken(token)
 if is_valid:
     print('Token is valid')
 else:
     print(f'Token is invalid: {message}')
 
 # Get the user ID from a token
 user_id = jwt.getUserId(token)
-print(f'User ID: {user_id}')
+print(f'User ID: {sub}')
 ```
 
 # Contributing
 Contributions are welcome! Please open an issue or submit a pull request.
 
 # License
 This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.0.2/README.md` & `ft_jwt-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 
 A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 
 ## Features
 
 - Generate JWT tokens with customizable expiration times
 - Validate JWT tokens and verify their integrity using a symmetric secret key and HMAC-SHA256
-- Extract user information (such as user ID) from JWT tokens
+- Extract user information (such as user ID 'sub') from JWT tokens
 
 ## Installation
 
 You can install the package via pip:
 
-```pip install my_jwt```
+```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from my_jwt import JWT
+from ft_jwt import JWT
 
 # Create a JWT instance with your secret key
 secret_key = 'your_secret_key'
 jwt = JWT(secret_key)
 
 # Generate a token for a user
-user_id = 'user123'
-token = jwt.createToken(user_id)
+sub = '1'
+token = jwt.createToken(sub)
 
 # Validate a token
 is_valid, message = jwt.validateToken(token)
 if is_valid:
     print('Token is valid')
 else:
     print(f'Token is invalid: {message}')
 
 # Get the user ID from a token
 user_id = jwt.getUserId(token)
-print(f'User ID: {user_id}')
+print(f'User ID: {sub}')
 ```
 
 # Contributing
 Contributions are welcome! Please open an issue or submit a pull request.
 
 # License
 This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.0.2/ft_jwt/jwt.py` & `ft_jwt-0.0.4/ft_jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.2/ft_jwt.egg-info/PKG-INFO` & `ft_jwt-0.0.4/ft_jwt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.2
+Version: 0.0.4
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,45 +15,45 @@
 
 A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 
 ## Features
 
 - Generate JWT tokens with customizable expiration times
 - Validate JWT tokens and verify their integrity using a symmetric secret key and HMAC-SHA256
-- Extract user information (such as user ID) from JWT tokens
+- Extract user information (such as user ID 'sub') from JWT tokens
 
 ## Installation
 
 You can install the package via pip:
 
-```pip install my_jwt```
+```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from my_jwt import JWT
+from ft_jwt import JWT
 
 # Create a JWT instance with your secret key
 secret_key = 'your_secret_key'
 jwt = JWT(secret_key)
 
 # Generate a token for a user
-user_id = 'user123'
-token = jwt.createToken(user_id)
+sub = '1'
+token = jwt.createToken(sub)
 
 # Validate a token
 is_valid, message = jwt.validateToken(token)
 if is_valid:
     print('Token is valid')
 else:
     print(f'Token is invalid: {message}')
 
 # Get the user ID from a token
 user_id = jwt.getUserId(token)
-print(f'User ID: {user_id}')
+print(f'User ID: {sub}')
 ```
 
 # Contributing
 Contributions are welcome! Please open an issue or submit a pull request.
 
 # License
 This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.0.2/setup.py` & `ft_jwt-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.0.2",
+	version="0.0.4",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	packages=setuptools.find_packages(),
 	classifiers=[
```

