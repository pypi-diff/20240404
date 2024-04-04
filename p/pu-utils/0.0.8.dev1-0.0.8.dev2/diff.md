# Comparing `tmp/pu_utils-0.0.8.dev1-py3-none-any.whl.zip` & `tmp/pu_utils-0.0.8.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23170 bytes, number of entries: 16
--rw-r--r--  2.0 unx    14073 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE
+Zip file size: 23264 bytes, number of entries: 16
+-rw-r--r--  2.0 unx    14073 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev2.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev2.dist-info/WHEEL
+-rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev2.dist-info/licenses/LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/aws/__init__.py
 -rw-r--r--  2.0 unx      140 b- defN 16-Jan-01 00:00 pu_utils/aws/api/__init__.py
--rw-r--r--  2.0 unx     6953 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_gateway.py
--rw-r--r--  2.0 unx     5681 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_resource.py
+-rw-r--r--  2.0 unx     7528 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_gateway.py
+-rw-r--r--  2.0 unx     5636 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_resource.py
 -rw-r--r--  2.0 unx     6317 b- defN 16-Jan-01 00:00 pu_utils/aws/iam.py
 -rw-r--r--  2.0 unx     3944 b- defN 16-Jan-01 00:00 pu_utils/aws/iam_test.py
 -rw-r--r--  2.0 unx    14327 b- defN 16-Jan-01 00:00 pu_utils/aws/lambda_.py
 -rw-r--r--  2.0 unx     1620 b- defN 16-Jan-01 00:00 pu_utils/namer.py
 -rw-r--r--  2.0 unx     1437 b- defN 16-Jan-01 00:00 pu_utils/namer_test.py
 -rw-r--r--  2.0 unx     2754 b- defN 16-Jan-01 00:00 pu_utils/python_zip.py
 -rw-r--r--  2.0 unx     1773 b- defN 16-Jan-01 00:00 pu_utils/python_zip_test.py
-?rw-------  2.0 unx     1290 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/RECORD
-16 files, 71756 bytes uncompressed, 21056 bytes compressed:  70.7%
+?rw-------  2.0 unx     1290 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev2.dist-info/RECORD
+16 files, 72286 bytes uncompressed, 21150 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: pu_utils-0.0.8.dev1.dist-info/METADATA
+Filename: pu_utils-0.0.8.dev2.dist-info/METADATA
 Comment: 
 
-Filename: pu_utils-0.0.8.dev1.dist-info/WHEEL
+Filename: pu_utils-0.0.8.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE
+Filename: pu_utils-0.0.8.dev2.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: pu_utils/__init__.py
 Comment: 
 
 Filename: pu_utils/aws/__init__.py
 Comment: 
@@ -39,11 +39,11 @@
 
 Filename: pu_utils/python_zip.py
 Comment: 
 
 Filename: pu_utils/python_zip_test.py
 Comment: 
 
-Filename: pu_utils-0.0.8.dev1.dist-info/RECORD
+Filename: pu_utils-0.0.8.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pu_utils/aws/api/_gateway.py

```diff
@@ -17,34 +17,14 @@
 from pulumi_aws.lambda_ import Function
 
 from pu_utils.aws.api._resource import RestResourceNode, create_route
 from pu_utils.aws.iam import create_lambda_invoke_permission
 from pu_utils.namer import Namer
 
 
-def _authorizer_invoke_uri(arn: str) -> str:
-    region = os.environ["AWS_REGION"]
-    return f"arn:aws:apigateway:{region}:lambda:path/2015-03-31/functions/{arn}/invocations"
-
-
-def _deployment_hash() -> str:
-    return str(datetime.now(tz=UTC))
-
-
-def _collect_resources(root: RestResourceNode) -> list[Resource]:
-    stacks = [root]
-    resources = []
-    while stacks:
-        node = stacks.pop()
-        if node.resource:
-            resources.extend(node.resource.resources())
-        stacks.extend(node.children.values())
-    return resources
-
-
 class RestEndpoint(ComponentResource):
     """Create a lambda-backed REST API endpoint"""
 
     def __init__(
         self,
         name: str,
         path: str,
@@ -80,14 +60,17 @@
             uri=self.function.invoke_arn,
             rest_api=api_id,
             resource_id=resource_id,
             opts=ResourceOptions(parent=self),
         )
         self.register_outputs({})
 
+    def resources(self) -> list[Resource]:
+        return [self.integration, self.method]
+
 
 class RestGateway(ComponentResource):
     @property
     def id(self) -> Output[str]:
         return self._api.id
 
     @property
@@ -116,47 +99,53 @@
         self._authorizer = (
             self._create_authorizer(authorizer_func) if authorizer_func else None
         )
         self._root_resource = RestResourceNode(
             full_path="/",
             aws_resource_id=self._api.root_resource_id,
         )
+        self._endpoints = []
         # May also add catch-all route and return mock 404
 
     def add_endpoint(
         self,
         name: str,
         method: Literal["GET", "POST", "PUT", "PATCH", "DELETE"],
         path: str,
         function: Function,
         *,
         authorized: bool = True,
     ) -> None:
-        RestEndpoint(
-            name,
-            path=path,
-            resource_id=self._route_resource_id(path),
-            method=method,
-            api_id=self._api.id,
-            gateway_execution_arn=self._api.execution_arn,
-            function=function,
-            authorizer_id=self._authorizer.id
-            if authorized and self._authorizer
-            else None,
-            opts=ResourceOptions(parent=self),
+        self._endpoints.append(
+            RestEndpoint(
+                name,
+                path=path,
+                resource_id=self._route_resource_id(path),
+                method=method,
+                api_id=self._api.id,
+                gateway_execution_arn=self._api.execution_arn,
+                function=function,
+                authorizer_id=self._authorizer.id
+                if authorized and self._authorizer
+                else None,
+                opts=ResourceOptions(parent=self),
+            )
         )
 
     def finish(self, stage: Input[str]) -> None:
         deployment = Deployment(
             "api",
             rest_api=self._api.id,
             triggers={"redeployment": _deployment_hash()},
             opts=ResourceOptions(
                 parent=self,
-                depends_on=_collect_resources(self._root_resource),
+                depends_on=[
+                    *_collect_resources_from_resource_tree(self._root_resource),
+                    *_collect_resources_from_endpoints(self._endpoints),
+                ],
             ),
         )
         self.stage = Stage(
             "api",
             stage_name=stage,
             rest_api=self._api.id,
             deployment=deployment.id,
@@ -209,7 +198,34 @@
             api_id=self._api.id,
             path=path,
             parent=self,
         ).aws_resource_id
 
     def _export_outputs(self) -> None:
         export("gateway_stage_url", self.stage.invoke_url)
+
+
+def _authorizer_invoke_uri(arn: str) -> str:
+    region = os.environ["AWS_REGION"]
+    return f"arn:aws:apigateway:{region}:lambda:path/2015-03-31/functions/{arn}/invocations"
+
+
+def _deployment_hash() -> str:
+    return str(datetime.now(tz=UTC))
+
+
+def _collect_resources_from_endpoints(endpoints: list[RestEndpoint]) -> list[Resource]:
+    resources = []
+    for endpoint in endpoints:
+        resources.extend(endpoint.resources())
+    return resources
+
+
+def _collect_resources_from_resource_tree(root: RestResourceNode) -> list[Resource]:
+    stacks = [root]
+    resources = []
+    while stacks:
+        node = stacks.pop()
+        if node.resource:
+            resources.extend(node.resource.resources())
+        stacks.extend(node.children.values())
+    return resources
```

## pu_utils/aws/api/_resource.py

```diff
@@ -1,10 +1,9 @@
 import pulumi
 from pulumi import ComponentResource, Input, Output, ResourceOptions
-from pulumi import Resource as PulumiResource
 from pulumi_aws.apigateway import (
     Integration,
     IntegrationResponse,
     Method,
     MethodResponse,
     Resource,
 )
@@ -147,15 +146,15 @@
         self.children = {}
 
 
 def create_route(
     root: RestResourceNode,
     api_id: Input[str],
     path: str,
-    parent: PulumiResource,
+    parent: pulumi.Resource,
 ) -> RestResourceNode:
     """Create resources as needed to have `path` as an API endpoint"""
     node = root
     accumulated_segments = []
     for segment in path.removesuffix("/").removeprefix("/").split("/"):
         accumulated_segments.append(segment)
         res_name = "_".join(accumulated_segments)
```

## Comparing `pu_utils-0.0.8.dev1.dist-info/METADATA` & `pu_utils-0.0.8.dev2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pu-utils
-Version: 0.0.8.dev1
+Version: 0.0.8.dev2
 Summary: Random stuff to help writing Pulumi scripts easier
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE` & `pu_utils-0.0.8.dev2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pu_utils-0.0.8.dev1.dist-info/RECORD` & `pu_utils-0.0.8.dev2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pu_utils-0.0.8.dev1.dist-info/METADATA,sha256=jZWjkQOj154g8b7pNijgHJSXsIpe6f-5BQtIPzKmUTM,14073
-pu_utils-0.0.8.dev1.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
-pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pu_utils-0.0.8.dev2.dist-info/METADATA,sha256=x5lsDyxAht58g6FkmdkpbnWwcL92Cfk6T1rBXe4yPW4,14073
+pu_utils-0.0.8.dev2.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
+pu_utils-0.0.8.dev2.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 pu_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pu_utils/aws/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pu_utils/aws/api/__init__.py,sha256=TbCCwI-R0z1U2nXJ2VyE4ORyBVhpPiel6i06AvnHDDo,140
-pu_utils/aws/api/_gateway.py,sha256=M_XfVJr_-frDJPPIa3YtC_5qeBpGxRIzc1kEcvV9XeI,6953
-pu_utils/aws/api/_resource.py,sha256=zYRiSL0ONOUqkgacEjKJwrT90zCF3OZrKQT31dxdzvs,5681
+pu_utils/aws/api/_gateway.py,sha256=7hsB7Ixc1QVlgWaYxjdPmuwTZOiApnGUWZ3i-INcJqs,7528
+pu_utils/aws/api/_resource.py,sha256=EXK7_wsDootuB5KcYONq4PnwIO6cm9tjAwuYEhb9rzw,5636
 pu_utils/aws/iam.py,sha256=HsnrzhncEQ81JxW-H22LKRNtBiPFjiuXcujxixAob7I,6317
 pu_utils/aws/iam_test.py,sha256=LNP-cegreyGK0osrVF1FDOdivByFuTukkKsIxt_SPM4,3944
 pu_utils/aws/lambda_.py,sha256=ZjW1NGaRrVvdK3cmz93dJEk5NeBlDD9lNhtuflUyCBY,14327
 pu_utils/namer.py,sha256=Ft94juGYhZF4Q1th6d_ZckMTHwfo_oZ7HWXOLhT4MtU,1620
 pu_utils/namer_test.py,sha256=rZ_hSe4Gz5lqtR9I5zYDdf7cohFlID2hmtMr88Lvva8,1437
 pu_utils/python_zip.py,sha256=VB1sHYsz1S28iYt9sjrUpjEkoiiX8HW7IzIFoe9SFog,2754
 pu_utils/python_zip_test.py,sha256=9iEiYI2zCHi3-sEVtF9Kws5kA7oGCdgpHS-Gntz-23Y,1773
-pu_utils-0.0.8.dev1.dist-info/RECORD,,
+pu_utils-0.0.8.dev2.dist-info/RECORD,,
```

