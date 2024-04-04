# Comparing `tmp/ithaca_py-0.1.6.tar.gz` & `tmp/ithaca_py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.1.6.tar", max compression
+gzip compressed data, was "ithaca_py-0.1.7.tar", max compression
```

## Comparing `ithaca_py-0.1.6.tar` & `ithaca_py-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/README.md
--rw-r--r--   0        0        0     4395 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/analytics.py
--rw-r--r--   0        0        0    10546 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/calculation.py
--rw-r--r--   0        0        0     2921 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/constants.py
--rw-r--r--   0        0        0    11748 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/market.py
--rw-r--r--   0        0        0     6467 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/protocol.py
--rw-r--r--   0        0        0     2210 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-04-03 20:20:04.455503 ithaca_py-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-04-04 09:18:25.067482 ithaca_py-0.1.7/README.md
+-rw-r--r--   0        0        0     4637 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/analytics.py
+-rw-r--r--   0        0        0    10546 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/calculation.py
+-rw-r--r--   0        0        0     2921 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/constants.py
+-rw-r--r--   0        0        0    11748 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/market.py
+-rw-r--r--   0        0        0     6467 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/protocol.py
+-rw-r--r--   0        0        0     2210 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-04-04 09:18:25.071482 ithaca_py-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.1.7/PKG-INFO
```

### Comparing `ithaca_py-0.1.6/README.md` & `ithaca_py-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/__init__.py` & `ithaca_py-0.1.7/ithaca/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,18 @@
           ws_endpoint (str): Websocket Endpoint
           graphql_endpoint (str): Graphql Endpoint
           rpc_endpoint (str): RPC Endpoint
           env_name (str): (Depreciated) Environment Name
         """
         if not all([api_endpoint, ws_endpoint, graphql_endpoint, rpc_endpoint]):
           logging.warning(f"Endpoint specifications not found, defaulting to 'env_name': {env_name}")
+          logging.warning(f"api_endpoint: {api_endpoint}")
+          logging.warning(f"ws_endpoint: {ws_endpoint}")
+          logging.warning(f"graphql_endpoint: {graphql_endpoint}")
+          logging.warning(f"rpc_endpoint: {rpc_endpoint}")
           self.env = ENVS.get(env_name)
         else:
           self.env = {
             "base_url": api_endpoint,
             "ws_url": ws_endpoint,
             "subgraph": graphql_endpoint,
             "rpc_url": rpc_endpoint
```

### Comparing `ithaca_py-0.1.6/ithaca/analytics.py` & `ithaca_py-0.1.7/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/auth.py` & `ithaca_py-0.1.7/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/calculation.py` & `ithaca_py-0.1.7/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/client.py` & `ithaca_py-0.1.7/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/constants.py` & `ithaca_py-0.1.7/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/fundlock.py` & `ithaca_py-0.1.7/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/market.py` & `ithaca_py-0.1.7/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/orders.py` & `ithaca_py-0.1.7/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/protocol.py` & `ithaca_py-0.1.7/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/ithaca/socket.py` & `ithaca_py-0.1.7/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.6/pyproject.toml` & `ithaca_py-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.1.6"
+version = "0.1.7"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.1.6/PKG-INFO` & `ithaca_py-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

