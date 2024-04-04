# Comparing `tmp/flowdapt_sdk-0.1.2-py3-none-any.whl.zip` & `tmp/flowdapt_sdk-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,33 +1,33 @@
-Zip file size: 21453 bytes, number of entries: 31
+Zip file size: 21396 bytes, number of entries: 31
 -rw-r--r--  2.0 unx      227 b- defN 80-Jan-01 00:00 flowdapt_sdk/__init__.py
 -rw-r--r--  2.0 unx     1885 b- defN 80-Jan-01 00:00 flowdapt_sdk/_compat.py
 -rw-r--r--  2.0 unx      418 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/__init__.py
 -rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/base.py
--rw-r--r--  2.0 unx     6537 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/configs.py
+-rw-r--r--  2.0 unx     6203 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/configs.py
 -rw-r--r--  2.0 unx     2162 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/metrics.py
 -rw-r--r--  2.0 unx     4194 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/plugins.py
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/system.py
 -rw-r--r--  2.0 unx     6445 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/triggers.py
 -rw-r--r--  2.0 unx    11208 b- defN 80-Jan-01 00:00 flowdapt_sdk/api/workflows.py
 -rw-r--r--  2.0 unx     8822 b- defN 80-Jan-01 00:00 flowdapt_sdk/client.py
 -rw-r--r--  2.0 unx       35 b- defN 80-Jan-01 00:00 flowdapt_sdk/constants.py
 -rw-r--r--  2.0 unx     3090 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/__init__.py
 -rw-r--r--  2.0 unx      204 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/base.py
--rw-r--r--  2.0 unx     2415 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/configs.py
+-rw-r--r--  2.0 unx     2180 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/configs.py
 -rw-r--r--  2.0 unx      610 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/error.py
 -rw-r--r--  2.0 unx     1365 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/metrics.py
 -rw-r--r--  2.0 unx     1030 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/plugin.py
 -rw-r--r--  2.0 unx      601 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/resource.py
 -rw-r--r--  2.0 unx     1493 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/system.py
 -rw-r--r--  2.0 unx     2336 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/triggers.py
 -rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 flowdapt_sdk/dto/workflows.py
 -rw-r--r--  2.0 unx     1249 b- defN 80-Jan-01 00:00 flowdapt_sdk/errors.py
 -rw-r--r--  2.0 unx     1842 b- defN 80-Jan-01 00:00 flowdapt_sdk/sdk.py
 -rw-r--r--  2.0 unx      172 b- defN 80-Jan-01 00:00 flowdapt_sdk/serialize.py
 -rw-r--r--  2.0 unx     2400 b- defN 80-Jan-01 00:00 flowdapt_sdk/utils.py
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 flowdapt_sdk/version.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2531 b- defN 16-Jan-01 00:00 flowdapt_sdk-0.1.2.dist-info/RECORD
-31 files, 71124 bytes uncompressed, 17415 bytes compressed:  75.5%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2531 b- defN 16-Jan-01 00:00 flowdapt_sdk-0.1.3.dist-info/RECORD
+31 files, 70555 bytes uncompressed, 17358 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: flowdapt_sdk/utils.py
 Comment: 
 
 Filename: flowdapt_sdk/version.py
 Comment: 
 
-Filename: flowdapt_sdk-0.1.2.dist-info/LICENSE
+Filename: flowdapt_sdk-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: flowdapt_sdk-0.1.2.dist-info/METADATA
+Filename: flowdapt_sdk-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: flowdapt_sdk-0.1.2.dist-info/WHEEL
+Filename: flowdapt_sdk-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: flowdapt_sdk-0.1.2.dist-info/RECORD
+Filename: flowdapt_sdk-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowdapt_sdk/api/configs.py

```diff
@@ -1,17 +1,14 @@
-from typing import Union
 from uuid import UUID
 
 from flowdapt_sdk._compat import validate_model, model_dump
 from flowdapt_sdk.api.base import BaseAPI
 from flowdapt_sdk.dto.configs import (
     V1Alpha1ConfigResourceCreateRequest,
     V1Alpha1ConfigResourceCreateResponse,
-    V1Alpha2ConfigResourceCreateRequest,
-    V1Alpha2ConfigResourceCreateResponse,
     V1Alpha1ConfigResourceUpdateRequest,
     V1Alpha1ConfigResourceUpdateResponse,
     V1Alpha1ConfigResourceReadResponse,
 )
 from flowdapt_sdk.constants import APIVersionHeader
 from flowdapt_sdk.utils import (
     build_request_data,
@@ -21,38 +18,28 @@
 ResourceType = "config"
 
 ConfigCreateRequestDTOs = {
     "v1alpha1": (
         V1Alpha1ConfigResourceCreateRequest,
         V1Alpha1ConfigResourceCreateResponse,
     ),
-    "v1alpha2": (
-        V1Alpha2ConfigResourceCreateRequest,
-        V1Alpha2ConfigResourceCreateResponse,
-    )
 }
 ConfigUpdateRequestDTOs = {
     "v1alpha1": (
         V1Alpha1ConfigResourceUpdateRequest,
         V1Alpha1ConfigResourceUpdateResponse,
     ),
 }
 ConfigReadRequestDTOs = {
     "v1alpha1": (None, V1Alpha1ConfigResourceReadResponse),
 }
 
 ConfigReadResponse = V1Alpha1ConfigResourceReadResponse
-ConfigCreateRequest = Union[
-    V1Alpha1ConfigResourceCreateRequest,
-    V1Alpha2ConfigResourceCreateRequest,
-]
-ConfigCreateResponse = Union[
-    V1Alpha1ConfigResourceCreateResponse,
-    V1Alpha2ConfigResourceCreateResponse,
-]
+ConfigCreateRequest = V1Alpha1ConfigResourceCreateRequest
+ConfigCreateResponse = V1Alpha1ConfigResourceCreateResponse
 ConfigUpdateRequest = V1Alpha1ConfigResourceUpdateRequest
 ConfigUpdateResponse = V1Alpha1ConfigResourceUpdateResponse
 
 
 class ConfigsAPI(BaseAPI):
     """
     The ConfigsAPI class provides methods for interacting with the Flowdapt Configs API.
```

## flowdapt_sdk/dto/configs.py

```diff
@@ -9,20 +9,14 @@
 
 
 class V1Alpha1ConfigSelectorType(Enum):
     name = 'name'
     annotation = 'annotation'
 
 
-class V1Alpha2ConfigSelector(BaseModel):
-    kind: Annotated[str | None, Field(title='Kind')] = None
-    type: V1Alpha1ConfigSelectorType | None = 'name'
-    value: Annotated[str | dict[str, str] | None, Field(title='Value')] = None
-
-
 class V1Alpha1ConfigSelector(BaseModel):
     kind: Annotated[str | None, Field(title='Kind')] = None
     type: V1Alpha1ConfigSelectorType | None = 'name'
     value: Annotated[str | dict[str, str] | None, Field(title='Value')] = None
 
 
 class V1Alpha1ConfigResourceSpec(BaseModel):
```

## Comparing `flowdapt_sdk-0.1.2.dist-info/LICENSE` & `flowdapt_sdk-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flowdapt_sdk-0.1.2.dist-info/METADATA` & `flowdapt_sdk-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowdapt_sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python SDK for Flowdapt
 Home-page: https://gitlab.com/emergentmethods/flowdapt-python-sdk
 License: MIT
 Author: Emergent Methods
 Author-email: contact@emergentmethods.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `flowdapt_sdk-0.1.2.dist-info/RECORD` & `flowdapt_sdk-0.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 flowdapt_sdk/__init__.py,sha256=RFWxkEJG3SpUmiQhcaSxZvIfdQysFdb7gCCqToMKc-0,227
 flowdapt_sdk/_compat.py,sha256=BY1dRLoyE22XsW4UoWZk7yIOKWlemprLGPqFl1G2rdE,1885
 flowdapt_sdk/api/__init__.py,sha256=QTZHblyMjjyoQfmMSIe1Qs7bc4N6wWpjTMelPTRrOw0,418
 flowdapt_sdk/api/base.py,sha256=wARM0r_8xvCUgAPy_b2FcDsdk73i1jcY3BcGRrnZLpg,139
-flowdapt_sdk/api/configs.py,sha256=SkDle8ColWW4Pa5zS_bSbeKduT9D61_1Gq_xEtzj6aU,6537
+flowdapt_sdk/api/configs.py,sha256=x0mgJ76SlqgkbVs8HUUe3X3_aBOV83eEMi6Do192CdE,6203
 flowdapt_sdk/api/metrics.py,sha256=wBzWDNurXXrLpwYxsiO1Pujtieyr34oz_Kp1wxjBTm8,2162
 flowdapt_sdk/api/plugins.py,sha256=0OIVYAam7J5F1pZfiGTUDAtDJRFJzqK0-YDPpM3C8OA,4194
 flowdapt_sdk/api/system.py,sha256=x3ebLpmTmRRUH9703nD7BVJlqn3t5d5kO0w83of21xg,1415
 flowdapt_sdk/api/triggers.py,sha256=FOp-OZv_3Oy822iK5eN_CEpwQhjDBDNSsTnNzDM42Q4,6445
 flowdapt_sdk/api/workflows.py,sha256=6VVYT_4DHeaCzXCLO0GQdrLuskotCKnmr476i0nISbs,11208
 flowdapt_sdk/client.py,sha256=SbcfuHyBsp6DGd62ldmrsC9CHMb8bJvO3-0nQ1l7MB0,8822
 flowdapt_sdk/constants.py,sha256=2Ou6j4B7zi9c7-oZLdLqzST7n6kIjnpUGdTvxJSLdDI,35
 flowdapt_sdk/dto/__init__.py,sha256=dLLcqEZW1geekwxAWkH53YoFssBQvOixIZk-NSSZ9vo,3090
 flowdapt_sdk/dto/base.py,sha256=u2yEe2lBSyu0cKHZbXrNRYkkNAZSd-kF9ai7fugxlVE,204
-flowdapt_sdk/dto/configs.py,sha256=CrcHEtLftiCkFZWTUNWACdqje8flDdCG9e4UDirvOpY,2415
+flowdapt_sdk/dto/configs.py,sha256=8zNXF14tOc_keQm8PZOwLdRsJBhqQ5eUSulQsRFlkZc,2180
 flowdapt_sdk/dto/error.py,sha256=FS3L_gu8CiKkuOxmxN-VIhV9r0aN6mps-1GSD0qXDO4,610
 flowdapt_sdk/dto/metrics.py,sha256=IeCosyosfaFHmBiCUe9LW5FjJZZWQDyBBpiIBDmVmms,1365
 flowdapt_sdk/dto/plugin.py,sha256=YP1I1nd7F1gQ-il-j4f987jsmxLx-82CQEr3APJX5vM,1030
 flowdapt_sdk/dto/resource.py,sha256=geCuTDSu-vNmh3JSs5iRMuRh6_voKqaUKvpoUnlzaPI,601
 flowdapt_sdk/dto/system.py,sha256=CqZMgpP_6ga_uwRCGouXhBySpAZWZQsIvmTXmDGc-uA,1493
 flowdapt_sdk/dto/triggers.py,sha256=nn8daHjEFLFJqhOfwtkdrhWR1RLWN8KVACt8uJ6YVQ4,2336
 flowdapt_sdk/dto/workflows.py,sha256=p2az4NptrlHqMjW9kbn3QNZVl_XLZaok-9A6M2rLa4w,3088
 flowdapt_sdk/errors.py,sha256=yTNgjfQNIZXBvt2MCBoGQSqdqud39pcnLgl6deFf6Dc,1249
 flowdapt_sdk/sdk.py,sha256=Adh-UwqykMIMZFiGc5xT5i8wPNMjRe8JHYdVcHpTbHo,1842
 flowdapt_sdk/serialize.py,sha256=KKc4AbAz_Bc9f_qzBcbJqU3HWnZidSK3-M-n7JHXEpo,172
 flowdapt_sdk/utils.py,sha256=7DMBCN63DoBK76auaTN_XUNprxrwd2NGUcNY0DGXpgk,2400
 flowdapt_sdk/version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
-flowdapt_sdk-0.1.2.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
-flowdapt_sdk-0.1.2.dist-info/METADATA,sha256=QECdIjo9yNJ7wcQraNehytX4v2XuOy57Qhl2v26NXMk,2028
-flowdapt_sdk-0.1.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-flowdapt_sdk-0.1.2.dist-info/RECORD,,
+flowdapt_sdk-0.1.3.dist-info/LICENSE,sha256=PphLPr74YBd3DwU0qher5XzGzcSJdOH9MYgApVO6wIo,1073
+flowdapt_sdk-0.1.3.dist-info/METADATA,sha256=GM3hRtK43dOBbLS_ItPt9QgUYcOOgxP7yN0jJtIIyus,2028
+flowdapt_sdk-0.1.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+flowdapt_sdk-0.1.3.dist-info/RECORD,,
```

