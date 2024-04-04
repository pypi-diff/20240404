# Comparing `tmp/gamspy_copt-46.3.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_copt-46.4.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8337103 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      383 b- defN 24-Mar-28 19:09 gamspy_copt/__init__.py
--rw-rw-rw-  2.0 fat 19559424 b- defN 24-Mar-28 19:09 gamspy_copt/copt.dll
--rw-rw-rw-  2.0 fat   459776 b- defN 24-Mar-28 19:09 gamspy_copt/cptcclib64.dll
--rw-rw-rw-  2.0 fat  5458432 b- defN 24-Mar-28 19:09 gamspy_copt/libcrypto-3-x64.dll
--rw-rw-rw-  2.0 fat     8873 b- defN 24-Mar-28 19:09 gamspy_copt/optcopt.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-28 19:09 gamspy_copt/version.py
--rw-rw-rw-  2.0 fat       61 b- defN 24-Mar-28 19:09 gamspy_copt-46.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-28 19:09 gamspy_copt-46.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Mar-28 19:09 gamspy_copt-46.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      810 b- defN 24-Mar-28 19:09 gamspy_copt-46.3.1.dist-info/RECORD
-10 files, 25487897 bytes uncompressed, 8335735 bytes compressed:  67.3%
+Zip file size: 8337109 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      383 b- defN 24-Apr-04 14:13 gamspy_copt/__init__.py
+-rw-rw-rw-  2.0 fat 19559424 b- defN 24-Apr-04 14:13 gamspy_copt/copt.dll
+-rw-rw-rw-  2.0 fat   459776 b- defN 24-Apr-04 14:13 gamspy_copt/cptcclib64.dll
+-rw-rw-rw-  2.0 fat  5458432 b- defN 24-Apr-04 14:13 gamspy_copt/libcrypto-3-x64.dll
+-rw-rw-rw-  2.0 fat     8873 b- defN 24-Apr-04 14:13 gamspy_copt/optcopt.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-04 14:13 gamspy_copt/version.py
+-rw-rw-rw-  2.0 fat       61 b- defN 24-Apr-04 14:13 gamspy_copt-46.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-04 14:13 gamspy_copt-46.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-04 14:13 gamspy_copt-46.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      810 b- defN 24-Apr-04 14:13 gamspy_copt-46.4.0.dist-info/RECORD
+10 files, 25487897 bytes uncompressed, 8335741 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: gamspy_copt/optcopt.def
 Comment: 
 
 Filename: gamspy_copt/version.py
 Comment: 
 
-Filename: gamspy_copt-46.3.1.dist-info/METADATA
+Filename: gamspy_copt-46.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_copt-46.3.1.dist-info/WHEEL
+Filename: gamspy_copt-46.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_copt-46.3.1.dist-info/top_level.txt
+Filename: gamspy_copt-46.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_copt-46.3.1.dist-info/RECORD
+Filename: gamspy_copt-46.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_copt/cptcclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005f6e0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 10:11:00 2024
+Time/Date		Tue Apr  2 08:19:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000060400
 SizeOfInitializedData	0000000000012a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005f6e0
@@ -99408,17 +99408,17 @@
    18006bc67:	add    %ch,0x72(%rcx)
    18006bc6a:	movsxd 0x6d(%rdi),%ebx
    18006bc6d:	jae    0x18006bcd6
    18006bc6f:	cs fs insb (%dx),%es:(%rdi)
    18006bc72:	insb   (%dx),%es:(%rdi)
    18006bc73:	add    %al,(%rax)
    18006bc75:	add    %al,(%rax)
-   18006bc77:	add    %dh,0x65f9(%rsp,%riz,2)
-   18006bc7e:	add    %al,(%rax)
-   18006bc80:	or     $0x64000000,%eax
+   18006bc77:	add    %dl,0x660bbf(%rbx)
+   18006bc7d:	add    %al,(%rax)
+   18006bc7f:	add    %cl,0x64000000(%rip)        # 0x1e406bc85
    18006bc85:	add    (%rax),%al
    18006bc87:	add    %bl,(%rax)
    18006bc89:	mov    $0xa6180006,%esi
    18006bc8e:	(bad)
    18006bc8f:	add    %bh,(%rax)
    18006bc91:	add    %eax,(%rax)
 	...
```

## gamspy_copt/libcrypto-3-x64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001253
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 10:04:46 2024
+Time/Date		Tue Apr  2 08:13:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000003df000
 SizeOfInitializedData	0000000000158a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001253
@@ -96088,15 +96088,15 @@
 	reloc    4 offset   40 [52d040] DIR64
 	reloc    5 offset    0 [52d000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1804b45d4
 
 Type                Size     Rva      Offset
   2        CodeView 0000005c 004b729c 004b669c
-(format RSDS signature d4546d2e91a340f6883a81f170f8e1de age 1 pdb C:\home\distrib\porting\btree\openssl\wei\build\libcrypto-3-x64.pdb)
+(format RSDS signature 1ea762db59a04c4187135e4ce9ca9e53 age 1 pdb C:\home\distrib\porting\btree\openssl\wei\build\libcrypto-3-x64.pdb)
  12         Feature 00000014 004b72f8 004b66f8
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000010, Value: 0x80000018
 018    Name Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 028     Entry: ID: 0x000001, Value: 0x80000030
@@ -1868369,24 +1868369,24 @@
    180441db4:	xor    %esi,(%rdx)
    180441db6:	add    %al,(%rax)
    180441db8:	(bad)
    180441dbd:	and    %ch,0x6e(%rdi)
    180441dc0:	cmp    (%rax),%ah
    180441dc2:	push   %rsp
    180441dc3:	jne    0x180441e2a
-   180441dc5:	and    %cl,0x61(%rbp)
+   180441dc5:	and    %al,0x70(%rcx)
    180441dc8:	jb     0x180441dea
-   180441dca:	xor    %edi,(%rcx)
-   180441dcc:	and    %dh,(%rcx)
-   180441dce:	xor    %bh,(%rdx)
-   180441dd0:	xor    %dh,(%rbx)
-   180441dd2:	cmp    (%rbx,%rsi,1),%dh
-   180441dd5:	and    %dh,(%rdx)
-   180441dd7:	xor    %dh,(%rdx)
-   180441dd9:	xor    $0x20,%al
+   180441dca:	and    %dh,(%rdx)
+   180441dcc:	and    %dh,(%rax)
+   180441dce:	cmp    %bh,(%rdx)
+   180441dd0:	xor    %esi,(%rdx)
+   180441dd2:	cmp    (%rbx),%dh
+   180441dd4:	cmp    %ah,(%rax)
+   180441dd6:	xor    (%rax),%dh
+   180441dd8:	xor    (%rax,%riz,1),%dh
    180441ddb:	push   %rbp
    180441ddc:	push   %rsp
    180441ddd:	rex.XB add %al,(%r8)
 	...
    180441de8:	jo     0x180441e56
    180441dea:	(bad)
    180441deb:	je     0x180441e53
@@ -2015464,28 +2015464,26 @@
    1804b45bb:	(bad)
    1804b45bc:	(bad)
    1804b45bd:	(bad)
    1804b45be:	(bad)
    1804b45bf:	incl   (%rax)
 	...
    1804b45d5:	add    %al,(%rax)
-   1804b45d7:	add    %bh,(%rsi)
-   1804b45d9:	movsxd %ecx,%edi
-   1804b45db:	add    %al,%gs:(%rax)
+   1804b45d7:	add    %dh,(%rcx)
+   1804b45d9:	mov    $0x660b,%esi
    1804b45de:	add    %al,(%rax)
    1804b45e0:	add    (%rax),%al
    1804b45e2:	add    %al,(%rax)
    1804b45e4:	pop    %rsp
    1804b45e5:	add    %al,(%rax)
    1804b45e7:	add    %bl,0x669c004b(%rdx,%rsi,2)
    1804b45ee:	rex.WXB add %al,(%r8)
    1804b45f1:	add    %al,(%rax)
-   1804b45f3:	add    %bh,(%rsi)
-   1804b45f5:	movsxd %ecx,%edi
-   1804b45f7:	add    %al,%gs:(%rax)
+   1804b45f3:	add    %dh,(%rcx)
+   1804b45f5:	mov    $0x660b,%esi
    1804b45fa:	add    %al,(%rax)
    1804b45fc:	or     $0x0,%al
    1804b45fe:	add    %al,(%rax)
    1804b4600:	adc    $0x0,%al
    1804b4602:	add    %al,(%rax)
    1804b4604:	clc
    1804b4605:	jb     0x1804b4652
@@ -2015527,20 +2015525,18 @@
    1804b4742:	push   %rax
    1804b4743:	addb   $0x0,(%rcx)
 	...
    1804b729a:	add    %al,(%rax)
    1804b729c:	push   %rdx
    1804b729d:	push   %rbx
    1804b729e:	rex.R push %rbx
-   1804b72a0:	cs insl (%dx),%es:(%rdi)
-   1804b72a2:	push   %rsp
+   1804b72a0:	(bad)  -0x59(%rdx)
    1804b72a3:	(bad)
-   1804b72a4:	movabs %eax,0x70f1813a8840f691
-   1804b72ad:	clc
-   1804b72ae:	loope  0x1804b728e
+   1804b72a4:	movabs 0xe94c5e13874c4159,%al
+   1804b72ad:	lret   $0x539e
    1804b72b0:	add    %eax,(%rax)
    1804b72b2:	add    %al,(%rax)
    1804b72b4:	cmp    0x6f(%r8,%r13,2),%bl
    1804b72b9:	insl   (%dx),%es:(%rdi)
    1804b72ba:	gs pop %rsp
    1804b72bc:	imul   $0x5c626972,%fs:0x74(%rbx),%esi
    1804b72c4:	jo     0x1804b7335
```

## gamspy_copt/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.3.1'
+__version__ = '46.4.0'
```

