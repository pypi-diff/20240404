# Comparing `tmp/pbx_cloud_utils-1.2.0a3-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.2.0a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7065 bytes, number of entries: 10
+Zip file size: 7094 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 08:55 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    11695 b- defN 24-Apr-03 12:59 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx    11798 b- defN 24-Apr-04 10:07 cloud_utils/aio_storage.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-10 08:55 cloud_utils/exceptions.py
 -rw-r--r--  2.0 unx     9825 b- defN 24-Apr-02 13:37 cloud_utils/storage.py
--rw-r--r--  2.0 unx     1261 b- defN 24-Apr-02 13:41 cloud_utils/types.py
+-rw-r--r--  2.0 unx     1261 b- defN 24-Apr-04 10:05 cloud_utils/types.py
 -rw-r--r--  2.0 unx      346 b- defN 23-May-10 08:55 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      811 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/RECORD
-10 files, 24650 bytes uncompressed, 5675 bytes compressed:  77.0%
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-04 10:10 pbx_cloud_utils-1.2.0a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 10:10 pbx_cloud_utils-1.2.0a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 10:10 pbx_cloud_utils-1.2.0a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      811 b- defN 24-Apr-04 10:10 pbx_cloud_utils-1.2.0a4.dist-info/RECORD
+10 files, 24753 bytes uncompressed, 5704 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a3.dist-info/METADATA
+Filename: pbx_cloud_utils-1.2.0a4.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a3.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.2.0a4.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a3.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.2.0a4.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a3.dist-info/RECORD
+Filename: pbx_cloud_utils-1.2.0a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/aio_storage.py

```diff
@@ -127,29 +127,29 @@
         self,
         key: str,
         target_storage_class: PbxStorageClass,
         acl: PbxACL = PbxACL.PUBLIC_READ,
     ):
         session = aiobotocore.session.get_session()
         async with session.create_client("s3", self.region_name) as client:
-            client.copy_object(
+            await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 MetadataDirective="COPY",
             )
 
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
         session = aiobotocore.session.get_session()
         async with session.create_client("s3", self.region_name) as client:
-            client.copy_object(
+            await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=target_key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 MetadataDirective="COPY",
             )
 
@@ -248,22 +248,23 @@
 
 class AsyncGoogleCloudStorage(AsyncStorage):
     provider_storage_class_map: dict[str, str] = gcs_storage_class_map
     provider_acl_map: dict[str, str] = gcs_acl_map
     bucket_client: gcs_storage.Bucket
     endpoint_url: str
 
-    def __init__(self, gcs_project_id: str, endpoint_url: str, *args, **kwargs):
+    def __init__(self, endpoint_url: str, gcs_project_id: str = "", *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.gcs_project = gcs_project_id or os.environ.get("GCS_PROJECT_ID")
         gcs_storage_client_kwargs = {
             key.removeprefix("gcs_"): value
             for key, value in kwargs.items()
             if key.startswith("gcs_")
         }
-        client = gcs_storage.Client(project=gcs_project_id, **gcs_storage_client_kwargs)
+        client = gcs_storage.Client(project=self.gcs_project, **gcs_storage_client_kwargs)
         bucket = client.bucket(self.bucket_name)
         self.bucket_client = bucket
         self.endpoint_url = endpoint_url
 
     async def delete_object(self, key: str) -> None:
         raise NotImplementedError()
 
@@ -286,15 +287,15 @@
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
         session = aiobotocore.session.get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
-            client.copy_object(
+            await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=target_key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 MetadataDirective="COPY",
             )
```

## Comparing `pbx_cloud_utils-1.2.0a3.dist-info/RECORD` & `pbx_cloud_utils-1.2.0a4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cloud_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cloud_utils/aio_storage.py,sha256=Wr_DW-xpMGCV4I4pdy4xtKzpZYS6TihJJwzg6J2AV58,11695
+cloud_utils/aio_storage.py,sha256=xD1-IkQYH4htmuXVRVJcgHkPefwcr7lE61inGccL21Y,11798
 cloud_utils/exceptions.py,sha256=4TFl0EqL8X2vEgs4xpNgev93bDMcawfVc9DAty7SAqw,284
 cloud_utils/storage.py,sha256=QPvy35b-Y4WZrZ6H_yWXwsra_g9uruHHO0q37U-SyT8,9825
 cloud_utils/types.py,sha256=_tLXnVfC4SGw3t-rawmgjAPjeqImtW4WhsiMoSqIYkU,1261
 cloud_utils/utils.py,sha256=gi__PPdP5YKxehoe9Az5lhAgN11sFxk3YLmHM0cxm1I,346
-pbx_cloud_utils-1.2.0a3.dist-info/METADATA,sha256=ihzvbvUpmDNC4sd5L2Qpl4NUQvMc121Kfu2GkZMekIY,324
-pbx_cloud_utils-1.2.0a3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pbx_cloud_utils-1.2.0a3.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
-pbx_cloud_utils-1.2.0a3.dist-info/RECORD,,
+pbx_cloud_utils-1.2.0a4.dist-info/METADATA,sha256=t5EcI5XyzdBlBfLyVuU_Vhrnl_OSgIH1e3Y-3zpHgCI,324
+pbx_cloud_utils-1.2.0a4.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+pbx_cloud_utils-1.2.0a4.dist-info/top_level.txt,sha256=zcaARuOP8yoOZ9pwOjV7p4206IX9CFMTKA_QPvxCtvA,12
+pbx_cloud_utils-1.2.0a4.dist-info/RECORD,,
```

