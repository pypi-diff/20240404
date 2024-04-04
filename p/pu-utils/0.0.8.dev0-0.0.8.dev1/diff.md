# Comparing `tmp/pu_utils-0.0.8.dev0-py3-none-any.whl.zip` & `tmp/pu_utils-0.0.8.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 23178 bytes, number of entries: 16
--rw-r--r--  2.0 unx    14073 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/WHEEL
--rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE
+Zip file size: 23170 bytes, number of entries: 16
+-rw-r--r--  2.0 unx    14073 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/aws/__init__.py
 -rw-r--r--  2.0 unx      140 b- defN 16-Jan-01 00:00 pu_utils/aws/api/__init__.py
--rw-r--r--  2.0 unx     6962 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_gateway.py
+-rw-r--r--  2.0 unx     6953 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_gateway.py
 -rw-r--r--  2.0 unx     5681 b- defN 16-Jan-01 00:00 pu_utils/aws/api/_resource.py
 -rw-r--r--  2.0 unx     6317 b- defN 16-Jan-01 00:00 pu_utils/aws/iam.py
 -rw-r--r--  2.0 unx     3944 b- defN 16-Jan-01 00:00 pu_utils/aws/iam_test.py
 -rw-r--r--  2.0 unx    14327 b- defN 16-Jan-01 00:00 pu_utils/aws/lambda_.py
 -rw-r--r--  2.0 unx     1620 b- defN 16-Jan-01 00:00 pu_utils/namer.py
 -rw-r--r--  2.0 unx     1437 b- defN 16-Jan-01 00:00 pu_utils/namer_test.py
 -rw-r--r--  2.0 unx     2754 b- defN 16-Jan-01 00:00 pu_utils/python_zip.py
 -rw-r--r--  2.0 unx     1773 b- defN 16-Jan-01 00:00 pu_utils/python_zip_test.py
-?rw-------  2.0 unx     1290 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev0.dist-info/RECORD
-16 files, 71765 bytes uncompressed, 21064 bytes compressed:  70.6%
+?rw-------  2.0 unx     1290 b- defN 16-Jan-01 00:00 pu_utils-0.0.8.dev1.dist-info/RECORD
+16 files, 71756 bytes uncompressed, 21056 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: pu_utils-0.0.8.dev0.dist-info/METADATA
+Filename: pu_utils-0.0.8.dev1.dist-info/METADATA
 Comment: 
 
-Filename: pu_utils-0.0.8.dev0.dist-info/WHEEL
+Filename: pu_utils-0.0.8.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE
+Filename: pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE
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
 
-Filename: pu_utils-0.0.8.dev0.dist-info/RECORD
+Filename: pu_utils-0.0.8.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pu_utils/aws/api/_gateway.py

```diff
@@ -105,15 +105,15 @@
         """
         Create a REST Gateway (API Gateway v1)
 
         Set `gateway_id` to use existing gateway or leave it `None` to create a new one.
 
         `finish()` must be called after endpoints are added
         """
-        super().__init__("pulumi-lambda-api:index:RestGateway", name, None, opts)
+        super().__init__("pu-utils:index:RestGateway", name, None, opts)
 
         self._namer = namer
         self._api = self._find_or_create_api(gateway_id)
         self._authorizer = (
             self._create_authorizer(authorizer_func) if authorizer_func else None
         )
         self._root_resource = RestResourceNode(
```

## Comparing `pu_utils-0.0.8.dev0.dist-info/METADATA` & `pu_utils-0.0.8.dev1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pu-utils
-Version: 0.0.8.dev0
+Version: 0.0.8.dev1
 Summary: Random stuff to help writing Pulumi scripts easier
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE` & `pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pu_utils-0.0.8.dev0.dist-info/RECORD` & `pu_utils-0.0.8.dev1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pu_utils-0.0.8.dev0.dist-info/METADATA,sha256=fuo5bFJ-daV89NEfvcrPcZjEEqtPC4zJKpsspiDPUrA,14073
-pu_utils-0.0.8.dev0.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
-pu_utils-0.0.8.dev0.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pu_utils-0.0.8.dev1.dist-info/METADATA,sha256=jZWjkQOj154g8b7pNijgHJSXsIpe6f-5BQtIPzKmUTM,14073
+pu_utils-0.0.8.dev1.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
+pu_utils-0.0.8.dev1.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 pu_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pu_utils/aws/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pu_utils/aws/api/__init__.py,sha256=TbCCwI-R0z1U2nXJ2VyE4ORyBVhpPiel6i06AvnHDDo,140
-pu_utils/aws/api/_gateway.py,sha256=DtjeCUZvju-5RgVXDoGwn30CKaysDnzfWnDkx2dXxf8,6962
+pu_utils/aws/api/_gateway.py,sha256=M_XfVJr_-frDJPPIa3YtC_5qeBpGxRIzc1kEcvV9XeI,6953
 pu_utils/aws/api/_resource.py,sha256=zYRiSL0ONOUqkgacEjKJwrT90zCF3OZrKQT31dxdzvs,5681
 pu_utils/aws/iam.py,sha256=HsnrzhncEQ81JxW-H22LKRNtBiPFjiuXcujxixAob7I,6317
 pu_utils/aws/iam_test.py,sha256=LNP-cegreyGK0osrVF1FDOdivByFuTukkKsIxt_SPM4,3944
 pu_utils/aws/lambda_.py,sha256=ZjW1NGaRrVvdK3cmz93dJEk5NeBlDD9lNhtuflUyCBY,14327
 pu_utils/namer.py,sha256=Ft94juGYhZF4Q1th6d_ZckMTHwfo_oZ7HWXOLhT4MtU,1620
 pu_utils/namer_test.py,sha256=rZ_hSe4Gz5lqtR9I5zYDdf7cohFlID2hmtMr88Lvva8,1437
 pu_utils/python_zip.py,sha256=VB1sHYsz1S28iYt9sjrUpjEkoiiX8HW7IzIFoe9SFog,2754
 pu_utils/python_zip_test.py,sha256=9iEiYI2zCHi3-sEVtF9Kws5kA7oGCdgpHS-Gntz-23Y,1773
-pu_utils-0.0.8.dev0.dist-info/RECORD,,
+pu_utils-0.0.8.dev1.dist-info/RECORD,,
```

