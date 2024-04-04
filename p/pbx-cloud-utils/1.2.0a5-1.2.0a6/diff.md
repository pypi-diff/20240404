# Comparing `tmp/pbx_cloud_utils-1.2.0a5-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.2.0a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7109 bytes, number of entries: 10
+Zip file size: 7160 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 08:55 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    11798 b- defN 24-Apr-04 11:29 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx    11956 b- defN 24-Apr-04 11:56 cloud_utils/aio_storage.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-10 08:55 cloud_utils/exceptions.py
 -rw-r--r--  2.0 unx     9825 b- defN 24-Apr-02 13:37 cloud_utils/storage.py
 -rw-r--r--  2.0 unx     1258 b- defN 24-Apr-04 11:29 cloud_utils/types.py
 -rw-r--r--  2.0 unx      346 b- defN 23-May-10 08:55 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-04 11:31 pbx_cloud_utils-1.2.0a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 11:31 pbx_cloud_utils-1.2.0a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 11:31 pbx_cloud_utils-1.2.0a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      811 b- defN 24-Apr-04 11:31 pbx_cloud_utils-1.2.0a5.dist-info/RECORD
-10 files, 24750 bytes uncompressed, 5719 bytes compressed:  76.9%
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      811 b- defN 24-Apr-04 11:59 pbx_cloud_utils-1.2.0a6.dist-info/RECORD
+10 files, 24908 bytes uncompressed, 5770 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a5.dist-info/METADATA
+Filename: pbx_cloud_utils-1.2.0a6.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a5.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.2.0a6.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a5.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.2.0a6.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a5.dist-info/RECORD
+Filename: pbx_cloud_utils-1.2.0a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/aio_storage.py

```diff
@@ -320,15 +320,18 @@
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
     ):
         session = aiobotocore.session.get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
-            return await client.put_object(
+            obj = await client.put_object(
                 ACL=self.provider_acl_map[acl.name],
                 Body=content.getvalue(),
                 Bucket=self.bucket_name,
                 Key=key,
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 ContentType=mimetype,
             )
+        # aiobotocore doesn't support changing storage class on gcs
+        await self.change_storage_class(key, target_storage_class, acl)
+        return obj
```

