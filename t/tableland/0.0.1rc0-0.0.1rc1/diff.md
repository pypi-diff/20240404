# Comparing `tmp/tableland-0.0.1rc0.tar.gz` & `tmp/tableland-0.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableland-0.0.1rc0.tar", max compression
+gzip compressed data, was "tableland-0.0.1rc1.tar", max compression
```

## Comparing `tableland-0.0.1rc0.tar` & `tableland-0.0.1rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1092 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/LICENSE
--rw-r--r--   0        0        0     9723 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/LICENSE-APACHE
--rw-r--r--   0        0        0     5800 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/README.md
--rw-r--r--   0        0        0    22663 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/abi.json
--rw-r--r--   0        0        0     1573 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/pyproject.toml
--rw-r--r--   0        0        0     1120 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/__main__.py
--rw-r--r--   0        0        0     8346 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/database.py
--rw-r--r--   0        0        0     6478 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/helpers.py
--rw-r--r--   0        0        0     3268 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/types.py
--rw-r--r--   0        0        0     6423 1970-01-01 00:00:00.000000 tableland-0.0.1rc0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-04 07:02:19.547519 tableland-0.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     9723 2024-03-28 22:25:56.228374 tableland-0.0.1rc1/LICENSE-APACHE
+-rw-r--r--   0        0        0     5810 2024-04-04 07:02:26.258854 tableland-0.0.1rc1/README.md
+-rw-r--r--   0        0        0     1497 2024-04-04 07:01:42.570760 tableland-0.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     1120 2024-04-04 04:50:22.113829 tableland-0.0.1rc1/tableland/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:33:35.553404 tableland-0.0.1rc1/tableland/__main__.py
+-rw-r--r--   0        0        0    22663 2024-04-02 02:05:50.567072 tableland-0.0.1rc1/tableland/abi.json
+-rw-r--r--   0        0        0     8339 2024-04-04 06:58:40.742608 tableland-0.0.1rc1/tableland/database.py
+-rw-r--r--   0        0        0     6478 2024-04-04 07:02:56.358179 tableland-0.0.1rc1/tableland/helpers.py
+-rw-r--r--   0        0        0     3268 2024-04-03 23:42:44.792540 tableland-0.0.1rc1/tableland/types.py
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 tableland-0.0.1rc1/PKG-INFO
```

### Comparing `tableland-0.0.1rc0/LICENSE` & `tableland-0.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc0/LICENSE-APACHE` & `tableland-0.0.1rc1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc0/README.md` & `tableland-0.0.1rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -156,8 +156,8 @@
 PRs accepted.
 
 This package was created with Cookiecutter and the [sourcery.ai](https://github.com/sourcery-ai/python-best-practices-cookiecutter) project template. Small note: If editing the README, please conform to the
 [standard-readme](https://github.com/RichardLitt/standard-readme) specification.
 
 ## License
 
-MIT AND Apache-2.0, © 2021-2024 Textile Contributors
+MIT AND Apache-2.0, © 2021-2024 Tableland Network Contributors
```

### Comparing `tableland-0.0.1rc0/abi.json` & `tableland-0.0.1rc1/tableland/abi.json`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc0/pyproject.toml` & `tableland-0.0.1rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 [tool.poetry]
 name = "tableland"
-version = "0.0.1-pre.0"
+version = "0.0.1-pre.1"
 description = "A minimal Tableland Python SDK for creating, writing, and reading onchain tables"
 authors = ["Dan Buchholz <dbuchholz30@gmail.com>"]
 license = "MIT AND Apache-2.0"
 readme = "README.md"
-packages = [
-    { include = "abi.json" },
-    { include = "tableland" },
-]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 web3 = "^6.16.0"
 requests = "^2.31.0"
 sqlglot = "^23.6.3"
```

### Comparing `tableland-0.0.1rc0/tableland/__init__.py` & `tableland-0.0.1rc1/tableland/__init__.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc0/tableland/database.py` & `tableland-0.0.1rc1/tableland/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         private_key: str,
         provider_uri: str,
     ):
         # Set up web3 instance and signer
         self.w3 = Web3(Web3.HTTPProvider(provider_uri))
         self.signer = Account.from_key(private_key)
         # Set up Tableland registry contract and validator base URI
-        abi_file = Path(__file__).parent.parent / "abi.json"
+        abi_file = Path(__file__).parent / "abi.json"
         abi = read_file_to_json(abi_file)
         registry_addr = get_registry_address(self.w3.eth.chain_id)
         self.registry = self.w3.eth.contract(
             address=to_checksum_address(registry_addr), abi=abi
         )
         self.validator_uri = get_validator_base_uri(chain_id=self.get_chain_id())
```

### Comparing `tableland-0.0.1rc0/tableland/helpers.py` & `tableland-0.0.1rc1/tableland/helpers.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc0/tableland/types.py` & `tableland-0.0.1rc1/tableland/types.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc0/PKG-INFO` & `tableland-0.0.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableland
-Version: 0.0.1rc0
+Version: 0.0.1rc1
 Summary: A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 License: MIT AND Apache-2.0
 Author: Dan Buchholz
 Author-email: dbuchholz30@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -173,9 +173,9 @@
 PRs accepted.
 
 This package was created with Cookiecutter and the [sourcery.ai](https://github.com/sourcery-ai/python-best-practices-cookiecutter) project template. Small note: If editing the README, please conform to the
 [standard-readme](https://github.com/RichardLitt/standard-readme) specification.
 
 ## License
 
-MIT AND Apache-2.0, © 2021-2024 Textile Contributors
+MIT AND Apache-2.0, © 2021-2024 Tableland Network Contributors
```

