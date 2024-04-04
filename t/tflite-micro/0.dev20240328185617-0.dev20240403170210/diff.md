# Comparing `tmp/tflite_micro-0.dev20240328185617-cp311-cp311-manylinux_2_28_x86_64.whl.zip` & `tmp/tflite_micro-0.dev20240403170210-cp311-cp311-manylinux_2_28_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 775329 bytes, number of entries: 12
--r-xr-xr-x  2.0 unx     1241 b- defN 24-Mar-29 13:12 tflite_micro/__init__.py
--r-xr-xr-x  2.0 unx  3334672 b- defN 24-Mar-29 13:15 tflite_micro/python/tflite_micro/_runtime.so
--r-xr-xr-x  2.0 unx       45 b- defN 24-Mar-29 13:12 tflite_micro/python/tflite_micro/_version.py
--r-xr-xr-x  2.0 unx     1796 b- defN 24-Mar-29 13:12 tflite_micro/python/tflite_micro/postinstall_check.py
--r-xr-xr-x  2.0 unx     9906 b- defN 24-Mar-29 13:12 tflite_micro/python/tflite_micro/runtime.py
--r-xr-xr-x  2.0 unx     3164 b- defN 24-Mar-29 13:12 tflite_micro/python/tflite_micro/sine_float.tflite
--r-xr-xr-x  2.0 unx   629940 b- defN 24-Mar-29 13:12 tflite_micro/tensorflow/lite/python/schema_py_generated.py
--r-xr-xr-x  2.0 unx     1631 b- defN 24-Mar-29 13:12 tflite_micro/tensorflow/lite/python/schema_util.py
--r-xr-xr-x  2.0 unx    14383 b- defN 24-Mar-29 13:12 tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py
-?rw-------  2.0 unx      113 b- defN 24-Mar-29 13:15 tflite_micro-0.dev20240328185617.dist-info/WHEEL
-?rw-------  2.0 unx      478 b- defN 24-Mar-29 13:15 tflite_micro-0.dev20240328185617.dist-info/METADATA
-?rw-------  2.0 unx     1200 b- defN 24-Mar-29 13:15 tflite_micro-0.dev20240328185617.dist-info/RECORD
+-r-xr-xr-x  2.0 unx     1241 b- defN 24-Apr-04 13:12 tflite_micro/__init__.py
+-r-xr-xr-x  2.0 unx  3334672 b- defN 24-Apr-04 13:15 tflite_micro/python/tflite_micro/_runtime.so
+-r-xr-xr-x  2.0 unx       45 b- defN 24-Apr-04 13:12 tflite_micro/python/tflite_micro/_version.py
+-r-xr-xr-x  2.0 unx     1796 b- defN 24-Apr-04 13:12 tflite_micro/python/tflite_micro/postinstall_check.py
+-r-xr-xr-x  2.0 unx     9906 b- defN 24-Apr-04 13:12 tflite_micro/python/tflite_micro/runtime.py
+-r-xr-xr-x  2.0 unx     3164 b- defN 24-Apr-04 13:12 tflite_micro/python/tflite_micro/sine_float.tflite
+-r-xr-xr-x  2.0 unx   629940 b- defN 24-Apr-04 13:12 tflite_micro/tensorflow/lite/python/schema_py_generated.py
+-r-xr-xr-x  2.0 unx     1631 b- defN 24-Apr-04 13:12 tflite_micro/tensorflow/lite/python/schema_util.py
+-r-xr-xr-x  2.0 unx    14383 b- defN 24-Apr-04 13:12 tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py
+?rw-------  2.0 unx      113 b- defN 24-Apr-04 13:15 tflite_micro-0.dev20240403170210.dist-info/WHEEL
+?rw-------  2.0 unx      478 b- defN 24-Apr-04 13:15 tflite_micro-0.dev20240403170210.dist-info/METADATA
+?rw-------  2.0 unx     1200 b- defN 24-Apr-04 13:15 tflite_micro-0.dev20240403170210.dist-info/RECORD
 12 files, 3998569 bytes uncompressed, 773259 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -21,17 +21,17 @@
 
 Filename: tflite_micro/tensorflow/lite/python/schema_util.py
 Comment: 
 
 Filename: tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py
 Comment: 
 
-Filename: tflite_micro-0.dev20240328185617.dist-info/WHEEL
+Filename: tflite_micro-0.dev20240403170210.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_micro-0.dev20240328185617.dist-info/METADATA
+Filename: tflite_micro-0.dev20240403170210.dist-info/METADATA
 Comment: 
 
-Filename: tflite_micro-0.dev20240328185617.dist-info/RECORD
+Filename: tflite_micro-0.dev20240403170210.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_micro/python/tflite_micro/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.dev20240328185617-gbb4fc83"
+__version__ = "0.dev20240403170210-g7aa0d93"
```

## Comparing `tflite_micro-0.dev20240328185617.dist-info/RECORD` & `tflite_micro-0.dev20240403170210.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tflite_micro/__init__.py,sha256=fjz_YqLilIRTfAnsshkOiF_EJVVnq5-f8UpLHBSl7mg,1241
 tflite_micro/python/tflite_micro/_runtime.so,sha256=-T7ByVyapR3SNbhc9ZO702_0seeuQBjw5vZLVaNa-8k,3334672
-tflite_micro/python/tflite_micro/_version.py,sha256=Us5026Ocoe6Q5Rl4VfaF8zJ4Ny_8aao49eSv2AXSoYQ,45
+tflite_micro/python/tflite_micro/_version.py,sha256=BH0qrxaHHzdY8ZfafD0ldPqc-kLE5tJUFXZVmcNYuEM,45
 tflite_micro/python/tflite_micro/postinstall_check.py,sha256=txtw1er-0lCsMnicKOkRsP9RU0fZ73U6t2wGOE-D9wc,1796
 tflite_micro/python/tflite_micro/runtime.py,sha256=_AHamRV4YML5GuYfU1q_cfeeApAY_xbk6wMOE_OuEhU,9906
 tflite_micro/python/tflite_micro/sine_float.tflite,sha256=7pOYYxlco3zgY7GOFPuCqg2Y22WWukEJV1f2tWDaEHA,3164
 tflite_micro/tensorflow/lite/python/schema_py_generated.py,sha256=GJd_oEHr-w42H9CM5Qqo5Rv6C27-8WTcOYZFbaWcJQw,629940
 tflite_micro/tensorflow/lite/python/schema_util.py,sha256=M1LrSqMKK3e3SKsg-98ovSOkWO4-ly91FFu2JI32TZk,1631
 tflite_micro/tensorflow/lite/tools/flatbuffer_utils.py,sha256=whDjbHdpQx3_1fEue2Wb5GTqj1U2NrUvqWzK-kC65bA,14383
-tflite_micro-0.dev20240328185617.dist-info/METADATA,sha256=rRtItp8_3O2W7CVm65hFFoV8ZE3gXdYbsMC8Yl8vhZM,478
-tflite_micro-0.dev20240328185617.dist-info/RECORD,,
-tflite_micro-0.dev20240328185617.dist-info/WHEEL,sha256=qeKfpRMWEkf6-wLErlsQMeI6ob4StU6OQRW53pZ_1Pk,113
+tflite_micro-0.dev20240403170210.dist-info/METADATA,sha256=nE5y9KBs1BOZ1nOJi3XgG1drMi4ZaSIDJ0o034AUP9E,478
+tflite_micro-0.dev20240403170210.dist-info/RECORD,,
+tflite_micro-0.dev20240403170210.dist-info/WHEEL,sha256=qeKfpRMWEkf6-wLErlsQMeI6ob4StU6OQRW53pZ_1Pk,113
```

