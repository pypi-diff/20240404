# Comparing `tmp/ft_jwt-0.0.5.tar.gz` & `tmp/ft_jwt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_jwt-0.0.5.tar", last modified: Thu Apr  4 08:14:53 2024, max compression
+gzip compressed data, was "ft_jwt-0.0.6.tar", last modified: Thu Apr  4 14:02:02 2024, max compression
```

## Comparing `ft_jwt-0.0.5.tar` & `ft_jwt-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 08:14:53.039876 ft_jwt-0.0.5/
--rw-r--r--   0 minthe     (501) staff       (20)     1063 2024-04-04 07:43:46.000000 ft_jwt-0.0.5/LICENSE
--rw-r--r--   0 minthe     (501) staff       (20)     1592 2024-04-04 08:14:53.037807 ft_jwt-0.0.5/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)     1074 2024-04-04 07:56:40.000000 ft_jwt-0.0.5/README.md
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 08:14:53.033465 ft_jwt-0.0.5/ft_jwt/
--rw-r--r--   0 minthe     (501) staff       (20)        0 2024-04-04 07:32:01.000000 ft_jwt-0.0.5/ft_jwt/__init__.py
--rw-r--r--   0 minthe     (501) staff       (20)     3145 2024-04-04 07:24:14.000000 ft_jwt-0.0.5/ft_jwt/jwt.py
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 08:14:53.037049 ft_jwt-0.0.5/ft_jwt.egg-info/
--rw-r--r--   0 minthe     (501) staff       (20)     1592 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)      179 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 minthe     (501) staff       (20)        1 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 minthe     (501) staff       (20)        7 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 minthe     (501) staff       (20)       38 2024-04-04 08:14:53.040025 ft_jwt-0.0.5/setup.cfg
--rw-r--r--   0 minthe     (501) staff       (20)      675 2024-04-04 08:14:35.000000 ft_jwt-0.0.5/setup.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 12:46:38.000000 ft_jwt-0.0.6/LICENSE
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1797 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1279 2024-04-04 12:55:49.000000 ft_jwt-0.0.6/README.md
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 12:45:04.000000 ft_jwt-0.0.6/ft_jwt/__init__.py
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 12:45:41.000000 ft_jwt-0.0.6/ft_jwt/ft_jwt.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1797 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/setup.cfg
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      675 2024-04-04 12:51:38.000000 ft_jwt-0.0.6/setup.py
```

### Comparing `ft_jwt-0.0.5/LICENSE` & `ft_jwt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.5/PKG-INFO` & `ft_jwt-0.0.6/ft_jwt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ft_jwt
-Version: 0.0.5
+Name: ft-jwt
+Version: 0.0.6
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Home-page: https://github.com/minthe/ft_jwt
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,34 +27,45 @@
 You can install the package via pip:
 
 ```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from ft_jwt import JWT
+from ft_jwt import FT_JWT
 
 # Create a JWT instance with your secret key
+
 secret_key = 'your_secret_key'
-jwt = JWT(secret_key)
+ftjwt = FT_JWT(secret_key)
 
 # Generate a token for a user
+
 sub = '1'
 token = jwt.createToken(sub)
 
 # Validate a token
-is_valid, message = jwt.validateToken(token)
+
+is_valid, message = ftjwt.validateToken(token)
 if is_valid:
     print('Token is valid')
 else:
     print(f'Token is invalid: {message}')
 
 # Get the user ID from a token
-user_id = jwt.getUserId(token)
+
+user_id = ftjwt.getUserId(token)
 print(f'User ID: {sub}')
+
+# Use the decorator to validate against a JWT for a protected route
+
+@ftjwt.token_required
+def protected_route():
+    # This function will be executed only if the token is valid
+    # ...
 ```
 
 # Contributing
 Contributions are welcome! Please open an issue or submit a pull request.
 
 # License
 This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.0.5/README.md` & `ft_jwt-0.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -13,34 +13,45 @@
 You can install the package via pip:
 
 ```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from ft_jwt import JWT
+from ft_jwt import FT_JWT
 
 # Create a JWT instance with your secret key
+
 secret_key = 'your_secret_key'
-jwt = JWT(secret_key)
+ftjwt = FT_JWT(secret_key)
 
 # Generate a token for a user
+
 sub = '1'
 token = jwt.createToken(sub)
 
 # Validate a token
-is_valid, message = jwt.validateToken(token)
+
+is_valid, message = ftjwt.validateToken(token)
 if is_valid:
     print('Token is valid')
 else:
     print(f'Token is invalid: {message}')
 
 # Get the user ID from a token
-user_id = jwt.getUserId(token)
+
+user_id = ftjwt.getUserId(token)
 print(f'User ID: {sub}')
+
+# Use the decorator to validate against a JWT for a protected route
+
+@ftjwt.token_required
+def protected_route():
+    # This function will be executed only if the token is valid
+    # ...
 ```
 
 # Contributing
 Contributions are welcome! Please open an issue or submit a pull request.
 
 # License
 This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.0.5/ft_jwt/jwt.py` & `ft_jwt-0.0.6/ft_jwt/ft_jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib, base64, hmac, json
 from datetime import datetime, timedelta
 from django.http import HttpResponse
 from functools import wraps
 
-class JWT:
+class FT_JWT:
 
 	def __init__(self, secret):
 		self.secret = secret
 
 	def base64url_encode(self, input):
 		return base64.urlsafe_b64encode(input).decode('utf-8').rstrip('=')
```

### Comparing `ft_jwt-0.0.5/ft_jwt.egg-info/PKG-INFO` & `ft_jwt-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Home-page: https://github.com/minthe/ft_jwt
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,34 +27,45 @@
 You can install the package via pip:
 
 ```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from ft_jwt import JWT
+from ft_jwt import FT_JWT
 
 # Create a JWT instance with your secret key
+
 secret_key = 'your_secret_key'
-jwt = JWT(secret_key)
+ftjwt = FT_JWT(secret_key)
 
 # Generate a token for a user
+
 sub = '1'
 token = jwt.createToken(sub)
 
 # Validate a token
-is_valid, message = jwt.validateToken(token)
+
+is_valid, message = ftjwt.validateToken(token)
 if is_valid:
     print('Token is valid')
 else:
     print(f'Token is invalid: {message}')
 
 # Get the user ID from a token
-user_id = jwt.getUserId(token)
+
+user_id = ftjwt.getUserId(token)
 print(f'User ID: {sub}')
+
+# Use the decorator to validate against a JWT for a protected route
+
+@ftjwt.token_required
+def protected_route():
+    # This function will be executed only if the token is valid
+    # ...
 ```
 
 # Contributing
 Contributions are welcome! Please open an issue or submit a pull request.
 
 # License
 This project is licensed under the MIT License.
```

### Comparing `ft_jwt-0.0.5/setup.py` & `ft_jwt-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.0.5",
+	version="0.0.6",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/minthe/ft_jwt",
 	packages=setuptools.find_packages(),
```

