# Comparing `tmp/gamspy_conopt3-46.3.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_conopt3-46.4.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 918791 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      376 b- defN 24-Mar-28 19:09 gamspy_conopt3/__init__.py
--rw-rw-rw-  2.0 fat   389632 b- defN 24-Mar-28 19:09 gamspy_conopt3/concclib64.dll
--rw-rw-rw-  2.0 fat  1851904 b- defN 24-Mar-28 19:09 gamspy_conopt3/conopt3.dll
--rw-rw-rw-  2.0 fat    12089 b- defN 24-Mar-28 19:09 gamspy_conopt3/optconopt3.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-28 19:09 gamspy_conopt3/version.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-Mar-28 19:09 gamspy_conopt3-46.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-28 19:09 gamspy_conopt3-46.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Mar-28 19:09 gamspy_conopt3-46.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      752 b- defN 24-Mar-28 19:09 gamspy_conopt3-46.3.1.dist-info/RECORD
-9 files, 2254958 bytes uncompressed, 917495 bytes compressed:  59.3%
+Zip file size: 918796 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      376 b- defN 24-Apr-04 14:13 gamspy_conopt3/__init__.py
+-rw-rw-rw-  2.0 fat   389632 b- defN 24-Apr-04 14:13 gamspy_conopt3/concclib64.dll
+-rw-rw-rw-  2.0 fat  1851904 b- defN 24-Apr-04 14:13 gamspy_conopt3/conopt3.dll
+-rw-rw-rw-  2.0 fat    12089 b- defN 24-Apr-04 14:13 gamspy_conopt3/optconopt3.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-04 14:13 gamspy_conopt3/version.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-Apr-04 14:13 gamspy_conopt3-46.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-04 14:13 gamspy_conopt3-46.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-04 14:13 gamspy_conopt3-46.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      752 b- defN 24-Apr-04 14:13 gamspy_conopt3-46.4.0.dist-info/RECORD
+9 files, 2254958 bytes uncompressed, 917500 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: gamspy_conopt3/optconopt3.def
 Comment: 
 
 Filename: gamspy_conopt3/version.py
 Comment: 
 
-Filename: gamspy_conopt3-46.3.1.dist-info/METADATA
+Filename: gamspy_conopt3-46.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_conopt3-46.3.1.dist-info/WHEEL
+Filename: gamspy_conopt3-46.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_conopt3-46.3.1.dist-info/top_level.txt
+Filename: gamspy_conopt3-46.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_conopt3-46.3.1.dist-info/RECORD
+Filename: gamspy_conopt3-46.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_conopt3/concclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004fed0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 09:43:35 2024
+Time/Date		Tue Apr  2 07:53:41 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000051600
 SizeOfInitializedData	0000000000010200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004fed0
@@ -85469,19 +85469,17 @@
    18005a617:	add    %al,%al
    18005a619:	in     (%dx),%eax
    18005a61a:	add    $0x180,%eax
    18005a61f:	add    %ah,-0x12(%rax)
    18005a622:	add    $0x180,%eax
    18005a627:	add    %al,(%rax)
    18005a629:	add    %al,(%rax)
-   18005a62b:	add    %al,0x5e(%rdi)
-   18005a62e:	stc
-   18005a62f:	add    %al,%gs:(%rax)
-   18005a632:	add    %al,(%rax)
-   18005a634:	or     $0x64000000,%eax
+   18005a62b:	add    %al,0x660bb9(%rbp)
+   18005a631:	add    %al,(%rax)
+   18005a633:	add    %cl,0x64000000(%rip)        # 0x1e405a639
    18005a639:	add    (%rax),%al
    18005a63b:	add    %bl,(%rax)
    18005a63d:	test   $0x5,%al
    18005a63f:	add    %bl,(%rax)
    18005a641:	xchg   %eax,%edx
    18005a642:	add    $0x0,%eax
 	...
```

## gamspy_conopt3/conopt3.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180177ee0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 09:42:52 2024
+Time/Date		Tue Apr  2 07:52:59 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000179600
 SizeOfInitializedData	000000000004bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000177ee0
@@ -374612,17 +374612,16 @@
    1801a56fc:	add    %eax,(%rax)
    1801a56fe:	add    %al,(%rax)
    1801a5700:	orb    $0x1c,(%rbx)
    1801a5703:	addb   $0x0,(%rcx)
    1801a5706:	add    %al,(%rax)
    1801a5708:	add    %al,(%rax)
    1801a570a:	add    %al,(%rax)
-   1801a570c:	sbb    $0x5e,%al
-   1801a570e:	stc
-   1801a570f:	add    %al,%gs:(%rax)
+   1801a570c:	pop    %rbx
+   1801a570d:	mov    $0x660b,%ecx
    1801a5712:	add    %al,(%rax)
    1801a5714:	or     $0x64000000,%eax
    1801a5719:	add    (%rax),%al
    1801a571b:	add    %bl,-0x67ffe5a8(%rax)
    1801a5721:	rex.X sbb (%rax),%al
 	...
    1801a5730:	cmp    %al,(%rcx)
```

## gamspy_conopt3/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.3.1'
+__version__ = '46.4.0'
```

