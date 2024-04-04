# Comparing `tmp/gamspy_minos-46.3.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_minos-46.4.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 405787 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      357 b- defN 24-Mar-28 19:10 gamspy_minos/__init__.py
--rw-rw-rw-  2.0 fat   973312 b- defN 24-Mar-28 19:10 gamspy_minos/milcclib64.dll
--rw-rw-rw-  2.0 fat     5745 b- defN 24-Mar-28 19:10 gamspy_minos/optminos.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-28 19:10 gamspy_minos/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Mar-28 19:10 gamspy_minos-46.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-28 19:10 gamspy_minos-46.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Mar-28 19:10 gamspy_minos-46.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      647 b- defN 24-Mar-28 19:10 gamspy_minos-46.3.1.dist-info/RECORD
-8 files, 980262 bytes uncompressed, 404655 bytes compressed:  58.7%
+Zip file size: 405792 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      357 b- defN 24-Apr-04 14:14 gamspy_minos/__init__.py
+-rw-rw-rw-  2.0 fat   973312 b- defN 24-Apr-04 14:14 gamspy_minos/milcclib64.dll
+-rw-rw-rw-  2.0 fat     5745 b- defN 24-Apr-04 14:14 gamspy_minos/optminos.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-04 14:14 gamspy_minos/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-04 14:14 gamspy_minos-46.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-04 14:14 gamspy_minos-46.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-04 14:14 gamspy_minos-46.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      647 b- defN 24-Apr-04 14:14 gamspy_minos-46.4.0.dist-info/RECORD
+8 files, 980262 bytes uncompressed, 404660 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gamspy_minos/optminos.def
 Comment: 
 
 Filename: gamspy_minos/version.py
 Comment: 
 
-Filename: gamspy_minos-46.3.1.dist-info/METADATA
+Filename: gamspy_minos-46.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_minos-46.3.1.dist-info/WHEEL
+Filename: gamspy_minos-46.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_minos-46.3.1.dist-info/top_level.txt
+Filename: gamspy_minos-46.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_minos-46.3.1.dist-info/RECORD
+Filename: gamspy_minos-46.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_minos/milcclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800cb0e4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 09:59:46 2024
+Time/Date		Tue Apr  2 08:09:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000000cc800
 SizeOfInitializedData	0000000000024e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000cb0e4
@@ -202410,16 +202410,15 @@
    1800d9d46:	add    %al,(%rax)
    1800d9d48:	rol    $1,%al
    1800d9d4a:	(bad)
    1800d9d4b:	addb   $0x0,(%rcx)
    1800d9d4e:	add    %al,(%rax)
    1800d9d50:	add    %al,(%rax)
    1800d9d52:	add    %al,(%rax)
-   1800d9d54:	adc    -0x7(%rdx),%ah
-   1800d9d57:	add    %al,%gs:(%rax)
+   1800d9d54:	sub    %edi,0x660b(%rbp)
    1800d9d5a:	add    %al,(%rax)
    1800d9d5c:	or     $0x64000000,%eax
    1800d9d61:	add    (%rax),%al
    1800d9d63:	add    %bl,(%rax)
    1800d9d65:	lahf
    1800d9d66:	or     $0xd8b1800,%eax
    1800d9d6b:	add    %al,(%rax)
```

## gamspy_minos/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.3.1'
+__version__ = '46.4.0'
```

## Comparing `gamspy_minos-46.3.1.dist-info/RECORD` & `gamspy_minos-46.4.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gamspy_minos/__init__.py,sha256=KsFJW__AbhZgFlA3BVJpLRnQPE5X5DoIt8TF_qTo7H0,357
-gamspy_minos/milcclib64.dll,sha256=x8YmiukHRonp4Kib2mU7KYrC5prkO6z8id42AG-ByII,973312
+gamspy_minos/milcclib64.dll,sha256=lemFtvGotSbqmcR6KAqfmYPvWH9PQpqe3ozALGlpw7o,973312
 gamspy_minos/optminos.def,sha256=zKjp1whuFPe4wPwBIhe4eV_TdUeONZW4ASUOXVsJJWs,5745
-gamspy_minos/version.py,sha256=pI_HpTMcRcJbI4ztOwjiZW7rJxUGHQgZBbviFRoHXy4,22
-gamspy_minos-46.3.1.dist-info/METADATA,sha256=H5AzTgrn6sycKxWBkT2DEk3Ke6zclblCPWQGbuA6B5U,62
-gamspy_minos-46.3.1.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
-gamspy_minos-46.3.1.dist-info/top_level.txt,sha256=lmNjYS_YUYyttCdbZ_KGkM9XB-f-a92G0QB-N2J_Hw8,13
-gamspy_minos-46.3.1.dist-info/RECORD,,
+gamspy_minos/version.py,sha256=aPpKdDaOIvtNrT9mpHftLgRfZ1X1uLWURDzyhZyW1zI,22
+gamspy_minos-46.4.0.dist-info/METADATA,sha256=9pBeejN_w3hHPhrYkjpmHzBEKOmkf72KUMlkGB9XQ2I,62
+gamspy_minos-46.4.0.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
+gamspy_minos-46.4.0.dist-info/top_level.txt,sha256=lmNjYS_YUYyttCdbZ_KGkM9XB-f-a92G0QB-N2J_Hw8,13
+gamspy_minos-46.4.0.dist-info/RECORD,,
```

