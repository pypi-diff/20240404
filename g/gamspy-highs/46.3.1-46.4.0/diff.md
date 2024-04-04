# Comparing `tmp/gamspy_highs-46.3.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_highs-46.4.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2500392 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      331 b- defN 24-Mar-28 19:09 gamspy_highs/__init__.py
--rw-rw-rw-  2.0 fat  5996544 b- defN 24-Mar-28 19:09 gamspy_highs/hiscclib64.dll
--rw-rw-rw-  2.0 fat    10138 b- defN 24-Mar-28 19:09 gamspy_highs/opthighs.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-28 19:09 gamspy_highs/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Mar-28 19:09 gamspy_highs-46.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-28 19:09 gamspy_highs-46.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Mar-28 19:09 gamspy_highs-46.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      649 b- defN 24-Mar-28 19:09 gamspy_highs-46.3.1.dist-info/RECORD
-8 files, 6007863 bytes uncompressed, 2499260 bytes compressed:  58.4%
+Zip file size: 2500397 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      331 b- defN 24-Apr-04 14:13 gamspy_highs/__init__.py
+-rw-rw-rw-  2.0 fat  5996544 b- defN 24-Apr-04 14:13 gamspy_highs/hiscclib64.dll
+-rw-rw-rw-  2.0 fat    10138 b- defN 24-Apr-04 14:13 gamspy_highs/opthighs.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-04 14:13 gamspy_highs/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-04 14:13 gamspy_highs-46.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-04 14:13 gamspy_highs-46.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-04 14:13 gamspy_highs-46.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      649 b- defN 24-Apr-04 14:13 gamspy_highs-46.4.0.dist-info/RECORD
+8 files, 6007863 bytes uncompressed, 2499265 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gamspy_highs/opthighs.def
 Comment: 
 
 Filename: gamspy_highs/version.py
 Comment: 
 
-Filename: gamspy_highs-46.3.1.dist-info/METADATA
+Filename: gamspy_highs-46.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_highs-46.3.1.dist-info/WHEEL
+Filename: gamspy_highs-46.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_highs-46.3.1.dist-info/top_level.txt
+Filename: gamspy_highs-46.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_highs-46.3.1.dist-info/RECORD
+Filename: gamspy_highs-46.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_highs/hiscclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001804d5da4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 09:59:33 2024
+Time/Date		Tue Apr  2 08:09:01 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000004d7c00
 SizeOfInitializedData	00000000000f2000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000004d5da4
@@ -1334603,15 +1334603,15 @@
    18050085d:	add    %al,(%rax)
    18050085f:	add    %dh,(%rax)
    180500861:	call   *-0x80(%rsi)
    180500864:	add    %eax,(%rax)
    180500866:	add    %al,(%rax)
    180500868:	add    %al,(%rax)
    18050086a:	add    %al,(%rax)
-   18050086c:	add    $0x65f962,%eax
+   18050086c:	sbb    $0x660bbd,%eax
    180500871:	add    %al,(%rax)
    180500873:	add    %cl,-0x2c000000(%rip)        # 0x154500879
    180500879:	add    (%rax),%eax
    18050087b:	add    %dh,-0x54bffb0(%rdx,%rcx,1)
    180500882:	rex.WRXB add %r8b,(%r8)
 	...
    18050088d:	add    %al,(%rax)
```

## gamspy_highs/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.3.1'
+__version__ = '46.4.0'
```

