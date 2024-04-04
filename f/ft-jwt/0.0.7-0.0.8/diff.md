# Comparing `tmp/ft_jwt-0.0.7.tar.gz` & `tmp/ft_jwt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_jwt-0.0.7.tar", last modified: Thu Apr  4 14:05:20 2024, max compression
+gzip compressed data, was "ft_jwt-0.0.8.tar", last modified: Thu Apr  4 15:38:36 2024, max compression
```

## Comparing `ft_jwt-0.0.7.tar` & `ft_jwt-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 12:46:38.000000 ft_jwt-0.0.7/LICENSE
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1845 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1279 2024-04-04 12:55:49.000000 ft_jwt-0.0.7/README.md
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 12:45:04.000000 ft_jwt-0.0.7/ft_jwt/__init__.py
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 12:45:41.000000 ft_jwt-0.0.7/ft_jwt/ft_jwt.py
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1845 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/setup.cfg
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      723 2024-04-04 14:05:16.000000 ft_jwt-0.0.7/setup.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 14:17:44.000000 ft_jwt-0.0.8/LICENSE
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1852 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1286 2024-04-04 15:37:53.000000 ft_jwt-0.0.8/README.md
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/ft_jwt/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:17:44.000000 ft_jwt-0.0.8/ft_jwt/__init__.py
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 14:17:44.000000 ft_jwt-0.0.8/ft_jwt/ft_jwt.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/ft_jwt.egg-info/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1852 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 15:38:35.000000 ft_jwt-0.0.8/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 15:38:36.000000 ft_jwt-0.0.8/setup.cfg
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      723 2024-04-04 15:38:05.000000 ft_jwt-0.0.8/setup.py
```

### Comparing `ft_jwt-0.0.7/LICENSE` & `ft_jwt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.7/PKG-INFO` & `ft_jwt-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Home-page: https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 You can install the package via pip:
 
 ```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from ft_jwt import FT_JWT
+from ft_jwt.ft_jwt import FT_JWT
 
 # Create a JWT instance with your secret key
 
 secret_key = 'your_secret_key'
 ftjwt = FT_JWT(secret_key)
 
 # Generate a token for a user
```

### Comparing `ft_jwt-0.0.7/README.md` & `ft_jwt-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 You can install the package via pip:
 
 ```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from ft_jwt import FT_JWT
+from ft_jwt.ft_jwt import FT_JWT
 
 # Create a JWT instance with your secret key
 
 secret_key = 'your_secret_key'
 ftjwt = FT_JWT(secret_key)
 
 # Generate a token for a user
```

### Comparing `ft_jwt-0.0.7/ft_jwt/ft_jwt.py` & `ft_jwt-0.0.8/ft_jwt/ft_jwt.py`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.7/ft_jwt.egg-info/PKG-INFO` & `ft_jwt-0.0.8/ft_jwt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft-jwt
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
 Home-page: https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,15 +27,15 @@
 You can install the package via pip:
 
 ```pip install ft_jwt```
 
 ## Usage
 
 ```python
-from ft_jwt import FT_JWT
+from ft_jwt.ft_jwt import FT_JWT
 
 # Create a JWT instance with your secret key
 
 secret_key = 'your_secret_key'
 ftjwt = FT_JWT(secret_key)
 
 # Generate a token for a user
```

### Comparing `ft_jwt-0.0.7/setup.py` & `ft_jwt-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.0.7",
+	version="0.0.8",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py",
 	packages=setuptools.find_packages(),
```

