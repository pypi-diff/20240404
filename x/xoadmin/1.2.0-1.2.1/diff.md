# Comparing `tmp/xoadmin-1.2.0.tar.gz` & `tmp/xoadmin-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoadmin-1.2.0.tar", max compression
+gzip compressed data, was "xoadmin-1.2.1.tar", max compression
```

## Comparing `xoadmin-1.2.0.tar` & `xoadmin-1.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11336 2024-04-04 20:24:18.997663 xoadmin-1.2.0/LICENSE
--rw-r--r--   0        0        0     5934 2024-04-04 20:24:18.997663 xoadmin-1.2.0/README.md
--rw-r--r--   0        0        0      787 2024-04-04 20:24:18.997663 xoadmin-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/__init__.py
--rw-r--r--   0        0        0     4643 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/api.py
--rw-r--r--   0        0        0      389 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/error.py
--rw-r--r--   0        0        0     2192 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/host.py
--rw-r--r--   0        0        0     6696 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/manager.py
--rw-r--r--   0        0        0     1418 2024-04-04 20:24:18.997663 xoadmin-1.2.0/src/xoadmin/api/storage.py
--rw-r--r--   0        0        0     3824 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/api/user.py
--rw-r--r--   0        0        0     1586 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/api/vm.py
--rw-r--r--   0        0        0     5724 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/api/websocket.py
--rw-r--r--   0        0        0        0 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/__init__.py
--rw-r--r--   0        0        0      482 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/apply.py
--rw-r--r--   0        0        0     2199 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/auth.py
--rw-r--r--   0        0        0     1433 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/cli.py
--rw-r--r--   0        0        0     4542 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/config.py
--rw-r--r--   0        0        0     2002 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/hosts.py
--rw-r--r--   0        0        0     1751 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/model.py
--rw-r--r--   0        0        0      784 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/options.py
--rw-r--r--   0        0        0     1937 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/storage.py
--rw-r--r--   0        0        0     2046 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/users.py
--rw-r--r--   0        0        0     6103 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/utils.py
--rw-r--r--   0        0        0     1940 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/cli/vms.py
--rw-r--r--   0        0        0        0 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/__init__.py
--rw-r--r--   0        0        0      692 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/config.py
--rw-r--r--   0        0        0     1462 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/configurator.py
--rw-r--r--   0        0        0      277 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/configurator/loader.py
--rw-r--r--   0        0        0     1822 2024-04-04 20:24:19.001663 xoadmin-1.2.0/src/xoadmin/utils.py
--rw-r--r--   0        0        0     6798 1970-01-01 00:00:00.000000 xoadmin-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-04 20:49:55.268645 xoadmin-1.2.1/LICENSE
+-rw-r--r--   0        0        0     5705 2024-04-04 20:49:55.268645 xoadmin-1.2.1/README.md
+-rw-r--r--   0        0        0      787 2024-04-04 20:49:55.268645 xoadmin-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/__init__.py
+-rw-r--r--   0        0        0     4643 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/api.py
+-rw-r--r--   0        0        0      389 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/error.py
+-rw-r--r--   0        0        0     2192 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/host.py
+-rw-r--r--   0        0        0     6696 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/manager.py
+-rw-r--r--   0        0        0     1418 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/storage.py
+-rw-r--r--   0        0        0     3824 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/user.py
+-rw-r--r--   0        0        0     1586 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/vm.py
+-rw-r--r--   0        0        0     5724 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/api/websocket.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/__init__.py
+-rw-r--r--   0        0        0      750 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/apply.py
+-rw-r--r--   0        0        0     2199 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/auth.py
+-rw-r--r--   0        0        0     1433 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/cli.py
+-rw-r--r--   0        0        0     4542 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/config.py
+-rw-r--r--   0        0        0     2002 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/hosts.py
+-rw-r--r--   0        0        0     1751 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/model.py
+-rw-r--r--   0        0        0      784 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/options.py
+-rw-r--r--   0        0        0     1937 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/storage.py
+-rw-r--r--   0        0        0     2046 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/users.py
+-rw-r--r--   0        0        0     6103 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/utils.py
+-rw-r--r--   0        0        0     1940 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/cli/vms.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/__init__.py
+-rw-r--r--   0        0        0      708 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/config.py
+-rw-r--r--   0        0        0     1571 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/configurator.py
+-rw-r--r--   0        0        0      283 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/configurator/loader.py
+-rw-r--r--   0        0        0     1822 2024-04-04 20:49:55.268645 xoadmin-1.2.1/src/xoadmin/utils.py
+-rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 xoadmin-1.2.1/PKG-INFO
```

### Comparing `xoadmin-1.2.0/LICENSE` & `xoadmin-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/README.md` & `xoadmin-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -133,26 +133,19 @@
     ```
     List hosts
     ```
     xoadmin host list
     ```
 ## Applying a Configuration
 
-xoadmin allows you to quickly add hosts and users to an XOA instance (completely separate from the ~/.xoadmin/config host) using a YAML file. Here's how to do it:
+xoadmin allows you to quickly add hosts and users to an XOA instance using a YAML file:
 
 1. Create a YAML file with your desired configuration settings. For example:
 
     ```
-    xoa:
-      host: localhost
-      websocket: ws://localhost
-      rest_api: http://localhost:80
-      username: admin@admin.net
-      password: admin
-
     hypervisors:
       - host: 192.168.0.1
         username: root
         password: password
         allowUnauthorized: true
 
     users:
```

### Comparing `xoadmin-1.2.0/pyproject.toml` & `xoadmin-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xoadmin"
-version = "1.2.0"
+version = "1.2.1"
 description = "bindings and wrappers to manage an XOA instance"
 authors = ["dennis <it.admin@elnissi.co.id>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "xoadmin", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `xoadmin-1.2.0/src/xoadmin/api/api.py` & `xoadmin-1.2.1/src/xoadmin/api/api.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/api/host.py` & `xoadmin-1.2.1/src/xoadmin/api/host.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/api/manager.py` & `xoadmin-1.2.1/src/xoadmin/api/manager.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/api/storage.py` & `xoadmin-1.2.1/src/xoadmin/api/storage.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/api/user.py` & `xoadmin-1.2.1/src/xoadmin/api/user.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/api/vm.py` & `xoadmin-1.2.1/src/xoadmin/api/vm.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/api/websocket.py` & `xoadmin-1.2.1/src/xoadmin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/auth.py` & `xoadmin-1.2.1/src/xoadmin/cli/auth.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/cli.py` & `xoadmin-1.2.1/src/xoadmin/cli/cli.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/config.py` & `xoadmin-1.2.1/src/xoadmin/cli/config.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/hosts.py` & `xoadmin-1.2.1/src/xoadmin/cli/hosts.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/model.py` & `xoadmin-1.2.1/src/xoadmin/cli/model.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/options.py` & `xoadmin-1.2.1/src/xoadmin/cli/options.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/storage.py` & `xoadmin-1.2.1/src/xoadmin/cli/storage.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/users.py` & `xoadmin-1.2.1/src/xoadmin/cli/users.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/utils.py` & `xoadmin-1.2.1/src/xoadmin/cli/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/cli/vms.py` & `xoadmin-1.2.1/src/xoadmin/cli/vms.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/src/xoadmin/configurator/config.py` & `xoadmin-1.2.1/src/xoadmin/configurator/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     host: str
     username: str
     password: str
     autoConnect: Optional[bool] = True
     allowUnauthorized: Optional[bool] = False
 
 
-class XOAInstance(BaseModel):
-    host: str
-    rest_api: Optional[str] = None
-    websocket: Optional[str] = None
-    username: str
-    password: str
+# class XOAInstance(BaseModel):
+#     host: str
+#     rest_api: Optional[str] = None
+#     websocket: Optional[str] = None
+#     username: str
+#     password: str
 
 
 class UserConfig(BaseModel):
     username: str
     password: str
     permission: Optional[str] = "none"
 
 
-class AppConfig(BaseModel):
-    xoa: XOAInstance
+class ApplyConfig(BaseModel):
+    # xoa: XOAInstance
     hypervisors: List[HypervisorConfig]
     users: List[UserConfig]
```

### Comparing `xoadmin-1.2.0/src/xoadmin/configurator/configurator.py` & `xoadmin-1.2.1/src/xoadmin/configurator/configurator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from typing import Optional
 
 from xoadmin.api.manager import XOAManager
-from xoadmin.configurator.config import AppConfig
+from xoadmin.configurator.config import ApplyConfig
 from xoadmin.configurator.loader import load_config
 
 
 class XOAConfigurator:
-    def __init__(self, config_path: str):
-        self.config_path = config_path
-        self.app_config: Optional[AppConfig] = None
-
-    async def load_and_apply_configuration(self):
-        self.app_config = load_config(self.config_path)
-
-        # Initialize XOAManager with XOA instance details
-        xoa_manager = XOAManager(
-            self.app_config.xoa.host,
-            self.app_config.xoa.rest_api,
-            self.app_config.xoa.websocket,
-            verify_ssl=False,
-        )
-        await xoa_manager.authenticate(
-            username=self.app_config.xoa.username, password=self.app_config.xoa.password
-        )
+    def __init__(
+        self, apply_config: ApplyConfig = None, xoa_manager: XOAManager = None
+    ):
+        self.apply_config: ApplyConfig = apply_config
+        self.xoa_manager: Optional[XOAManager] = xoa_manager
+
+    def load(self, config_path: str):
+        self.apply_config = load_config(config_path)
+
+    async def apply(
+        self, apply_config: ApplyConfig = None, xoa_manager: XOAManager = None
+    ):
+        if not xoa_manager:
+            xoa_manager = self.xoa_manager
+        if not xoa_manager:
+            raise ValueError("No XOAPI instance provided.")
+        if not apply_config:
+            apply_config = self.apply_config
+        if not apply_config:
+            raise ValueError("No ApplyConfig provided.")
         # Create users
-        for user in self.app_config.users:
+        for user in self.apply_config.users:
             await xoa_manager.create_user(
                 email=user.username, password=user.password, permission=user.permission
             )
 
         # Add hypervisors
-        for hypervisor in self.app_config.hypervisors:
+        for hypervisor in self.apply_config.hypervisors:
             await xoa_manager.add_host(
                 host=hypervisor.host,
                 username=hypervisor.username,
                 password=hypervisor.password,
                 autoConnect=hypervisor.autoConnect,
                 allowUnauthorized=hypervisor.allowUnauthorized,
             )
```

### Comparing `xoadmin-1.2.0/src/xoadmin/utils.py` & `xoadmin-1.2.1/src/xoadmin/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.2.0/PKG-INFO` & `xoadmin-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoadmin
-Version: 1.2.0
+Version: 1.2.1
 Summary: bindings and wrappers to manage an XOA instance
 License: Apache 2.0
 Author: dennis
 Author-email: it.admin@elnissi.co.id
 Requires-Python: >=3.9.2
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -157,26 +157,19 @@
     ```
     List hosts
     ```
     xoadmin host list
     ```
 ## Applying a Configuration
 
-xoadmin allows you to quickly add hosts and users to an XOA instance (completely separate from the ~/.xoadmin/config host) using a YAML file. Here's how to do it:
+xoadmin allows you to quickly add hosts and users to an XOA instance using a YAML file:
 
 1. Create a YAML file with your desired configuration settings. For example:
 
     ```
-    xoa:
-      host: localhost
-      websocket: ws://localhost
-      rest_api: http://localhost:80
-      username: admin@admin.net
-      password: admin
-
     hypervisors:
       - host: 192.168.0.1
         username: root
         password: password
         allowUnauthorized: true
 
     users:
```

