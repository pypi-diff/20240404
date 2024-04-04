# Comparing `tmp/yowasp_wavedrom-3.5.0.1-py3-none-any.whl.zip` & `tmp/yowasp_wavedrom-3.5.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 40624 bytes, number of entries: 7
--rw-r--r--  2.0 unx      750 b- defN 24-Apr-04 17:14 yowasp_wavedrom/__init__.py
--rw-r--r--  2.0 unx   392672 b- defN 24-Apr-04 17:14 yowasp_wavedrom/bundle.js
--rw-r--r--  2.0 unx     3125 b- defN 24-Apr-04 17:15 yowasp_wavedrom-3.5.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 17:15 yowasp_wavedrom-3.5.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 17:15 yowasp_wavedrom-3.5.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-04 17:15 yowasp_wavedrom-3.5.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      610 b- defN 24-Apr-04 17:15 yowasp_wavedrom-3.5.0.1.dist-info/RECORD
-7 files, 397327 bytes uncompressed, 39530 bytes compressed:  90.1%
+Zip file size: 40646 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-04 17:25 yowasp_wavedrom/__init__.py
+-rw-r--r--  2.0 unx   392672 b- defN 24-Apr-04 17:25 yowasp_wavedrom/bundle.js
+-rw-r--r--  2.0 unx     3125 b- defN 24-Apr-04 17:25 yowasp_wavedrom-3.5.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 17:25 yowasp_wavedrom-3.5.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-04 17:25 yowasp_wavedrom-3.5.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-04 17:25 yowasp_wavedrom-3.5.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      610 b- defN 24-Apr-04 17:25 yowasp_wavedrom-3.5.0.2.dist-info/RECORD
+7 files, 397410 bytes uncompressed, 39552 bytes compressed:  90.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: yowasp_wavedrom/__init__.py
 Comment: 
 
 Filename: yowasp_wavedrom/bundle.js
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.1.dist-info/METADATA
+Filename: yowasp_wavedrom-3.5.0.2.dist-info/METADATA
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.1.dist-info/WHEEL
+Filename: yowasp_wavedrom-3.5.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.1.dist-info/entry_points.txt
+Filename: yowasp_wavedrom-3.5.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.1.dist-info/top_level.txt
+Filename: yowasp_wavedrom-3.5.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.1.dist-info/RECORD
+Filename: yowasp_wavedrom-3.5.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yowasp_wavedrom/__init__.py

```diff
@@ -1,12 +1,15 @@
 import sys
 import json
 import pathlib
 import quickjs
-import importlib_resources
+try:
+    import importlib.resources as importlib_resources
+except ImportError:
+    import importlib_resources
 
 
 def render(source):
     ctx = quickjs.Context()
     ctx.set("module", ctx.globalThis)
     ctx.eval((importlib_resources.files() /  "bundle.js").read_text())
     return ctx.eval("render(" + json.dumps(source) + ")")
```

## Comparing `yowasp_wavedrom-3.5.0.1.dist-info/METADATA` & `yowasp_wavedrom-3.5.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yowasp-wavedrom
-Version: 3.5.0.1
+Version: 3.5.0.2
 Summary: WaveDrom generates diagrams for digital waveforms, bit fields, and simple combinational circuits
 Author-email: Catherine <whitequark@whitequark.org>
 License: MIT
 Project-URL: Homepage, https://yowasp.org/
 Project-URL: Source Code, https://github.com/YoWASP/wavedrom
 Project-URL: Bug Tracker, https://github.com/YoWASP/wavedrom/issues
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `yowasp_wavedrom-3.5.0.1.dist-info/RECORD` & `yowasp_wavedrom-3.5.0.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-yowasp_wavedrom/__init__.py,sha256=HKMk-kQSfFYCsvb5DArUIIcDzpRtCgtlmbZZW2kXXbc,750
+yowasp_wavedrom/__init__.py,sha256=M3wtclsOskxI9kcM3LeB-kq8PxkRIrH3RYpXHQkGmns,833
 yowasp_wavedrom/bundle.js,sha256=mUTijLUykc-iz020AqiPa5NQJlfabkLkL6gFfnUOwNg,392672
-yowasp_wavedrom-3.5.0.1.dist-info/METADATA,sha256=cXw-vkVkwGzVvpWTGc58RT-IR23UJL2lhSmUkZKZXl4,3125
-yowasp_wavedrom-3.5.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-yowasp_wavedrom-3.5.0.1.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
-yowasp_wavedrom-3.5.0.1.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
-yowasp_wavedrom-3.5.0.1.dist-info/RECORD,,
+yowasp_wavedrom-3.5.0.2.dist-info/METADATA,sha256=U24Zb-YtbjNBmEPH3hY0jzBlPLUr5HP-dHNzQe-QvhE,3125
+yowasp_wavedrom-3.5.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+yowasp_wavedrom-3.5.0.2.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
+yowasp_wavedrom-3.5.0.2.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
+yowasp_wavedrom-3.5.0.2.dist-info/RECORD,,
```

