# Comparing `tmp/xoadmin-1.2.1.tar.gz` & `tmp/xoadmin-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoadmin-1.2.1.tar", max compression
+gzip compressed data, was "xoadmin-1.2.2.tar", max compression
```

## Comparing `xoadmin-1.2.1.tar` & `xoadmin-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11336 2024-04-04 20:49:55.268645 xoadmin-1.2.1/LICENSE
--rw-r--r--   0        0        0     5705 2024-04-04 20:49:55.268645 xoadmin-1.2.1/README.md
--rw-r--r--   0        0        0      787 2024-04-04 20:49:55.268645 xoadmin-1.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/__init__.py
--rw-r--r--   0        0        0     4643 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/api.py
--rw-r--r--   0        0        0      389 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/error.py
--rw-r--r--   0        0        0     2192 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/host.py
--rw-r--r--   0        0        0     6696 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/manager.py
--rw-r--r--   0        0        0     1418 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/storage.py
--rw-r--r--   0        0        0     3824 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/user.py
--rw-r--r--   0        0        0     1586 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/vm.py
--rw-r--r--   0        0        0     5724 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/websocket.py
--rw-r--r--   0        0        0        0 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/__init__.py
--rw-r--r--   0        0        0      750 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/apply.py
--rw-r--r--   0        0        0     2199 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/auth.py
--rw-r--r--   0        0        0     1433 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/cli.py
--rw-r--r--   0        0        0     4542 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/config.py
--rw-r--r--   0        0        0     2002 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/hosts.py
--rw-r--r--   0        0        0     1751 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/model.py
--rw-r--r--   0        0        0      784 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/options.py
--rw-r--r--   0        0        0     1937 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/storage.py
--rw-r--r--   0        0        0     2046 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/users.py
--rw-r--r--   0        0        0     6103 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/utils.py
--rw-r--r--   0        0        0     1940 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/vms.py
--rw-r--r--   0        0        0        0 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/__init__.py
--rw-r--r--   0        0        0      708 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/config.py
--rw-r--r--   0        0        0     1571 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/configurator.py
--rw-r--r--   0        0        0      283 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/loader.py
--rw-r--r--   0        0        0     1822 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/utils.py
--rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 xoadmin-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-04 20:56:51.381844 xoadmin-1.2.2/LICENSE
+-rw-r--r--   0        0        0     5725 2024-04-04 20:56:51.381844 xoadmin-1.2.2/README.md
+-rw-r--r--   0        0        0      787 2024-04-04 20:56:51.381844 xoadmin-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/__init__.py
+-rw-r--r--   0        0        0     4643 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/api.py
+-rw-r--r--   0        0        0      389 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/error.py
+-rw-r--r--   0        0        0     2192 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/host.py
+-rw-r--r--   0        0        0     6696 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/manager.py
+-rw-r--r--   0        0        0     1418 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/storage.py
+-rw-r--r--   0        0        0     3824 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/user.py
+-rw-r--r--   0        0        0     1586 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/vm.py
+-rw-r--r--   0        0        0     5724 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/api/websocket.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/apply.py
+-rw-r--r--   0        0        0     2199 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/auth.py
+-rw-r--r--   0        0        0     1433 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/cli.py
+-rw-r--r--   0        0        0     4542 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/config.py
+-rw-r--r--   0        0        0     2002 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/hosts.py
+-rw-r--r--   0        0        0     1736 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/model.py
+-rw-r--r--   0        0        0      784 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/options.py
+-rw-r--r--   0        0        0     1937 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/storage.py
+-rw-r--r--   0        0        0     2046 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/users.py
+-rw-r--r--   0        0        0     6103 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/utils.py
+-rw-r--r--   0        0        0     1940 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/cli/vms.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/__init__.py
+-rw-r--r--   0        0        0      708 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/config.py
+-rw-r--r--   0        0        0     1571 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/configurator.py
+-rw-r--r--   0        0        0      283 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/configurator/loader.py
+-rw-r--r--   0        0        0     1822 2024-04-04 20:56:51.381844 xoadmin-1.2.2/src/xoadmin/utils.py
+-rw-r--r--   0        0        0     6589 1970-01-01 00:00:00.000000 xoadmin-1.2.2/PKG-INFO
```

### Comparing `xoadmin-1.2.1/LICENSE` & `xoadmin-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/README.md` & `xoadmin-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     # - XOA_PASSWORD
     # - XOA_VERIFY_SSL
     ```
 
 3. **Performing Operations:** You can now perform various operations using the CLI.
 
     The cli utilizes a config file under ~/.xoadmin/config
-    ```
+    ```yaml
     xoa:
       host: localhost
       ws_url: ws://localhost
       rest_api: http://localhost:80
       verify_ssl: false
       password: admin
       username: admin@admin.net
@@ -137,15 +137,15 @@
     ```
 ## Applying a Configuration
 
 xoadmin allows you to quickly add hosts and users to an XOA instance using a YAML file:
 
 1. Create a YAML file with your desired configuration settings. For example:
 
-    ```
+    ```yaml
     hypervisors:
       - host: 192.168.0.1
         username: root
         password: password
         allowUnauthorized: true
 
     users:
@@ -160,15 +160,15 @@
     xoadmin apply -f config.yaml
     ```
 
 ## Module Usage
 
 You can also integrate the XO Admin Library directly into your Python scripts for more customized usage. Here's an example of how you can do this:
 
-```
+```python
 import asyncio
 from xoadmin.api.manager import XOAManager
 
 async def main():
     # Initialize XOAManager
     manager = XOAManager(
         host="localhost",
@@ -184,15 +184,15 @@
     vms = await manager.list_all_vms()
     print(vms)
 
     # Close session
     await manager.close()
 ```
 
-```
+```python
 import asyncio
 from xoadmin.api.api import XOAPI
 
 async def main():
     api = XOAPI(
                 rest_base_url="http://localhost:80", # without /rest
                 ws_url="ws://localhost",
```

### Comparing `xoadmin-1.2.1/pyproject.toml` & `xoadmin-1.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xoadmin"
-version = "1.2.1"
+version = "1.2.2"
 description = "bindings and wrappers to manage an XOA instance"
 authors = ["dennis <it.admin@elnissi.co.id>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "xoadmin", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `xoadmin-1.2.1/src/xoadmin/api/api.py` & `xoadmin-1.2.2/src/xoadmin/api/api.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/api/host.py` & `xoadmin-1.2.2/src/xoadmin/api/host.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/api/manager.py` & `xoadmin-1.2.2/src/xoadmin/api/manager.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/api/storage.py` & `xoadmin-1.2.2/src/xoadmin/api/storage.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/api/user.py` & `xoadmin-1.2.2/src/xoadmin/api/user.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/api/vm.py` & `xoadmin-1.2.2/src/xoadmin/api/vm.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/api/websocket.py` & `xoadmin-1.2.2/src/xoadmin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/apply.py` & `xoadmin-1.2.2/src/xoadmin/cli/apply.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/auth.py` & `xoadmin-1.2.2/src/xoadmin/cli/auth.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/cli.py` & `xoadmin-1.2.2/src/xoadmin/cli/cli.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/config.py` & `xoadmin-1.2.2/src/xoadmin/cli/config.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/hosts.py` & `xoadmin-1.2.2/src/xoadmin/cli/hosts.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/model.py` & `xoadmin-1.2.2/src/xoadmin/cli/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     rest_api: str = "XOA_REST_API"
     websocket: str = "XOA_WEBSOCKET"
     username: str = "XOA_USERNAME"
     password: str = "XOA_PASSWORD"
     verify_ssl: str = "XOA_VERIFY_SSL"
 
     defaults = {
-        "host": "default_host",
-        "websocket": "default_websocket",
-        "rest_api": "default_rest_api",
-        "username": "default_username",
-        "password": "default_password",
+        "host": "localhost",
+        "websocket": "ws://localhost",
+        "rest_api": "http://localhost:80",
+        "username": "admin@admin.net",
+        "password": "admin",
         "verify_ssl": False,
     }
 
     @staticmethod
     def get_env_var_name(key: str) -> Optional[str]:
         """Return the environment variable name for a given key."""
         name = getattr(XOASettings, key, None)
```

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/options.py` & `xoadmin-1.2.2/src/xoadmin/cli/options.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/storage.py` & `xoadmin-1.2.2/src/xoadmin/cli/storage.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/users.py` & `xoadmin-1.2.2/src/xoadmin/cli/users.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/utils.py` & `xoadmin-1.2.2/src/xoadmin/cli/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/cli/vms.py` & `xoadmin-1.2.2/src/xoadmin/cli/vms.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/configurator/config.py` & `xoadmin-1.2.2/src/xoadmin/configurator/config.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/configurator/configurator.py` & `xoadmin-1.2.2/src/xoadmin/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/src/xoadmin/utils.py` & `xoadmin-1.2.2/src/xoadmin/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.1/PKG-INFO` & `xoadmin-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoadmin
-Version: 1.2.1
+Version: 1.2.2
 Summary: bindings and wrappers to manage an XOA instance
 License: Apache 2.0
 Author: dennis
 Author-email: it.admin@elnissi.co.id
 Requires-Python: >=3.9.2
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -134,15 +134,15 @@
     # - XOA_PASSWORD
     # - XOA_VERIFY_SSL
     ```
 
 3. **Performing Operations:** You can now perform various operations using the CLI.
 
     The cli utilizes a config file under ~/.xoadmin/config
-    ```
+    ```yaml
     xoa:
       host: localhost
       ws_url: ws://localhost
       rest_api: http://localhost:80
       verify_ssl: false
       password: admin
       username: admin@admin.net
@@ -161,15 +161,15 @@
     ```
 ## Applying a Configuration
 
 xoadmin allows you to quickly add hosts and users to an XOA instance using a YAML file:
 
 1. Create a YAML file with your desired configuration settings. For example:
 
-    ```
+    ```yaml
     hypervisors:
       - host: 192.168.0.1
         username: root
         password: password
         allowUnauthorized: true
 
     users:
@@ -184,15 +184,15 @@
     xoadmin apply -f config.yaml
     ```
 
 ## Module Usage
 
 You can also integrate the XO Admin Library directly into your Python scripts for more customized usage. Here's an example of how you can do this:
 
-```
+```python
 import asyncio
 from xoadmin.api.manager import XOAManager
 
 async def main():
     # Initialize XOAManager
     manager = XOAManager(
         host="localhost",
@@ -208,15 +208,15 @@
     vms = await manager.list_all_vms()
     print(vms)
 
     # Close session
     await manager.close()
 ```
 
-```
+```python
 import asyncio
 from xoadmin.api.api import XOAPI
 
 async def main():
     api = XOAPI(
                 rest_base_url="http://localhost:80", # without /rest
                 ws_url="ws://localhost",
```

