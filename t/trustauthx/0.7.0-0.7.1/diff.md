# Comparing `tmp/trustauthx-0.7.0.tar.gz` & `tmp/trustauthx-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.7.0.tar", last modified: Wed Apr  3 18:43:41 2024, max compression
+gzip compressed data, was "trustauthx-0.7.1.tar", last modified: Wed Apr  3 22:42:19 2024, max compression
```

## Comparing `trustauthx-0.7.0.tar` & `trustauthx-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:43:41.092127 trustauthx-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 18:43:32.000000 trustauthx-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 18:43:41.092127 trustauthx-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 18:43:32.000000 trustauthx-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:43:41.092127 trustauthx-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 18:43:32.000000 trustauthx-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:43:41.088127 trustauthx-0.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 18:43:32.000000 trustauthx-0.7.0/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:43:41.088127 trustauthx-0.7.0/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 18:43:32.000000 trustauthx-0.7.0/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32917 2024-04-03 18:43:32.000000 trustauthx-0.7.0/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 18:43:32.000000 trustauthx-0.7.0/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 18:43:32.000000 trustauthx-0.7.0/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 18:43:32.000000 trustauthx-0.7.0/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:43:41.092127 trustauthx-0.7.0/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 18:43:41.000000 trustauthx-0.7.0/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 18:43:41.000000 trustauthx-0.7.0/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:43:41.000000 trustauthx-0.7.0/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 18:43:41.000000 trustauthx-0.7.0/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 18:43:41.000000 trustauthx-0.7.0/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:43:41.000000 trustauthx-0.7.0/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:42:19.940327 trustauthx-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 22:42:11.000000 trustauthx-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 22:42:19.940327 trustauthx-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 22:42:11.000000 trustauthx-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:42:19.940327 trustauthx-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 22:42:11.000000 trustauthx-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:42:19.936327 trustauthx-0.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 22:42:11.000000 trustauthx-0.7.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:42:19.936327 trustauthx-0.7.1/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 22:42:11.000000 trustauthx-0.7.1/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32997 2024-04-03 22:42:11.000000 trustauthx-0.7.1/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 22:42:11.000000 trustauthx-0.7.1/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 22:42:11.000000 trustauthx-0.7.1/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-03 22:42:11.000000 trustauthx-0.7.1/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:42:19.936327 trustauthx-0.7.1/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 22:42:19.000000 trustauthx-0.7.1/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 22:42:19.000000 trustauthx-0.7.1/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:42:19.000000 trustauthx-0.7.1/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 22:42:19.000000 trustauthx-0.7.1/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 22:42:19.000000 trustauthx-0.7.1/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 22:42:19.000000 trustauthx-0.7.1/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.7.0/LICENSE` & `trustauthx-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.0/PKG-INFO` & `trustauthx-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.7.0
+Version: 0.7.1
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.7.0/README.md` & `trustauthx-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.0/setup.py` & `trustauthx-0.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='trustauthx',
-    version='0.7.0',
+    version='0.7.1',
     description='Official connector SDK for TrustAuthx',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='moonlightnexus',
     author_email='nexus@trustauthx.com',
     url="https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git",
     license="MIT",
```

### Comparing `trustauthx-0.7.0/trustauthx/authlite.py` & `trustauthx-0.7.1/trustauthx/authlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         response = requests.post(url, headers=headers, params=params, data=json.dumps(data))
         role_data = response.json()
         permissions = [Permission(**p) for p in role_data.get("permissions", [])]
         return AddRoleResponse(
             org_id=role_data.get("org_id"),
             rol_id=role_data.get("rol_id"),
             name=role_data.get("name"),
-            permissions=permissions
+            permissions=[p.__dict__ for p in permissions]
         )
 
     def delete_role(self, rol_id) -> DeleteRoleResponse:
 
         """
         Deletes a role with the specified role ID.
 
@@ -368,15 +368,15 @@
         response = requests.delete(url, headers=headers, params=params, data=json.dumps(data))
         role_data = response.json()
         permissions = [Permission(**p) for p in role_data.get("permissions", [])]
         return DeleteRoleResponse(
             org_id=role_data.get("org_id"),
             rol_id=role_data.get("rol_id"),
             name=role_data.get("name"),
-            permissions=permissions
+            permissions=[p.__dict__ for p in permissions]
         )
 
     def add_permission(self, rol_id, foreground=False, **Permission_) -> AddPermissionResponse:
         """
         Adds a new permission to a role with the specified role ID.
 
         Args:
@@ -409,20 +409,20 @@
         data = {
             "org_id": f'{self.org_id}',
             "rol_id": rol_id,
             "permissions": permissions
         }
         response = requests.post(url, headers=headers, params=params, data=json.dumps(data))
         response_data = response.json()
-        permissions = [{k: v} for k, v in permissions.items()]
+        permissions = [Permission(**{k: v}) for k, v in permissions.items()]
         self.reinitialize_all(foreground)
         return AddPermissionResponse(
             org_id=response_data.get("org_id"),
             rol_id=response_data.get("rol_id"),
-            permissions=permissions
+            permissions=[p.__dict__ for p in permissions]
         )
 
     def delete_permission(self, rol_id, foreground=False, **Permission_) -> DeletePermissionResponse:
         """
         Deletes a permission from a role with the specified role ID.
 
         Args:
```

### Comparing `trustauthx-0.7.0/trustauthx/cli.py` & `trustauthx-0.7.1/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.0/trustauthx/llmai.py` & `trustauthx-0.7.1/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.7.0/trustauthx/scheme.py` & `trustauthx-0.7.1/trustauthx/scheme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from dataclasses import dataclass, asdict
 from typing import List, Dict, Union
 
 @dataclass
 class Permission:
     """
     A class representing a permission object.
-
-    Attributes:
-        name (str): The name of the permission.
-        value (str): The value of the permission.
     """
-    name: str
-    value: str
+    def __init__(self, **kwargs):
+        for key, value in kwargs.items():
+            setattr(self, key, value)
 
 @dataclass
 class Role:
     """
     A class representing a role object.
 
     Attributes:
@@ -25,18 +22,14 @@
         permissions (List[Permission]): A list of permissions associated with the role.
     """
     org_id: str
     rol_id: str
     name: str
     permissions: List[Permission]
 
-@dataclass
-class Permission:
-    name: str
-    value: str
 
 @dataclass
 class GetAllRolesResponse:
     roles_list: List[Role]
     roles_json_list: List[Dict[str, Union[str, List[Dict[str, str]]]]]
 
 @dataclass
@@ -121,8 +114,25 @@
     rol_id="rol_rce_474ae9e59b3d49ce",
     permissions=[
         Permission(name="user", value="administration"),
         Permission(name="viewer", value="administration"),
         Permission(name="maintainer", value="administration")
     ]
 )
-"""
+"""
+
+# class Permission:
+#     def __init__(self, **kwargs):
+#         for key, value in kwargs.items():
+#             setattr(self, key, value)
+
+# role_data = {
+#     "permissions": [
+#         {"read": "true", "write": "false"},
+#         {"execute": "true"}
+#     ]
+# }
+
+# permissions = [Permission(**p) for p in role_data.get("permissions", [])]
+
+# for permission in permissions:
+#     print(permission.__dict__)
```

### Comparing `trustauthx-0.7.0/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.7.1/trustauthx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.7.0
+Version: 0.7.1
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

