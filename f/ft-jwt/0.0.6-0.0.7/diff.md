# Comparing `tmp/ft_jwt-0.0.6.tar.gz` & `tmp/ft_jwt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_jwt-0.0.6.tar", last modified: Thu Apr  4 14:02:02 2024, max compression
+gzip compressed data, was "ft_jwt-0.0.7.tar", last modified: Thu Apr  4 14:05:20 2024, max compression
```

## Comparing `ft_jwt-0.0.6.tar` & `ft_jwt-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 12:46:38.000000 ft_jwt-0.0.6/LICENSE
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1797 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1279 2024-04-04 12:55:49.000000 ft_jwt-0.0.6/README.md
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 12:45:04.000000 ft_jwt-0.0.6/ft_jwt/__init__.py
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 12:45:41.000000 ft_jwt-0.0.6/ft_jwt/ft_jwt.py
-drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1797 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 14:02:02.000000 ft_jwt-0.0.6/setup.cfg
--rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      675 2024-04-04 12:51:38.000000 ft_jwt-0.0.6/setup.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1063 2024-04-04 12:46:38.000000 ft_jwt-0.0.7/LICENSE
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1845 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1279 2024-04-04 12:55:49.000000 ft_jwt-0.0.7/README.md
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 12:45:04.000000 ft_jwt-0.0.7/ft_jwt/__init__.py
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     3148 2024-04-04 12:45:41.000000 ft_jwt-0.0.7/ft_jwt/ft_jwt.py
+drwxr-xr-x   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        0 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)     1845 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      182 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        1 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)        7 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)       38 2024-04-04 14:05:20.000000 ft_jwt-0.0.7/setup.cfg
+-rw-r--r--   0 vfuhlenb (101447) 2021_wolfsburg  (4221)      723 2024-04-04 14:05:16.000000 ft_jwt-0.0.7/setup.py
```

### Comparing `ft_jwt-0.0.6/LICENSE` & `ft_jwt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.6/PKG-INFO` & `ft_jwt-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
-Home-page: https://github.com/minthe/ft_jwt
+Home-page: https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ft_jwt-0.0.6/README.md` & `ft_jwt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.6/ft_jwt/ft_jwt.py` & `ft_jwt-0.0.7/ft_jwt/ft_jwt.py`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.6/ft_jwt.egg-info/PKG-INFO` & `ft_jwt-0.0.7/ft_jwt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ft-jwt
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
-Home-page: https://github.com/minthe/ft_jwt
+Home-page: https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ft_jwt-0.0.6/setup.py` & `ft_jwt-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.0.6",
+	version="0.0.7",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
-	url="https://github.com/minthe/ft_jwt",
+	url="https://github.com/minthe/ft_transcendence/blob/jwt/auth/ft_jwt/ft_jwt/ft_jwt.py",
 	packages=setuptools.find_packages(),
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	python_requires='>=3.6',
```

