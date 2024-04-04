# Comparing `tmp/btcs_crypto_systems-0.0.8.tar.gz` & `tmp/btcs_crypto_systems-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btcs_crypto_systems-0.0.8.tar", last modified: Tue Feb 20 17:07:41 2024, max compression
+gzip compressed data, was "btcs_crypto_systems-0.0.9.tar", last modified: Thu Apr  4 06:34:08 2024, max compression
```

## Comparing `btcs_crypto_systems-0.0.8.tar` & `btcs_crypto_systems-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 17:07:41.503144 btcs_crypto_systems-0.0.8/
--rw-rw-rw-   0        0        0     1378 2024-02-20 17:07:41.500147 btcs_crypto_systems-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2024-02-20 17:05:29.000000 btcs_crypto_systems-0.0.8/README.md
--rw-rw-rw-   0        0        0      176 2024-02-20 17:07:21.000000 btcs_crypto_systems-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-20 17:07:41.503144 btcs_crypto_systems-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-20 17:07:41.452163 btcs_crypto_systems-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-02-20 17:07:41.480145 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/
--rw-rw-rw-   0        0        0        0 2024-01-26 15:26:09.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/__init__.py
--rw-rw-rw-   0        0        0     7715 2024-02-20 17:02:41.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/address_manangement_service.py
--rw-rw-rw-   0        0        0    13394 2024-01-26 16:51:18.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/token_master.py
--rw-rw-rw-   0        0        0      982 2024-01-26 16:50:51.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/txstore.py
--rw-rw-rw-   0        0        0      348 2024-01-26 15:26:09.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-20 17:07:41.498158 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems.egg-info/
--rw-rw-rw-   0        0        0     1378 2024-02-20 17:07:41.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2024-02-20 17:07:41.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 17:07:41.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-02-20 17:07:41.000000 btcs_crypto_systems-0.0.8/src/btcs_crypto_systems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 06:34:08.957143 btcs_crypto_systems-0.0.9/
+-rw-rw-rw-   0        0        0     1401 2024-04-04 06:34:08.954137 btcs_crypto_systems-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1220 2024-02-20 17:17:01.000000 btcs_crypto_systems-0.0.9/README.md
+-rw-rw-rw-   0        0        0      176 2024-04-04 06:29:36.000000 btcs_crypto_systems-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 06:34:08.957143 btcs_crypto_systems-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 06:34:08.908138 btcs_crypto_systems-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 06:34:08.932159 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/
+-rw-rw-rw-   0        0        0        0 2024-01-26 15:26:09.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/__init__.py
+-rw-rw-rw-   0        0        0    12097 2024-04-04 06:33:16.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/address_manangement_service.py
+-rw-rw-rw-   0        0        0    13394 2024-01-26 16:51:18.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/token_master.py
+-rw-rw-rw-   0        0        0      982 2024-01-26 16:50:51.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/txstore.py
+-rw-rw-rw-   0        0        0      348 2024-01-26 15:26:09.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:34:08.951145 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems.egg-info/
+-rw-rw-rw-   0        0        0     1401 2024-04-04 06:34:08.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2024-04-04 06:34:08.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 06:34:08.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-04 06:34:08.000000 btcs_crypto_systems-0.0.9/src/btcs_crypto_systems.egg-info/top_level.txt
```

### Comparing `btcs_crypto_systems-0.0.8/PKG-INFO` & `btcs_crypto_systems-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btcs_crypto_systems
-Version: 0.0.8
+Version: 0.0.9
 Summary: To interact with BTCS crypto systems.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # crypto systems package for BTCS crypto business systems
 
 
@@ -43,15 +43,15 @@
 
 ams = address_manangement_service.AMS(env="test")
 print(json.dumps(ams.get_addresses(is_deposit=True, include_balances=True, limit=10, tags=["siba"]), indent=2))
 ```
 
 
 ## Update the package
-Navigate to the folder where the pyproject.toml file is.
+Navigate to the folder where the pyproject.toml file is. Update version number.
 ```bash
 python3 -m build
 python3 -m twine upload --repository pypi dist/*
 ```
 ```
 username: __token__
 password: get an API key from here https://pypi.org/manage/account/token/
```

### Comparing `btcs_crypto_systems-0.0.8/README.md` & `btcs_crypto_systems-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 ams = address_manangement_service.AMS(env="test")
 print(json.dumps(ams.get_addresses(is_deposit=True, include_balances=True, limit=10, tags=["siba"]), indent=2))
 ```
 
 
 ## Update the package
-Navigate to the folder where the pyproject.toml file is.
+Navigate to the folder where the pyproject.toml file is. Update version number.
 ```bash
 python3 -m build
 python3 -m twine upload --repository pypi dist/*
 ```
 ```
 username: __token__
 password: get an API key from here https://pypi.org/manage/account/token/
```

### Comparing `btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/token_master.py` & `btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/token_master.py`

 * *Files identical despite different names*

### Comparing `btcs_crypto_systems-0.0.8/src/btcs_crypto_systems/txstore.py` & `btcs_crypto_systems-0.0.9/src/btcs_crypto_systems/txstore.py`

 * *Files identical despite different names*

### Comparing `btcs_crypto_systems-0.0.8/src/btcs_crypto_systems.egg-info/PKG-INFO` & `btcs_crypto_systems-0.0.9/src/btcs_crypto_systems.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btcs_crypto_systems
-Version: 0.0.8
+Version: 0.0.9
 Summary: To interact with BTCS crypto systems.
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # crypto systems package for BTCS crypto business systems
 
 
@@ -43,15 +43,15 @@
 
 ams = address_manangement_service.AMS(env="test")
 print(json.dumps(ams.get_addresses(is_deposit=True, include_balances=True, limit=10, tags=["siba"]), indent=2))
 ```
 
 
 ## Update the package
-Navigate to the folder where the pyproject.toml file is.
+Navigate to the folder where the pyproject.toml file is. Update version number.
 ```bash
 python3 -m build
 python3 -m twine upload --repository pypi dist/*
 ```
 ```
 username: __token__
 password: get an API key from here https://pypi.org/manage/account/token/
```

