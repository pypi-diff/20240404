# Comparing `tmp/lscsde_workspace_mgmt-0.1.2.tar.gz` & `tmp/lscsde_workspace_mgmt-0.1.3.tar.gz`

## Comparing `lscsde_workspace_mgmt-0.1.2.tar` & `lscsde_workspace_mgmt-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/.git
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/_version.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/exceptions.py
--rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/k8sio.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/managers.py
--rw-r--r--   0        0        0    12941 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/objects.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/.gitignore
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/LICENSE
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/README.md
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/.git
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/_version.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/exceptions.py
+-rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/k8sio.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/managers.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/models.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/objects.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/LICENSE
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/README.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 lscsde_workspace_mgmt-0.1.3/PKG-INFO
```

### Comparing `lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/exceptions.py` & `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/k8sio.py` & `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/k8sio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from logging import Logger
 from kubernetes_asyncio import client
 from kubernetes_asyncio.client.exceptions import ApiException
+from pydantic import TypeAdapter
+from .models import AnalyticsWorkspace, AnalyticsWorkspaceBinding
 from .exceptions import (
     InvalidParameterException,
     InvalidLabelFormatException
 )
 from .objects import (
     AnalyticsWorkspace,
     AnalyticsWorkspaceBinding,
     AnalyticsWorkspaceStatus,
     AnalyticsWorkspaceBindingStatus,
+    AnalyticsWorkspaceSpec,
+    AnalyticsWorkspaceBindingSpec,
     KubernetesHelper
 )
 from kubernetes_asyncio.client.models import (
     V1ObjectMeta,
     V1Pod,
     V1Volume,
     V1VolumeMount,
@@ -98,32 +102,33 @@
             version = self.version,
             namespace = namespace,
             plural = self.plural,
             name = name
         )
 
 class AnalyticsWorkspaceBindingClient(KubernetesNamespacedCustomClient):
+    adaptor = TypeAdapter(AnalyticsWorkspaceBinding)
     def __init__(self, k8s_api: client.CustomObjectsApi, log: Logger):
         super().__init__(
             k8s_api = k8s_api, 
             log = log, 
             group = "xlscsde.nhs.uk",
             version = "v1",
             plural = "analyticsworkspacebindings",
             kind = "AnalyticsWorkspaceBinding"
         )
 
     async def get(self, namespace, name):
         result = await super().get(namespace, name)
         print(result)
-        return AnalyticsWorkspaceBinding(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
     
     async def list(self, namespace, **kwargs):
         result = await super().list(namespace, **kwargs)
-        return [AnalyticsWorkspaceBinding(item, self.get_api_version(), self.kind) for item in result["items"]]
+        return [self.adaptor.validate_python(item) for item in result["items"]]
 
     
 
     async def list_by_username(self, namespace, username):
         helper = KubernetesHelper() 
         formatted_username = helper.format_as_label(username)
         no_label = await self.list(namespace = namespace, label_selector = f"!xlscsde.nhs.uk/username")
@@ -142,32 +147,35 @@
                         )
                 except InvalidLabelFormatException as ex:
                     self.log.error(f"Could not validate {item.metadata.name} due to a label format exception: {ex}")
 
         return await self.list(namespace = namespace, label_selector = f"xlscsde.nhs.uk/username={formatted_username}")
 
     async def create(self, body : AnalyticsWorkspaceBinding, append_label : bool = True):
-        contents = body.to_dictionary()
+        contents = self.adaptor.dump_python(body, by_alias=True)
         
         if append_label:
             contents["metadata"]["labels"]["xlscsde.nhs.uk/username"] = body.spec.username_as_label()
 
         result = await super().create(
             namespace = body.metadata.namespace,
             body = contents
         )
-        return AnalyticsWorkspaceBinding(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
 
     async def patch(self, namespace : str = None, name : str = None, patch_body : dict = None, body : AnalyticsWorkspaceBinding = None):
         if not patch_body:
             if not body:
                 raise InvalidParameterException("Either namespace, name and patch_body or body must be provided")
+            
+            spec_adapter = TypeAdapter(AnalyticsWorkspaceBindingSpec)
+            status_adapter = TypeAdapter(AnalyticsWorkspaceBindingStatus)
             patch_body = [
-                {"op": "replace", "path": "/spec", "value": body.spec.to_dictionary()},
-                {"op": "replace", "path": "/status", "value": body.status.to_dictionary()}
+                {"op": "replace", "path": "/spec", "value": spec_adapter.dump_python(body.spec, by_alias=True)},
+                {"op": "replace", "path": "/status", "value": status_adapter.dump_python(body.status, by_alias=True)}
             ]
 
         if not namespace:
             if not body:
                 raise InvalidParameterException("Either namespace, name and patch_body or body must be provided")
             namespace = body.metadata.namespace
 
@@ -177,36 +185,37 @@
             name = body.metadata.name
             
         result = await super().patch(
             namespace = namespace,
             name = name,
             body = patch_body
         )
-        return AnalyticsWorkspaceBinding(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
 
     async def patch_status(self, namespace : str, name : str, status : AnalyticsWorkspaceBindingStatus):
-        body = [{"op": "replace", "path": "/status", "value": status.to_dictionary()}] 
+        status_adapter = TypeAdapter(AnalyticsWorkspaceBindingStatus)
+        body = [{"op": "replace", "path": "/status", "value": status_adapter.dump_python(status, by_alias=True)}] 
         result = await super().patch_status(
             namespace = namespace,
             name = name,
             body = body
         )
-        return AnalyticsWorkspaceBinding(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
 
     async def replace(self, body : AnalyticsWorkspaceBinding, append_label : bool = True):
-        contents = body.to_dictionary()
+        contents = self.adaptor.dump_python(body, by_alias=True)
         if append_label:
             contents["metadata"]["labels"]["xlscsde.nhs.uk/username"] = body.spec.username_as_label()
 
         result = await super().replace(
             namespace = body.metadata.namespace,
             name = body.metadata.name,
             body = contents
         )
-        return AnalyticsWorkspaceBinding(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
     
     async def delete(self, body : AnalyticsWorkspaceBinding = None, namespace : str = None, name : str = None):
         if body:
             if not namespace:
                 namespace = body.metadata.namespace
             if not name:
                 name = body.metadata.name
@@ -224,31 +233,34 @@
         )
         return await super().delete(
             namespace = body.metadata.namespace,
             name = body.metadata.name
         )
 
 class AnalyticsWorkspaceClient(KubernetesNamespacedCustomClient):
+    adaptor = TypeAdapter(AnalyticsWorkspace)
+
     def __init__(self, k8s_api: client.CustomObjectsApi, log: Logger):
         super().__init__(
             k8s_api = k8s_api, 
             log = log, 
             group = "xlscsde.nhs.uk",
             version = "v1",
             plural = "analyticsworkspaces",
             kind = "AnalyticsWorkspace"
         )
         
     async def get(self, namespace, name):
         result = await super().get(namespace, name)
-        return AnalyticsWorkspace(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
     
     async def list(self, namespace, **kwargs):
         result = await super().list(namespace, **kwargs)
-        return [AnalyticsWorkspace(item, self.get_api_version(), self.kind) for item in result["items"]]
+        
+        return [self.adaptor.validate_python(item) for item in result["items"]]
     
     async def list_by_username(self, binding_client : AnalyticsWorkspaceBindingClient, namespace : str, username : str):
         bindings = await binding_client.list_by_username(
             namespace = namespace,
             username = username
             )
         bound_workspaces = list(set([x.spec.workspace for x in bindings]))
@@ -264,25 +276,29 @@
                     raise e    
         
         return workspaces     
             
     async def create(self, body : AnalyticsWorkspace):
         result = await super().create(
             namespace = body.metadata.namespace,
-            body = body.to_dictionary()
+            body = self.adaptor.dump_python(body, by_alias=True)
         )
-        return AnalyticsWorkspace(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
 
     async def patch(self, namespace : str = None, name : str = None, patch_body : dict = None, body : AnalyticsWorkspace = None):
         if not patch_body:
             if not body:
                 raise InvalidParameterException("Either namespace, name and patch_body or body must be provided")
+            
+            spec_adapter = TypeAdapter(AnalyticsWorkspaceSpec)
+            status_adapter = TypeAdapter(AnalyticsWorkspaceStatus)
+
             patch_body = [
-                {"op": "replace", "path": "/spec", "value": body.spec.to_dictionary()},
-                {"op": "replace", "path": "/status", "value": body.status.to_dictionary()}
+                {"op": "replace", "path": "/spec", "value": spec_adapter.dump_python(body.spec, by_alias=True)},
+                {"op": "replace", "path": "/status", "value": status_adapter.dump_python(body.status, by_alias=True)}
             ]
 
         if not namespace:
             if not body:
                 raise InvalidParameterException("Either namespace, name and patch_body or body must be provided")
             namespace = body.metadata.namespace
 
@@ -291,33 +307,37 @@
                 raise InvalidParameterException("Either namespace, name and patch_body or body must be provided")
             name = body.metadata.name
             
         result = await super().patch(
             namespace = namespace,
             name = name,
             body = patch_body
-        )
-        return AnalyticsWorkspace(result, self.get_api_version(), self.kind)
+        )        
+        
+        return self.adaptor.validate_python(result)
 
     async def patch_status(self, namespace : str, name : str, status : AnalyticsWorkspaceStatus):
-        body = [{"op": "replace", "path": "/status", "value": status.to_dictionary()}] 
+        status_adapter = TypeAdapter(AnalyticsWorkspaceStatus)
+        body = [{"op": "replace", "path": "/status", "value": status_adapter.dump_python(status, by_alias=True)}] 
         result = await super().patch_status(
             namespace = namespace,
             name = name,
             body = body
         )
-        return AnalyticsWorkspace(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
+
 
     async def replace(self, body : AnalyticsWorkspace):
         result = await super().replace(
             namespace = body.metadata.namespace,
             name = body.metadata.name,
-            body = body.to_dictionary()
+            body = self.adaptor.dump_python(body, by_alias=True)
         )
-        return AnalyticsWorkspace(result, self.get_api_version(), self.kind)
+        return self.adaptor.validate_python(result)
+        
     
     async def delete(self, body : AnalyticsWorkspace = None, namespace : str = None, name : str = None):
         if body:
             if not namespace:
                 namespace = body.metadata.namespace
             if not name:
                 name = body.metadata.name
```

### Comparing `lscsde_workspace_mgmt-0.1.2/src/lscsde_workspace_mgmt/managers.py` & `lscsde_workspace_mgmt-0.1.3/src/lscsde_workspace_mgmt/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
     PersistentVolumeClaimClient,
     V1ObjectMeta,
     V1Pod
 )
 
 from .objects import (
     AnalyticsWorkspace,
-    AnalyticsWorkspaceBinding
+    AnalyticsWorkspaceBinding,
+    AnalyticsWorkspaceConverter
 )
 
 from .exceptions import (
     WorkspaceNotFoundException
 )
 
 from kubernetes_asyncio.client import (
@@ -39,15 +40,16 @@
         return permitted_workspaces
 
     async def get_permitted_workspaces(self, namespace : str, username : str):
         permitted_workspaces = await self.get_workspaces_for_user(namespace, username)
         sorted_workspaces = sorted(
             permitted_workspaces.values(), key=lambda x: x.spec.display_name
         )
-        return [item.to_workspace_dict() for item in sorted_workspaces]
+        converter = AnalyticsWorkspaceConverter()
+        return [converter.to_workspace_dict(item) for item in sorted_workspaces]
         
     async def mount_workspace(self, pod : V1Pod, storage_class_name, mount_prefix, storage_prefix : str = "", read_only : bool = False, mount_path = ""):
         metadata : V1ObjectMeta = pod.metadata
         namespace = metadata.namespace
         name = metadata.name
         workspace_name = metadata.labels.get("workspace")
```

### Comparing `lscsde_workspace_mgmt-0.1.2/.gitignore` & `lscsde_workspace_mgmt-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.2/LICENSE` & `lscsde_workspace_mgmt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lscsde_workspace_mgmt-0.1.2/pyproject.toml` & `lscsde_workspace_mgmt-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 authors = [
   { name="Shaun Turner", email="shaun.turner1@nhs.net" },
 ]
 description = "LSCSDE Workspace Management" 
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
+  "pydantic",
   "kubernetes-asyncio",
   'importlib-metadata; python_version<"3.10"',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `lscsde_workspace_mgmt-0.1.2/PKG-INFO` & `lscsde_workspace_mgmt-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lscsde_workspace_mgmt
-Version: 0.1.2
+Version: 0.1.3
 Summary: LSCSDE Workspace Management
 Project-URL: Homepage, https://github.com/lsc-sde/py-lscsde-workspace-mgmt
 Project-URL: Issues, https://github.com/lsc-sde/py-lscsde-workspace-mgmt/issues
 Author-email: Shaun Turner <shaun.turner1@nhs.net>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: importlib-metadata; python_version < '3.10'
 Requires-Dist: kubernetes-asyncio
+Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # py-lscsde-workspace-mgmt
 Python Module for LSCSDE Workspace Management
 
 ## Developer Instructions
 ### Incrementing the version
```

