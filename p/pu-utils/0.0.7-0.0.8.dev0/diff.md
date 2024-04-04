# Comparing `tmp/pu_utils-0.0.7-py3-none-any.whl.zip` & `tmp/pu_utils-0.0.8.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,18 @@
-Zip file size: 18925 bytes, number of entries: 13
--rw-r--r--  2.0 unx    14068 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/licenses/LICENSE
+Zip file size: 23178 bytes, number of entries: 16
+-rw-r--r--  2.0 unx    14073 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/WHEEL
+-rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/aws/__init__.py
--rw-r--r--  2.0 unx     5525 b- defN 16-Jan-01 00:00 pu_utils/aws/iam.py
+-rw-r--r--  2.0 unx      140 b- defN 16-Jan-01 00:00 pu_utils/aws/api/__init__.py
+-rw-r--r--  2.0 unx     6962 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_gateway.py
+-rw-r--r--  2.0 unx     5681 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_resource.py
+-rw-r--r--  2.0 unx     6317 b- defN 16-Jan-01 00:00 pu_utils/aws/iam.py
 -rw-r--r--  2.0 unx     3944 b- defN 16-Jan-01 00:00 pu_utils/aws/iam_test.py
--rw-r--r--  2.0 unx    14803 b- defN 16-Jan-01 00:00 pu_utils/aws/lambda_.py
--rw-r--r--  2.0 unx     1609 b- defN 16-Jan-01 00:00 pu_utils/namer.py
+-rw-r--r--  2.0 unx    14327 b- defN 16-Jan-01 00:00 pu_utils/aws/lambda_.py
+-rw-r--r--  2.0 unx     1620 b- defN 16-Jan-01 00:00 pu_utils/namer.py
 -rw-r--r--  2.0 unx     1437 b- defN 16-Jan-01 00:00 pu_utils/namer_test.py
 -rw-r--r--  2.0 unx     2754 b- defN 16-Jan-01 00:00 pu_utils/python_zip.py
 -rw-r--r--  2.0 unx     1773 b- defN 16-Jan-01 00:00 pu_utils/python_zip_test.py
-?rw-------  2.0 unx     1015 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/RECORD
-13 files, 58375 bytes uncompressed, 17249 bytes compressed:  70.5%
+?rw-------  2.0 unx     1290 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/RECORD
+16 files, 71765 bytes uncompressed, 21064 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,22 +1,31 @@
-Filename: pu_utils-0.0.7.dist-info/METADATA
+Filename: pu_utils-0.0.8.dev0.dist-info/METADATA
 Comment: 
 
-Filename: pu_utils-0.0.7.dist-info/WHEEL
+Filename: pu_utils-0.0.8.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: pu_utils-0.0.7.dist-info/licenses/LICENSE
+Filename: pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: pu_utils/__init__.py
 Comment: 
 
 Filename: pu_utils/aws/__init__.py
 Comment: 
 
+Filename: pu_utils/aws/api/__init__.py
+Comment: 
+
+Filename: pu_utils/aws/api/_gateway.py
+Comment: 
+
+Filename: pu_utils/aws/api/_resource.py
+Comment: 
+
 Filename: pu_utils/aws/iam.py
 Comment: 
 
 Filename: pu_utils/aws/iam_test.py
 Comment: 
 
 Filename: pu_utils/aws/lambda_.py
@@ -30,11 +39,11 @@
 
 Filename: pu_utils/python_zip.py
 Comment: 
 
 Filename: pu_utils/python_zip_test.py
 Comment: 
 
-Filename: pu_utils-0.0.7.dist-info/RECORD
+Filename: pu_utils-0.0.8.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pu_utils/aws/iam.py

```diff
@@ -1,26 +1,43 @@
 import json
 import os
 from collections.abc import Sequence
 from dataclasses import dataclass
 
-from pulumi import Input
+from pulumi import Input, Output, ResourceOptions
 from pulumi_aws.iam import (
-    AwaitableGetPolicyDocumentResult,
     GetPolicyDocumentStatementArgs,
     GetPolicyDocumentStatementPrincipalArgs,
     RoleInlinePolicyArgs,
     get_policy_document,
 )
+from pulumi_aws.lambda_ import Permission
 
 from pu_utils.namer import Namer
 
 AWS_REGION = os.environ["AWS_REGION"]
 
 
+def create_lambda_invoke_permission(
+    name: str,
+    function_name: Input[str],
+    gateway_execution_arn: Input[str],
+    path: Input[str] = "*/*",
+    opts: ResourceOptions | None = None,
+) -> Permission:
+    return Permission(
+        name,
+        action="lambda:invokeFunction",
+        function=function_name,
+        principal="apigateway.amazonaws.com",
+        source_arn=Output.concat(gateway_execution_arn, "/", path),
+        opts=opts,
+    )
+
+
 def policy_json(*, actions: Sequence[str], resource: str, allow: bool = True) -> str:
     return json.dumps(
         {
             "Version": "2012-10-17",
             "Statement": [
                 {
                     "Action": actions,
@@ -130,14 +147,25 @@
                 actions=[
                     "ses:SendEmail",
                 ],
                 resource=f"arn:aws:ses:{AWS_REGION}:{self.aws_account_id}:identity/{sender}",
             ),
         )
 
+    def sms_policy(self) -> RoleInlinePolicyArgs:
+        return RoleInlinePolicyArgs(
+            name=self.namer.role_policy("sms"),
+            policy=policy_json(
+                actions=[
+                    "sns:Publish",
+                ],
+                resource="*",
+            ),
+        )
+
     def kms_policy(self) -> RoleInlinePolicyArgs:
         resource = f"arn:aws:kms:{AWS_REGION}:{self.aws_account_id}:key/*"
         return RoleInlinePolicyArgs(
             name=self.namer.role_policy("kms"),
             policy=policy_json(
                 actions=[
                     "kms:GenerateDataKey",
```

## pu_utils/aws/lambda_.py

```diff
@@ -7,15 +7,14 @@
 from pulumi_aws.cloudwatch import LogGroup
 from pulumi_aws.iam import Role, RoleInlinePolicyArgs
 from pulumi_aws.lambda_ import (
     Function,
     FunctionEnvironmentArgs,
     FunctionVpcConfigArgs,
     LayerVersion,
-    Permission,
 )
 from pulumi_aws.s3 import BucketObjectv2
 
 from pu_utils.aws.iam import PolicyFactory, assume_role_policy
 from pu_utils.namer import Namer
 from pu_utils.python_zip import pip_install, zip_source
 
@@ -329,31 +328,14 @@
             source_code_hash=source_hash,
             compatible_architectures=architectures,
             compatible_runtimes=runtime,
             opts=ResourceOptions(parent=self),
         )
 
 
-def create_lambda_invoke_permission(
-    name: str,
-    function_name: Input[str],
-    gateway_execution_arn: Input[str],
-    path: Input[str] = "*/*",
-    opts: ResourceOptions | None = None,
-) -> Permission:
-    return Permission(
-        name,
-        action="lambda:invokeFunction",
-        function=function_name,
-        principal="apigateway.amazonaws.com",
-        source_arn=Output.concat(gateway_execution_arn, "/", path),
-        opts=opts,
-    )
-
-
 class ContainerLambda(ComponentResource):
     @property
     def name(self) -> Output[str]:
         return self._function.name
 
     @property
     def arn(self) -> Output[str]:
```

## pu_utils/namer.py

```diff
@@ -50,8 +50,8 @@
             self._prefix,
             self._stage,
             resource,
             self._region,
             self._instance,
             description,
         ]
-        return "-".join(filter(None, parts))
+        return "-".join(part for part in parts if part)
```

## Comparing `pu_utils-0.0.7.dist-info/METADATA` & `pu_utils-0.0.8.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pu-utils
-Version: 0.0.7
+Version: 0.0.8.dev0
 Summary: Random stuff to help writing Pulumi scripts easier
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `pu_utils-0.0.7.dist-info/licenses/LICENSE` & `pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pu_utils-0.0.7.dist-info/RECORD` & `pu_utils-0.0.8.dev0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-pu_utils-0.0.7.dist-info/METADATA,sha256=vckrpddv9r9F_2nysC-_yb5vD6-4Ng2HjE4j0ICKelQ,14068
-pu_utils-0.0.7.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
-pu_utils-0.0.7.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pu_utils-0.0.8.dev0.dist-info/METADATA,sha256=fuo5bFJ-daV89NEfvcrPcZjEEqtPC4zJKpsspiDPUrA,14073
+pu_utils-0.0.8.dev0.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
+pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 pu_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pu_utils/aws/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pu_utils/aws/iam.py,sha256=xWMQ2mmYd73uRg5JBO8MFSQcivcmD2c-5I4fDZi2ucY,5525
+pu_utils/aws/api/__init__.py,sha256=TbCCwI-R0z1U2nXJ2VyE4ORyBVhpPiel6i06AvnHDDo,140
+pu_utils/aws/api/_gateway.py,sha256=DtjeCUZvju-5RgVXDoGwn30CKaysDnzfWnDkx2dXxf8,6962
+pu_utils/aws/api/_resource.py,sha256=zYRiSL0ONOUqkgacEjKJwrT90zCF3OZrKQT31dxdzvs,5681
+pu_utils/aws/iam.py,sha256=HsnrzhncEQ81JxW-H22LKRNtBiPFjiuXcujxixAob7I,6317
 pu_utils/aws/iam_test.py,sha256=LNP-cegreyGK0osrVF1FDOdivByFuTukkKsIxt_SPM4,3944
-pu_utils/aws/lambda_.py,sha256=JLG0qitabpc-lR-cW8xvEXeucbCjh8cxuYC4bcdgWrM,14803
-pu_utils/namer.py,sha256=7Xo0eNtTBq3z1187yV4O7gcRnRTMsI0NiZ1QCDMNWqo,1609
+pu_utils/aws/lambda_.py,sha256=ZjW1NGaRrVvdK3cmz93dJEk5NeBlDD9lNhtuflUyCBY,14327
+pu_utils/namer.py,sha256=Ft94juGYhZF4Q1th6d_ZckMTHwfo_oZ7HWXOLhT4MtU,1620
 pu_utils/namer_test.py,sha256=rZ_hSe4Gz5lqtR9I5zYDdf7cohFlID2hmtMr88Lvva8,1437
 pu_utils/python_zip.py,sha256=VB1sHYsz1S28iYt9sjrUpjEkoiiX8HW7IzIFoe9SFog,2754
 pu_utils/python_zip_test.py,sha256=9iEiYI2zCHi3-sEVtF9Kws5kA7oGCdgpHS-Gntz-23Y,1773
-pu_utils-0.0.7.dist-info/RECORD,,
+pu_utils-0.0.8.dev0.dist-info/RECORD,,
```

