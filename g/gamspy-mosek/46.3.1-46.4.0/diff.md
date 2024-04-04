# Comparing `tmp/gamspy_mosek-46.3.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_mosek-46.4.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8688763 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      423 b- defN 24-Mar-28 19:10 gamspy_mosek/__init__.py
--rw-rw-rw-  2.0 fat 24969728 b- defN 24-Mar-28 19:10 gamspy_mosek/mosek64_10_1.dll
--rw-rw-rw-  2.0 fat   568832 b- defN 24-Mar-28 19:10 gamspy_mosek/mskcclib64.dll
--rw-rw-rw-  2.0 fat   567328 b- defN 24-Mar-28 19:10 gamspy_mosek/msvcp140.dll
--rw-rw-rw-  2.0 fat    47074 b- defN 24-Mar-28 19:10 gamspy_mosek/optmosek.def
--rw-rw-rw-  2.0 fat   287880 b- defN 24-Mar-28 19:10 gamspy_mosek/tbb12.dll
--rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-28 19:10 gamspy_mosek/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Mar-28 19:10 gamspy_mosek-46.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Mar-28 19:10 gamspy_mosek-46.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Mar-28 19:10 gamspy_mosek-46.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      903 b- defN 24-Mar-28 19:10 gamspy_mosek-46.3.1.dist-info/RECORD
+-rw-rw-rw-  2.0 fat      423 b- defN 24-Apr-04 14:14 gamspy_mosek/__init__.py
+-rw-rw-rw-  2.0 fat 24969728 b- defN 24-Apr-04 14:14 gamspy_mosek/mosek64_10_1.dll
+-rw-rw-rw-  2.0 fat   568832 b- defN 24-Apr-04 14:14 gamspy_mosek/mskcclib64.dll
+-rw-rw-rw-  2.0 fat   567328 b- defN 24-Apr-04 14:14 gamspy_mosek/msvcp140.dll
+-rw-rw-rw-  2.0 fat    47074 b- defN 24-Apr-04 14:14 gamspy_mosek/optmosek.def
+-rw-rw-rw-  2.0 fat   287880 b- defN 24-Apr-04 14:14 gamspy_mosek/tbb12.dll
+-rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-04 14:14 gamspy_mosek/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-04 14:14 gamspy_mosek-46.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-04 14:14 gamspy_mosek-46.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-04 14:14 gamspy_mosek-46.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      903 b- defN 24-Apr-04 14:14 gamspy_mosek-46.4.0.dist-info/RECORD
 11 files, 26442369 bytes uncompressed, 8687251 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: gamspy_mosek/tbb12.dll
 Comment: 
 
 Filename: gamspy_mosek/version.py
 Comment: 
 
-Filename: gamspy_mosek-46.3.1.dist-info/METADATA
+Filename: gamspy_mosek-46.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_mosek-46.3.1.dist-info/WHEEL
+Filename: gamspy_mosek-46.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_mosek-46.3.1.dist-info/top_level.txt
+Filename: gamspy_mosek-46.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_mosek-46.3.1.dist-info/RECORD
+Filename: gamspy_mosek-46.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_mosek/mskcclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180076380
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Mar 19 10:13:22 2024
+Time/Date		Tue Apr  2 08:21:51 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000077800
 SizeOfInitializedData	0000000000016200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000076380
@@ -127100,17 +127100,17 @@
    180083833:	add    %al,(%rax)
    180083835:	add    %al,(%rax)
    180083837:	add    %al,(%rax)
    180083839:	test   $0x18008,%eax
    18008383e:	add    %al,(%rax)
    180083840:	movabs 0x18008a9,%al
    180083849:	add    %al,(%rax)
-   18008384b:	add    %al,0x65(%rdx)
-   18008384e:	stc
-   18008384f:	add    %al,%gs:(%rax)
+   18008384b:	add    %bl,(%rdi)
+   18008384d:	rorb   $0x66,(%rbx)
+   180083850:	add    %al,(%rax)
    180083852:	add    %al,(%rax)
    180083854:	or     $0x74000000,%eax
    180083859:	add    (%rax),%al
    18008385b:	add    %bl,(%rax)
    18008385d:	cmp    (%rax),%cl
    18008385f:	add    %bl,(%rax)
    180083861:	es or  %al,(%rax)
```

## gamspy_mosek/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.3.1'
+__version__ = '46.4.0'
```

