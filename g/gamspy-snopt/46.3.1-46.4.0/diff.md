# Comparing `tmp/gamspy_snopt-46.3.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_snopt-46.4.0-py3-none-manylinux_2_17_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 583366 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      357 b- defN 24-Mar-28 19:10 gamspy_snopt/__init__.py
--rw-rw-rw-  2.0 fat     6967 b- defN 24-Mar-28 19:10 gamspy_snopt/optsnopt.def
--rw-rw-rw-  2.0 fat  1416704 b- defN 24-Mar-28 19:10 gamspy_snopt/snlcclib64.dll
--rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-28 19:10 gamspy_snopt/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Mar-28 19:10 gamspy_snopt-46.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-28 19:10 gamspy_snopt-46.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Mar-28 19:10 gamspy_snopt-46.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      648 b- defN 24-Mar-28 19:10 gamspy_snopt-46.3.1.dist-info/RECORD
-8 files, 1424877 bytes uncompressed, 582234 bytes compressed:  59.1%
+Zip file size: 352465 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      350 b- defN 24-Apr-04 14:14 gamspy_snopt/__init__.py
+-rwxrwxrwx  2.0 unx  1005064 b- defN 24-Apr-04 14:14 gamspy_snopt/libsnlcclib64.so
+-rwxrwxrwx  2.0 unx     6967 b- defN 24-Apr-04 14:14 gamspy_snopt/optsnopt.def
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-04 14:14 gamspy_snopt/version.py
+-rw-r--r--  2.0 unx       58 b- defN 24-Apr-04 14:14 gamspy_snopt-46.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      116 b- defN 24-Apr-04 14:14 gamspy_snopt-46.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-04 14:14 gamspy_snopt-46.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      650 b- defN 24-Apr-04 14:14 gamspy_snopt-46.4.0.dist-info/RECORD
+8 files, 1013240 bytes uncompressed, 351329 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: gamspy_snopt/__init__.py
 Comment: 
 
-Filename: gamspy_snopt/optsnopt.def
+Filename: gamspy_snopt/libsnlcclib64.so
 Comment: 
 
-Filename: gamspy_snopt/snlcclib64.dll
+Filename: gamspy_snopt/optsnopt.def
 Comment: 
 
 Filename: gamspy_snopt/version.py
 Comment: 
 
-Filename: gamspy_snopt-46.3.1.dist-info/METADATA
+Filename: gamspy_snopt-46.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_snopt-46.3.1.dist-info/WHEEL
+Filename: gamspy_snopt-46.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_snopt-46.3.1.dist-info/top_level.txt
+Filename: gamspy_snopt-46.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_snopt-46.3.1.dist-info/RECORD
+Filename: gamspy_snopt-46.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_snopt/__init__.py

```diff
@@ -1,11 +1,11 @@
-import os
-from pathlib import Path
-
-from .version import __version__
-
-directory = str(Path(__file__).resolve().parent)
-
-files = ['snlcclib64.dll', 'optsnopt.def']
-
-file_paths = [directory + os.sep + file for file in files]
-verbatim = 'SNOPT 1 0 SN 1 0 2 LP RMIP NLP CNS DNLP RMINLP QCP RMIQCP\ngmsgennt.cmd\ngmsgennx.exe\nsnlcclib64.dll snl 1 0'
+import os
+from pathlib import Path
+
+from .version import __version__
+
+directory = str(Path(__file__).resolve().parent)
+
+files = ['libsnlcclib64.so', 'optsnopt.def']
+
+file_paths = [directory + os.sep + file for file in files]
+verbatim = 'SNOPT 1 0 SN 1 0 2 LP RMIP NLP CNS DNLP RMINLP QCP RMIQCP\ngmsgenus.run\ngmsgenux.out\nlibsnlcclib64.so snl 1 1'
```

## gamspy_snopt/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.3.1'
+__version__ = '46.4.0'
```

## Comparing `gamspy_snopt-46.3.1.dist-info/RECORD` & `gamspy_snopt-46.4.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-gamspy_snopt/__init__.py,sha256=ItjWqT-JyWUaYQhmDeEzNr26ixSYQxvuqYX9CbELSM4,357
+gamspy_snopt/__init__.py,sha256=eaHzwnYnGJUHsEMMjQ3UsitlAQbri1_L-ZENpTffljQ,350
+gamspy_snopt/libsnlcclib64.so,sha256=_C01ceOwqHc6EFDbvYbxq8AgwKaVccY-XDGppEofBg4,1005064
 gamspy_snopt/optsnopt.def,sha256=AyUyL0CwqFnJdUsE5vDxxiIDeJO5nF66jv4rcjktg1c,6967
-gamspy_snopt/snlcclib64.dll,sha256=THOCntkEuXzFl6AMgOuXRtiy4NV8Ynegq0_frqkjqjs,1416704
-gamspy_snopt/version.py,sha256=pI_HpTMcRcJbI4ztOwjiZW7rJxUGHQgZBbviFRoHXy4,22
-gamspy_snopt-46.3.1.dist-info/METADATA,sha256=smPuXKsh4wS0KDhRe5mwD1Fk3PtAp0TlSic3tgc9GRE,62
-gamspy_snopt-46.3.1.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
-gamspy_snopt-46.3.1.dist-info/top_level.txt,sha256=nZnA0uoys7BMIVU95a2187m-Cc0GjkYGFp1E1cEKujM,13
-gamspy_snopt-46.3.1.dist-info/RECORD,,
+gamspy_snopt/version.py,sha256=aPpKdDaOIvtNrT9mpHftLgRfZ1X1uLWURDzyhZyW1zI,22
+gamspy_snopt-46.4.0.dist-info/METADATA,sha256=FFUhzz1jqZpJi9POPrgR4qxueFWS1WkWyQ0ZcdXrHXQ,58
+gamspy_snopt-46.4.0.dist-info/WHEEL,sha256=EyChNuwWclgJLf8btn5REviYd5IxRGn2tIXp4VelYwc,116
+gamspy_snopt-46.4.0.dist-info/top_level.txt,sha256=nZnA0uoys7BMIVU95a2187m-Cc0GjkYGFp1E1cEKujM,13
+gamspy_snopt-46.4.0.dist-info/RECORD,,
```

