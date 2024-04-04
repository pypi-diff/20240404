# Comparing `tmp/ovos_translate_plugin_nllb-0.0.0a2-py3-none-any.whl.zip` & `tmp/ovos_translate_plugin_nllb-0.0.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9869 bytes, number of entries: 8
--rw-r--r--  2.0 unx    11621 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb/version.py
--rw-r--r--  2.0 unx    11347 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb-0.0.0a2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1015 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb-0.0.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb-0.0.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      104 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb-0.0.0a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb-0.0.0a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      798 b- defN 23-Aug-21 23:05 ovos_translate_plugin_nllb-0.0.0a2.dist-info/RECORD
-8 files, 25181 bytes uncompressed, 8439 bytes compressed:  66.5%
+Zip file size: 9878 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    11625 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb/version.py
+-rw-r--r--  2.0 unx    11347 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb-0.0.0a3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1015 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb-0.0.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb-0.0.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      104 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb-0.0.0a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb-0.0.0a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      798 b- defN 24-Apr-04 15:01 ovos_translate_plugin_nllb-0.0.0a3.dist-info/RECORD
+8 files, 25185 bytes uncompressed, 8448 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_translate_plugin_nllb/__init__.py
 Comment: 
 
 Filename: ovos_translate_plugin_nllb/version.py
 Comment: 
 
-Filename: ovos_translate_plugin_nllb-0.0.0a2.dist-info/LICENSE
+Filename: ovos_translate_plugin_nllb-0.0.0a3.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_translate_plugin_nllb-0.0.0a2.dist-info/METADATA
+Filename: ovos_translate_plugin_nllb-0.0.0a3.dist-info/METADATA
 Comment: 
 
-Filename: ovos_translate_plugin_nllb-0.0.0a2.dist-info/WHEEL
+Filename: ovos_translate_plugin_nllb-0.0.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_translate_plugin_nllb-0.0.0a2.dist-info/entry_points.txt
+Filename: ovos_translate_plugin_nllb-0.0.0a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_translate_plugin_nllb-0.0.0a2.dist-info/top_level.txt
+Filename: ovos_translate_plugin_nllb-0.0.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_translate_plugin_nllb-0.0.0a2.dist-info/RECORD
+Filename: ovos_translate_plugin_nllb-0.0.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_translate_plugin_nllb/__init__.py

```diff
@@ -10,15 +10,15 @@
     LanguageTranslator
 )
 from ovos_utils.log import LOG
 from ovos_utils.xdg_utils import xdg_data_home
 
 
 class NLLB200Translator(LanguageTranslator):
-    __base_url = "https://pretrained-nmt-models.s3.us-west-2.amazonaws.com/CTranslate2/nllb"
+    __base_url = "https://pretrained-nmt-models.s3.us-west-004.backblazeb2.com/CTranslate2/nllb"
 
     MODEL_URLS = {
         "nllb-200_600M_int8": f"{__base_url}/nllb-200_600M_int8_ct2.zip",
         "nllb-200_1.2B_int8": f"{__base_url}/nllb-200_1.2B_int8_ct2.zip",
         "nllb-200-3.3B-int8": f"{__base_url}/nllb-200_3.3B_int8_ct2.zip",
         "flores200_sacrebleu_tokenizer_spm": f"{__base_url}/flores200_sacrebleu_tokenizer_spm.model"
     }
```

## ovos_translate_plugin_nllb/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 0
-VERSION_ALPHA = 2
+VERSION_ALPHA = 3
 # END_VERSION_BLOCK
```

## Comparing `ovos_translate_plugin_nllb-0.0.0a2.dist-info/LICENSE` & `ovos_translate_plugin_nllb-0.0.0a3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_translate_plugin_nllb-0.0.0a2.dist-info/METADATA` & `ovos_translate_plugin_nllb-0.0.0a3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-translate-plugin-nllb
-Version: 0.0.0a2
+Version: 0.0.0a3
 Summary: OVOS translation module for No Language Left Behind
 Home-page: https://github.com/OpenVoiceOS/ovos-translate-plugin-nllb
 Author: jarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `ovos_translate_plugin_nllb-0.0.0a2.dist-info/RECORD` & `ovos_translate_plugin_nllb-0.0.0a3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ovos_translate_plugin_nllb/__init__.py,sha256=yZErRVPUY9XVp0lbY7T_d9Z12E7VG4dXLcDtgM5rHBg,11621
-ovos_translate_plugin_nllb/version.py,sha256=qbOVTdDXh7dwDi60rr2DZTzYPxPV2NRmIEkMGRkodnk,177
-ovos_translate_plugin_nllb-0.0.0a2.dist-info/LICENSE,sha256=RXUFLO6ywCoDqy1m8f12aYd4p5MxELJ5xnYC9PfK3lw,11347
-ovos_translate_plugin_nllb-0.0.0a2.dist-info/METADATA,sha256=0rQvXK4i7GCN-1Fd44KAfzGCiS_w01uTNuixLiEEWpU,1015
-ovos_translate_plugin_nllb-0.0.0a2.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
-ovos_translate_plugin_nllb-0.0.0a2.dist-info/entry_points.txt,sha256=I7_QXvq2mZRzGIOtY30VeECysBc_iABx3E72WRgYr7s,104
-ovos_translate_plugin_nllb-0.0.0a2.dist-info/top_level.txt,sha256=2BPje71yj14X-vs01eI6zGYKm5CCroJ9-VVAY7LZVJY,27
-ovos_translate_plugin_nllb-0.0.0a2.dist-info/RECORD,,
+ovos_translate_plugin_nllb/__init__.py,sha256=KeMPP-tKkbDw0B3XtWyOXsVw1TC5k6_GtdMlkgoDqFc,11625
+ovos_translate_plugin_nllb/version.py,sha256=mdTwoA3M5jrv1DgpMMdhUkhzeydBmSNmT4F8k_15_Ug,177
+ovos_translate_plugin_nllb-0.0.0a3.dist-info/LICENSE,sha256=RXUFLO6ywCoDqy1m8f12aYd4p5MxELJ5xnYC9PfK3lw,11347
+ovos_translate_plugin_nllb-0.0.0a3.dist-info/METADATA,sha256=SstIW1P2r3rFWyPYCkj619_BiXaf65y8Q_8FmjE081o,1015
+ovos_translate_plugin_nllb-0.0.0a3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ovos_translate_plugin_nllb-0.0.0a3.dist-info/entry_points.txt,sha256=I7_QXvq2mZRzGIOtY30VeECysBc_iABx3E72WRgYr7s,104
+ovos_translate_plugin_nllb-0.0.0a3.dist-info/top_level.txt,sha256=2BPje71yj14X-vs01eI6zGYKm5CCroJ9-VVAY7LZVJY,27
+ovos_translate_plugin_nllb-0.0.0a3.dist-info/RECORD,,
```

