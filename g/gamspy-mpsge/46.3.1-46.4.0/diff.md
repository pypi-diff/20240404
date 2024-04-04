# Comparing `tmp/gamspy_mpsge-46.3.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_mpsge-46.4.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 500400 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      357 b- defN 24-Mar-28 19:10 gamspy_mpsge/__init__.py
--rw-rw-rw-  2.0 fat      378 b- defN 24-Mar-28 19:10 gamspy_mpsge/gmsge_nt.cmd
--rw-rw-rw-  2.0 fat   240640 b- defN 24-Mar-28 19:10 gamspy_mpsge/gmsge_nx.exe
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-28 19:10 gamspy_mpsge/gmsgewnt.cmd
--rw-rw-rw-  2.0 fat   697344 b- defN 24-Mar-28 19:10 gamspy_mpsge/gmsgewnx.exe
--rw-rw-rw-  2.0 fat     1796 b- defN 24-Mar-28 19:10 gamspy_mpsge/mpsgeset
--rw-rw-rw-  2.0 fat   332800 b- defN 24-Mar-28 19:10 gamspy_mpsge/mpsgeval.dll
--rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-28 19:10 gamspy_mpsge/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Mar-28 19:10 gamspy_mpsge-46.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-28 19:10 gamspy_mpsge-46.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Mar-28 19:10 gamspy_mpsge-46.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      970 b- defN 24-Mar-28 19:10 gamspy_mpsge-46.3.1.dist-info/RECORD
-12 files, 1274578 bytes uncompressed, 498776 bytes compressed:  60.9%
+Zip file size: 500402 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      357 b- defN 24-Apr-04 14:14 gamspy_mpsge/__init__.py
+-rw-rw-rw-  2.0 fat      378 b- defN 24-Apr-04 14:14 gamspy_mpsge/gmsge_nt.cmd
+-rw-rw-rw-  2.0 fat   240640 b- defN 24-Apr-04 14:14 gamspy_mpsge/gmsge_nx.exe
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-04 14:14 gamspy_mpsge/gmsgewnt.cmd
+-rw-rw-rw-  2.0 fat   697344 b- defN 24-Apr-04 14:14 gamspy_mpsge/gmsgewnx.exe
+-rw-rw-rw-  2.0 fat     1796 b- defN 24-Apr-04 14:14 gamspy_mpsge/mpsgeset
+-rw-rw-rw-  2.0 fat   332800 b- defN 24-Apr-04 14:14 gamspy_mpsge/mpsgeval.dll
+-rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-04 14:14 gamspy_mpsge/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-04 14:14 gamspy_mpsge-46.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-04 14:14 gamspy_mpsge-46.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-04 14:14 gamspy_mpsge-46.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      970 b- defN 24-Apr-04 14:14 gamspy_mpsge-46.4.0.dist-info/RECORD
+12 files, 1274578 bytes uncompressed, 498778 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: gamspy_mpsge/mpsgeval.dll
 Comment: 
 
 Filename: gamspy_mpsge/version.py
 Comment: 
 
-Filename: gamspy_mpsge-46.3.1.dist-info/METADATA
+Filename: gamspy_mpsge-46.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_mpsge-46.3.1.dist-info/WHEEL
+Filename: gamspy_mpsge-46.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_mpsge-46.3.1.dist-info/top_level.txt
+Filename: gamspy_mpsge-46.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_mpsge-46.3.1.dist-info/RECORD
+Filename: gamspy_mpsge-46.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_mpsge/gmsge_nx.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014002e150
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Mar 19 10:00:02 2024
+Time/Date		Tue Apr  2 08:09:24 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000002f800
 SizeOfInitializedData	0000000000042600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000002e150
@@ -57160,18 +57160,18 @@
    140035976:	add    %al,(%rax)
    140035978:	adc    %dh,%dl
    14003597a:	add    $0x40,%al
    14003597c:	add    %eax,(%rax)
    14003597e:	add    %al,(%rax)
    140035980:	add    %al,(%rax)
    140035982:	add    %al,(%rax)
-   140035984:	and    -0x7(%rdx),%ah
-   140035987:	add    %al,%gs:(%rax)
-   14003598a:	add    %al,(%rax)
-   14003598c:	or     $0x90000000,%eax
+   140035984:	xor    $0xbd,%al
+   140035986:	or     0x0(%rsi),%esp
+   140035989:	add    %al,(%rax)
+   14003598b:	add    %cl,-0x70000000(%rip)        # 0xd0035991
    140035991:	add    (%rax),%al
    140035993:	add    %bl,(%rax)
    140035995:	pop    %rbx
    140035996:	add    (%rax),%eax
    140035998:	sbb    %al,0x3(%rdi)
    14003599b:	add    %al,(%rax)
    14003599d:	add    %al,(%rax)
```

## gamspy_mpsge/gmsgewnx.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014008c800
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Mar 19 10:00:03 2024
+Time/Date		Tue Apr  2 08:09:25 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000008de00
 SizeOfInitializedData	0000000000579a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000008c800
@@ -162842,18 +162842,17 @@
    14009ee55:	add    %al,(%rax)
    14009ee57:	add    %dl,(%rax)
    14009ee59:	(bad)
    14009ee5c:	add    %eax,(%rax)
    14009ee5e:	add    %al,(%rax)
    14009ee60:	add    %al,(%rax)
    14009ee62:	add    %al,(%rax)
-   14009ee64:	and    -0x7(%rdx),%esp
-   14009ee67:	add    %al,%gs:(%rax)
-   14009ee6a:	add    %al,(%rax)
-   14009ee6c:	or     $0x90000000,%eax
+   14009ee64:	xor    $0x660bbd,%eax
+   14009ee69:	add    %al,(%rax)
+   14009ee6b:	add    %cl,-0x70000000(%rip)        # 0xd009ee71
    14009ee71:	add    (%rax),%al
    14009ee73:	add    %bl,(%rax)
    14009ee75:	lock or %eax,(%rax)
    14009ee78:	sbb    %ah,%dl
    14009ee7a:	or     %eax,(%rax)
    14009ee7c:	add    %al,(%rax)
    14009ee7e:	add    %al,(%rax)
```

## gamspy_mpsge/mpsgeval.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180043970
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 10:00:00 2024
+Time/Date		Tue Apr  2 08:09:23 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000045000
 SizeOfInitializedData	0000000000567c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000043970
@@ -73827,16 +73827,15 @@
    18004a075:	add    %al,(%rax)
    18004a077:	add    %al,0x40(%rax)
    18004a07a:	or     0x1(%rax),%eax
    18004a080:	loopne 0x18004a0c2
    18004a082:	or     0x1(%rax),%eax
    18004a088:	add    %al,(%rax)
    18004a08a:	add    %al,(%rax)
-   18004a08c:	and    %ah,-0x7(%rdx)
-   18004a08f:	add    %al,%gs:(%rax)
+   18004a08c:	xor    0x660b(%rbp),%edi
    18004a092:	add    %al,(%rax)
    18004a094:	or     $0x64000000,%eax
    18004a099:	add    (%rax),%al
    18004a09b:	add    %bl,(%rax)
    18004a09d:	movabs %al,0x496180004
 	...
    18004a0ae:	add    %al,(%rax)
```

## gamspy_mpsge/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.3.1'
+__version__ = '46.4.0'
```

