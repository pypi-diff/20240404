# Comparing `tmp/ft_jwt-0.0.4.tar.gz` & `tmp/ft_jwt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_jwt-0.0.4.tar", last modified: Thu Apr  4 07:57:27 2024, max compression
+gzip compressed data, was "ft_jwt-0.0.5.tar", last modified: Thu Apr  4 08:14:53 2024, max compression
```

## Comparing `ft_jwt-0.0.4.tar` & `ft_jwt-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:57:27.117657 ft_jwt-0.0.4/
--rw-r--r--   0 minthe     (501) staff       (20)     1063 2024-04-04 07:43:46.000000 ft_jwt-0.0.4/LICENSE
--rw-r--r--   0 minthe     (501) staff       (20)     1548 2024-04-04 07:57:27.115499 ft_jwt-0.0.4/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)     1074 2024-04-04 07:56:40.000000 ft_jwt-0.0.4/README.md
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:57:27.109885 ft_jwt-0.0.4/ft_jwt/
--rw-r--r--   0 minthe     (501) staff       (20)        0 2024-04-04 07:32:01.000000 ft_jwt-0.0.4/ft_jwt/__init__.py
--rw-r--r--   0 minthe     (501) staff       (20)     3145 2024-04-04 07:24:14.000000 ft_jwt-0.0.4/ft_jwt/jwt.py
-drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 07:57:27.114714 ft_jwt-0.0.4/ft_jwt.egg-info/
--rw-r--r--   0 minthe     (501) staff       (20)     1548 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/PKG-INFO
--rw-r--r--   0 minthe     (501) staff       (20)      179 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 minthe     (501) staff       (20)        1 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 minthe     (501) staff       (20)        7 2024-04-04 07:57:27.000000 ft_jwt-0.0.4/ft_jwt.egg-info/top_level.txt
--rw-r--r--   0 minthe     (501) staff       (20)       38 2024-04-04 07:57:27.117821 ft_jwt-0.0.4/setup.cfg
--rw-r--r--   0 minthe     (501) staff       (20)      634 2024-04-04 07:57:20.000000 ft_jwt-0.0.4/setup.py
+drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 08:14:53.039876 ft_jwt-0.0.5/
+-rw-r--r--   0 minthe     (501) staff       (20)     1063 2024-04-04 07:43:46.000000 ft_jwt-0.0.5/LICENSE
+-rw-r--r--   0 minthe     (501) staff       (20)     1592 2024-04-04 08:14:53.037807 ft_jwt-0.0.5/PKG-INFO
+-rw-r--r--   0 minthe     (501) staff       (20)     1074 2024-04-04 07:56:40.000000 ft_jwt-0.0.5/README.md
+drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 08:14:53.033465 ft_jwt-0.0.5/ft_jwt/
+-rw-r--r--   0 minthe     (501) staff       (20)        0 2024-04-04 07:32:01.000000 ft_jwt-0.0.5/ft_jwt/__init__.py
+-rw-r--r--   0 minthe     (501) staff       (20)     3145 2024-04-04 07:24:14.000000 ft_jwt-0.0.5/ft_jwt/jwt.py
+drwxr-xr-x   0 minthe     (501) staff       (20)        0 2024-04-04 08:14:53.037049 ft_jwt-0.0.5/ft_jwt.egg-info/
+-rw-r--r--   0 minthe     (501) staff       (20)     1592 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 minthe     (501) staff       (20)      179 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 minthe     (501) staff       (20)        1 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 minthe     (501) staff       (20)        7 2024-04-04 08:14:52.000000 ft_jwt-0.0.5/ft_jwt.egg-info/top_level.txt
+-rw-r--r--   0 minthe     (501) staff       (20)       38 2024-04-04 08:14:53.040025 ft_jwt-0.0.5/setup.cfg
+-rw-r--r--   0 minthe     (501) staff       (20)      675 2024-04-04 08:14:35.000000 ft_jwt-0.0.5/setup.py
```

### Comparing `ft_jwt-0.0.4/LICENSE` & `ft_jwt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.4/PKG-INFO` & `ft_jwt-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
+Home-page: https://github.com/minthe/ft_jwt
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ft_jwt-0.0.4/README.md` & `ft_jwt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.4/ft_jwt/jwt.py` & `ft_jwt-0.0.5/ft_jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `ft_jwt-0.0.4/ft_jwt.egg-info/PKG-INFO` & `ft_jwt-0.0.5/ft_jwt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: ft_jwt
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.
+Home-page: https://github.com/minthe/ft_jwt
 Author: vfuhlenb
 Author-email: minh.tee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ft_jwt-0.0.4/setup.py` & `ft_jwt-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="ft_jwt",
-	version="0.0.4",
+	version="0.0.5",
 	author="vfuhlenb",
 	author_email="minh.tee@gmail.com",
 	description="A Python implementation of JSON Web Tokens (JWT) for authentication and authorization using a symmetric secret key and HMAC-SHA256.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
+	url="https://github.com/minthe/ft_jwt",
 	packages=setuptools.find_packages(),
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	python_requires='>=3.6',
```

