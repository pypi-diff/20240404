# Comparing `tmp/locidex-0.1.1.tar.gz` & `tmp/locidex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/locidex-0.1.1.tar", last modified: Mon Mar 18 19:08:17 2024, max compression
+gzip compressed data, was "dist/locidex-0.1.2.tar", last modified: Thu Apr  4 17:36:16 2024, max compression
```

## Comparing `locidex-0.1.1.tar` & `locidex-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 19:08:17.000000 locidex-0.1.1/
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 18:56:29.000000 locidex-0.1.1/MANIFEST.in
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)     1009 2024-03-18 19:08:17.000000 locidex-0.1.1/PKG-INFO
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    26860 2024-03-18 18:56:29.000000 locidex-0.1.1/README.md
-drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex/
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/__init__.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     7795 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/build.py
-drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 19:08:17.000000 locidex-0.1.1/locidex/classes/
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)      561 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/__init__.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     6560 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/aligner.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)      348 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/assignment.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     5141 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/blast.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     3349 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/db.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    15660 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/extractor.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1716 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/fasta.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     5083 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/gbk.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/gff.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1355 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/mafft.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1048 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/metadata.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1005 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/prodigal.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    12726 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/seq_intake.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        3 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/classes/seq_writers.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     2243 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/constants.py
-drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 19:08:17.000000 locidex-0.1.1/locidex/example/
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 18:56:29.000000 locidex-0.1.1/locidex/example/__init__.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    11523 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/extract.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/fetch.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    10378 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/format.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1760 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/main.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     2952 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/merge.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    13449 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/report.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    10913 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/search.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     3022 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/utils.py
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)       21 2024-03-18 18:56:30.000000 locidex-0.1.1/locidex/version.py
-drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex.egg-info/
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)     1009 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex.egg-info/PKG-INFO
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)      837 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex.egg-info/SOURCES.txt
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)        1 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex.egg-info/dependency_links.txt
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)       47 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex.egg-info/entry_points.txt
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)       94 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex.egg-info/requires.txt
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)        8 2024-03-18 19:08:16.000000 locidex-0.1.1/locidex.egg-info/top_level.txt
--rwxr-x---   0 jarobert (101035) grp_jarobert (101035)       38 2024-03-18 19:08:17.000000 locidex-0.1.1/setup.cfg
--rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1882 2024-03-18 18:56:30.000000 locidex-0.1.1/setup.py
+drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:36:16.000000 locidex-0.1.2/
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:29:39.000000 locidex-0.1.2/MANIFEST.in
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)     1009 2024-04-04 17:36:16.000000 locidex-0.1.2/PKG-INFO
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    27385 2024-04-04 17:29:39.000000 locidex-0.1.2/README.md
+drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:36:16.000000 locidex-0.1.2/locidex/
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/__init__.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     7795 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/build.py
+drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:36:16.000000 locidex-0.1.2/locidex/classes/
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)      561 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/__init__.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     6560 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/aligner.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)      348 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/assignment.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     5141 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/blast.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     3349 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/db.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    18776 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/extractor.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1716 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/fasta.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     5083 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/gbk.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/gff.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1355 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/mafft.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1048 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/metadata.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1005 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/prodigal.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    12726 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/seq_intake.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        3 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/classes/seq_writers.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     2243 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/constants.py
+drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:36:16.000000 locidex-0.1.2/locidex/example/
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/example/__init__.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    11523 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/extract.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/fetch.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    10378 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/format.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1760 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/main.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     2952 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/merge.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    14848 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/report.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)    10913 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/search.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     3022 2024-04-04 17:29:39.000000 locidex-0.1.2/locidex/utils.py
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)       22 2024-04-04 17:36:04.000000 locidex-0.1.2/locidex/version.py
+drwxr-x---   0 jarobert (101035) grp_jarobert (101035)        0 2024-04-04 17:36:16.000000 locidex-0.1.2/locidex.egg-info/
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)     1009 2024-04-04 17:36:15.000000 locidex-0.1.2/locidex.egg-info/PKG-INFO
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)      837 2024-04-04 17:36:15.000000 locidex-0.1.2/locidex.egg-info/SOURCES.txt
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)        1 2024-04-04 17:36:15.000000 locidex-0.1.2/locidex.egg-info/dependency_links.txt
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)       47 2024-04-04 17:36:15.000000 locidex-0.1.2/locidex.egg-info/entry_points.txt
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)       94 2024-04-04 17:36:15.000000 locidex-0.1.2/locidex.egg-info/requires.txt
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)        8 2024-04-04 17:36:15.000000 locidex-0.1.2/locidex.egg-info/top_level.txt
+-rwxr-x---   0 jarobert (101035) grp_jarobert (101035)       38 2024-04-04 17:36:16.000000 locidex-0.1.2/setup.cfg
+-rwxr-xr--   0 jarobert (101035) grp_jarobert (101035)     1882 2024-04-04 17:29:39.000000 locidex-0.1.2/setup.py
```

### Comparing `locidex-0.1.1/PKG-INFO` & `locidex-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: locidex
-Version: 0.1.1
+Version: 0.1.2
 Summary: Genomic Address Service: De novo clustering and cluster address assignment
 Home-page: https://github.com/phac-nml/locidex
 Author: James Robertson
 Author-email: james.robertson@phac-aspc.gc.ca
 License: GPLv3
 Description: UNKNOWN
 Keywords: cgMLST,wgMLST,outbreak,surveillance,blast,antimicrobial resistance,amr,virulence
```

### Comparing `locidex-0.1.1/README.md` & `locidex-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,1679 +1,1712 @@
 00000000: 5b21 5b50 7950 495d 2868 7474 7073 3a2f  [![PyPI](https:/
 00000010: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
 00000020: 6261 6467 652f 496e 7374 616c 6c25 3230  badge/Install%20
 00000030: 7769 7468 2d50 7950 492d 626c 7565 295d  with-PyPI-blue)]
 00000040: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
 00000050: 672f 7072 6f6a 6563 742f 6c6f 6369 6465  g/project/locide
-00000060: 782f 2364 6573 6372 6970 7469 6f6e 290a  x/#description).
-00000070: 5b21 5b42 696f 636f 6e64 615d 2868 7474  [![Bioconda](htt
-00000080: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000090: 2e69 6f2f 6261 6467 652f 496e 7374 616c  .io/badge/Instal
-000000a0: 6c25 3230 7769 7468 2d62 696f 636f 6e64  l%20with-biocond
-000000b0: 612d 6772 6565 6e29 5d28 6874 7470 733a  a-green)](https:
-000000c0: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f62  //anaconda.org/b
-000000d0: 696f 636f 6e64 612f 6c6f 6369 6465 7829  ioconda/locidex)
-000000e0: 0a5b 215b 436f 6e64 615d 2868 7474 7073  .[![Conda](https
-000000f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000100: 6f2f 636f 6e64 612f 646e 2f62 696f 636f  o/conda/dn/bioco
-00000110: 6e64 612f 6c6f 6369 6465 783f 636f 6c6f  nda/locidex?colo
-00000120: 723d 6772 6565 6e29 5d28 6874 7470 733a  r=green)](https:
-00000130: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f62  //anaconda.org/b
-00000140: 696f 636f 6e64 612f 6c6f 6369 6465 7829  ioconda/locidex)
-00000150: 0a5b 215b 4c69 6365 6e73 653a 2041 7061  .[![License: Apa
-00000160: 6368 652d 322e 305d 2868 7474 7073 3a2f  che-2.0](https:/
-00000170: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000180: 6769 7468 7562 2f6c 6963 656e 7365 2f70  github/license/p
-00000190: 6861 632d 6e6d 6c2f 6c6f 6369 6465 7829  hac-nml/locidex)
-000001a0: 5d28 6874 7470 733a 2f2f 7777 772e 6170  ](https://www.ap
-000001b0: 6163 6865 2e6f 7267 2f6c 6963 656e 7365  ache.org/license
-000001c0: 732f 4c49 4345 4e53 452d 322e 3029 0a0a  s/LICENSE-2.0)..
-000001d0: 0a23 2320 4c6f 6369 6465 780a 215b 616c  .## Locidex.![al
-000001e0: 7420 7465 7874 5d28 6874 7470 733a 2f2f  t text](https://
-000001f0: 6769 7468 7562 2e63 6f6d 2f70 6861 632d  github.com/phac-
-00000200: 6e6d 6c2f 6c6f 6369 6465 782f 626c 6f62  nml/locidex/blob
-00000210: 2f6d 6169 6e2f 6c6f 676f 2e70 6e67 3f72  /main/logo.png?r
-00000220: 6177 3d74 7275 6529 0a0a 2323 2043 6f6e  aw=true)..## Con
-00000230: 7465 6e74 730a 0a2d 205b 496e 7472 6f64  tents..- [Introd
-00000240: 7563 7469 6f6e 5d28 2369 6e74 726f 6475  uction](#introdu
-00000250: 6374 696f 6e29 0a2d 205b 496e 7374 616c  ction).- [Instal
-00000260: 6c61 7469 6f6e 5d28 2369 6e73 7461 6c6c  lation](#install
-00000270: 6174 696f 6e29 0a2d 205b 5573 6167 655d  ation).- [Usage]
-00000280: 2823 7573 6167 6529 0a2d 205b 5175 6963  (#usage).- [Quic
-00000290: 6b20 5374 6172 745d 2823 7175 6963 6b2d  k Start](#quick-
-000002a0: 7374 6172 7429 0a2d 205b 4641 515d 2823  start).- [FAQ](#
-000002b0: 6661 7129 0a2d 205b 4369 7461 7469 6f6e  faq).- [Citation
-000002c0: 5d28 2363 6974 6174 696f 6e29 0a2d 205b  ](#citation).- [
-000002d0: 4c65 6761 6c5d 2823 6c65 6761 6c29 0a2d  Legal](#legal).-
-000002e0: 205b 436f 6e74 6163 745d 2823 636f 6e74   [Contact](#cont
-000002f0: 6163 7429 0a0a 2323 2049 6e74 726f 6475  act)..## Introdu
-00000300: 6374 696f 6e0a 0a41 2063 6f6d 6d6f 6e20  ction..A common 
-00000310: 6675 6e63 7469 6f6e 2066 6f72 206d 616e  function for man
-00000320: 7920 746f 6f6c 7320 696e 2062 6163 7465  y tools in bacte
-00000330: 7269 616c 2074 7970 696e 6720 6973 2070  rial typing is p
-00000340: 6572 666f 726d 696e 6720 7369 6d69 6c61  erforming simila
-00000350: 7269 7479 2073 6561 7263 6869 6e67 2075  rity searching u
-00000360: 7369 6e67 204e 4342 4920 5b62 6c61 7374  sing NCBI [blast
-00000370: 5d28 6874 7470 733a 2f2f 626c 6173 742e  ](https://blast.
-00000380: 6e63 6269 2e6e 6c6d 2e6e 6968 2e67 6f76  ncbi.nlm.nih.gov
-00000390: 2f42 6c61 7374 2e63 6769 292e 200a 426c  /Blast.cgi). .Bl
-000003a0: 6173 7420 7072 6f76 6964 6573 2061 2072  ast provides a r
-000003b0: 6f62 7573 7420 636f 6d6d 616e 6420 6c69  obust command li
-000003c0: 6e65 2069 6e74 6572 6661 6365 2066 6f72  ne interface for
-000003d0: 2020 636f 6e73 7472 7563 7469 6e67 2061    constructing a
-000003e0: 6e64 2075 7369 6e67 2064 6174 6162 6173  nd using databas
-000003f0: 6573 2066 6f72 2073 696d 696c 6172 6974  es for similarit
-00000400: 7920 7365 6172 6368 696e 6720 616e 6420  y searching and 
-00000410: 6973 2075 6269 7175 6974 6f75 732e 2054  is ubiquitous. T
-00000420: 6865 7265 2061 7265 206d 616e 7920 7479  here are many ty
-00000430: 7069 6e67 200a 6170 706c 6963 6174 696f  ping .applicatio
-00000440: 6e73 2077 6865 7265 2063 7573 746f 6d20  ns where custom 
-00000450: 636f 6465 2069 7320 7772 6974 7465 6e20  code is written 
-00000460: 6172 6f75 6e64 2074 6865 2062 6c61 7374  around the blast
-00000470: 2063 6f6d 6d61 6e64 206c 696e 6520 696e   command line in
-00000480: 7465 7266 6163 6520 746f 2070 6572 666f  terface to perfo
-00000490: 726d 200a 7365 6172 6368 6573 2066 6f72  rm .searches for
-000004a0: 2061 2076 6172 6965 7479 206f 6620 646f   a variety of do
-000004b0: 776e 7374 7265 616d 2061 7070 6c69 6361  wnstream applica
-000004c0: 7469 6f6e 732e 204f 6e65 206d 616a 6f72  tions. One major
-000004d0: 2061 7070 6c69 6361 7469 6f6e 2077 6974   application wit
-000004e0: 6869 6e20 7075 626c 6963 2068 6561 6c74  hin public healt
-000004f0: 6820 6973 2069 6465 6e74 6966 6963 6174  h is identificat
-00000500: 696f 6e20 6f66 200a 7370 6563 6966 6963  ion of .specific
-00000510: 2074 6172 6765 7420 7365 7175 656e 6365   target sequence
-00000520: 7320 7769 7468 696e 2061 6e20 6173 7365  s within an asse
-00000530: 6d62 6c79 2074 6f20 7065 7266 6f72 6d20  mbly to perform 
-00000540: 6765 6e65 2d62 792d 6765 6e65 2070 6879  gene-by-gene phy
-00000550: 6c6f 6765 6e65 7469 6320 616e 616c 7973  logenetic analys
-00000560: 6973 200a 284d 4c53 542c 2063 674d 4c53  is .(MLST, cgMLS
-00000570: 542c 2077 674d 4c53 5429 2c20 616e 7469  T, wgMLST), anti
-00000580: 6d69 6372 6f62 6961 6c20 7265 7369 7374  microbial resist
-00000590: 616e 6365 2067 656e 6520 6465 7465 6374  ance gene detect
-000005a0: 696f 6e2c 2076 6972 756c 656e 6365 2067  ion, virulence g
-000005b0: 656e 6520 6465 7465 6374 696f 6e2c 2061  ene detection, a
-000005c0: 6e64 2069 6e20 7369 6c69 636f 2070 7265  nd in silico pre
-000005d0: 6469 6374 696f 6e73 206f 6620 0a70 6865  dictions of .phe
-000005e0: 6e6f 7479 7065 7320 7375 6368 2061 7320  notypes such as 
-000005f0: 7365 726f 7479 7065 2e20 5468 6520 7479  serotype. The ty
-00000600: 7069 6361 6c20 6170 7072 6f61 6368 2069  pical approach i
-00000610: 7320 746f 2062 756e 646c 6520 7468 6520  s to bundle the 
-00000620: 7365 6172 6368 2d62 6173 6564 206c 6f67  search-based log
-00000630: 6963 2077 6974 6820 6164 6469 7469 6f6e  ic with addition
-00000640: 616c 2073 7065 6369 616c 697a 6564 206c  al specialized l
-00000650: 6f67 6963 200a 666f 7220 7065 7266 6f72  ogic .for perfor
-00000660: 6d69 6e67 2074 6865 2064 6573 6972 6564  ming the desired
-00000670: 2061 6e61 6c79 7369 732e 2020 200a 0a44   analysis.   ..D
-00000680: 6563 656e 7472 616c 697a 6564 2061 6c6c  ecentralized all
-00000690: 656c 6520 6361 6c6c 696e 6720 6861 7320  ele calling has 
-000006a0: 6265 636f 6d65 2061 2070 7265 7373 696e  become a pressin
-000006b0: 6720 636f 6e63 6572 6e20 6279 2070 7562  g concern by pub
-000006c0: 6c69 6320 6865 616c 7468 206c 6162 6f72  lic health labor
-000006d0: 6174 6f72 6965 7320 6475 6520 746f 2074  atories due to t
-000006e0: 6865 2069 6e63 7265 6173 6564 2075 7365  he increased use
-000006f0: 206f 6620 0a77 686f 6c65 2067 656e 6f6d   of .whole genom
-00000700: 6520 7365 7175 656e 6369 6e67 2028 5747  e sequencing (WG
-00000710: 5329 2061 7320 7061 7274 206f 6620 6f75  S) as part of ou
-00000720: 7462 7265 616b 2064 6574 6563 7469 6f6e  tbreak detection
-00000730: 2061 6e64 2073 7572 7665 696c 6c61 6e63   and surveillanc
-00000740: 6520 6f66 2020 6120 7661 7269 6574 7920  e of  a variety 
-00000750: 6f66 2070 6174 686f 6765 6e73 2e20 0a47  of pathogens. .G
-00000760: 656e 652d 6279 2d67 656e 6520 6170 7072  ene-by-gene appr
-00000770: 6f61 6368 6573 2068 6176 6520 6120 7661  oaches have a va
-00000780: 7269 6574 7920 6f66 2062 656e 6566 6974  riety of benefit
-00000790: 7320 7369 6e63 6520 7468 6520 696e 7472  s since the intr
-000007a0: 6f64 7563 7469 6f6e 206f 6620 372d 6765  oduction of 7-ge
-000007b0: 6e65 204d 4c53 5420 6170 7072 6f61 6368  ne MLST approach
-000007c0: 6573 2066 6f72 2073 7065 6369 6573 2074  es for species t
-000007d0: 7970 696e 6720 0a77 6869 6368 2069 6e63  yping .which inc
-000007e0: 6c75 6465 2061 2073 7461 6e64 6172 6469  lude a standardi
-000007f0: 7a65 6420 7365 7420 6f66 206c 6f63 6920  zed set of loci 
-00000800: 666f 7220 6573 7469 6d61 7469 6e67 2067  for estimating g
-00000810: 656e 6574 6963 2073 696d 696c 6172 6974  enetic similarit
-00000820: 7920 6265 7477 6565 6e20 7361 6d70 6c65  y between sample
-00000830: 732e 2054 6869 7320 7374 616e 6461 7264  s. This standard
-00000840: 697a 6174 696f 6e20 616c 6c6f 7773 200a  ization allows .
-00000850: 666f 7220 696e 7465 726f 7065 7261 6269  for interoperabi
-00000860: 6c69 7479 2062 6574 7765 656e 2064 6966  lity between dif
-00000870: 6665 7265 6e74 2067 726f 7570 7320 616e  ferent groups an
-00000880: 6420 616c 736f 2068 6173 2074 6865 2062  d also has the b
-00000890: 656e 6566 6974 7320 6f66 2063 6f6d 7072  enefits of compr
-000008a0: 6573 7369 6f6e 2062 7920 7369 6d70 6c69  ession by simpli
-000008b0: 6679 696e 6720 6765 6e65 7469 6320 636f  fying genetic co
-000008c0: 6d70 6172 6973 6f6e 7320 0a74 6f20 7573  mparisons .to us
-000008d0: 6520 6120 7369 6d70 6c65 2068 616d 6d69  e a simple hammi
-000008e0: 6e67 2064 6973 7461 6e63 6520 6261 7365  ng distance base
-000008f0: 6420 6f6e 2061 6c6c 656c 6520 6964 656e  d on allele iden
-00000900: 7469 6669 6572 7320 696e 7374 6561 6420  tifiers instead 
-00000910: 6f66 2061 2077 686f 6c65 2073 6571 7565  of a whole seque
-00000920: 6e63 652e 2048 6f77 6576 6572 2c20 6120  nce. However, a 
-00000930: 6c69 6d69 7461 7469 6f6e 206f 6620 7468  limitation of th
-00000940: 6973 200a 6170 7072 6f61 6368 2069 7320  is .approach is 
-00000950: 7468 6520 7265 7175 6972 656d 656e 7420  the requirement 
-00000960: 6f66 2061 2063 656e 7472 616c 697a 6564  of a centralized
-00000970: 2061 7574 686f 7269 7479 2074 6f20 6973   authority to is
-00000980: 7375 6520 756e 6971 7565 2061 6c6c 656c  sue unique allel
-00000990: 6520 6964 656e 7469 6669 6572 2061 6e64  e identifier and
-000009a0: 2074 6869 7320 706f 7365 7320 6d75 6c74   this poses mult
-000009b0: 6970 6c65 2070 726f 626c 656d 7320 0a66  iple problems .f
-000009c0: 6f72 206f 7065 7261 7469 6f6e 616c 697a  or operationaliz
-000009d0: 6174 696f 6e20 7375 6368 2061 7320 7072  ation such as pr
-000009e0: 6976 6163 7920 616e 6420 636f 6e6e 6563  ivacy and connec
-000009f0: 7469 7669 7479 2e20 4465 7370 6974 6520  tivity. Despite 
-00000a00: 7468 6973 206c 696d 6974 6174 696f 6e20  this limitation 
-00000a10: 5075 6c73 654e 6574 2049 6e74 6572 6e61  PulseNet Interna
-00000a20: 7469 6f6e 616c 2068 6173 2061 646f 7074  tional has adopt
-00000a30: 6564 200a 6765 6e65 2d62 792d 6765 6e65  ed .gene-by-gene
-00000a40: 2061 6e61 6c79 7369 7320 6173 2069 7473   analysis as its
-00000a50: 2070 7265 6665 7272 6564 2061 6e61 6c79   preferred analy
-00000a60: 7469 6361 6c20 6170 7072 6f61 6368 2066  tical approach f
-00000a70: 6f72 2065 7374 696d 6174 696e 6720 6765  or estimating ge
-00000a80: 6e65 7469 6320 7369 6d69 6c61 7269 7479  netic similarity
-00000a90: 2062 6574 7765 656e 2073 616d 706c 6573   between samples
-00000aa0: 2066 6f72 200a 726f 7574 696e 6520 6f70   for .routine op
-00000ab0: 6572 6174 696f 6e73 2077 6974 6820 7468  erations with th
-00000ac0: 6520 6c69 6d69 7461 7469 6f6e 2074 6861  e limitation tha
-00000ad0: 7420 636f 6d70 6172 696e 6720 6265 7477  t comparing betw
-00000ae0: 6565 6e20 6a75 7269 7364 6963 7469 6f6e  een jurisdiction
-00000af0: 7320 7265 7175 6972 6573 2074 6865 2073  s requires the s
-00000b00: 6861 7269 6e67 206f 6620 7468 6520 7072  haring of the pr
-00000b10: 696d 6172 7920 0a73 6571 7565 6e63 6520  imary .sequence 
-00000b20: 6461 7461 2072 6174 6865 7220 7468 616e  data rather than
-00000b30: 2074 6865 2061 6c6c 656c 6520 6964 656e   the allele iden
-00000b40: 7469 6669 6572 732e 2020 200a 0a49 6e20  tifiers.   ..In 
-00000b50: 7265 6365 6e74 2079 6561 7273 2c20 7468  recent years, th
-00000b60: 6520 636f 6e63 6570 7420 6f66 2075 7369  e concept of usi
-00000b70: 6e67 2063 7279 7074 6f67 7261 7068 6963  ng cryptographic
-00000b80: 2068 6173 6865 7320 6f66 2074 6865 200a   hashes of the .
-00000b90: 616c 6c65 6c65 2073 6571 7565 6e63 6520  allele sequence 
-00000ba0: 6974 7365 6c66 2068 6176 6520 6761 696e  itself have gain
-00000bb0: 6564 2074 7261 6374 696f 6e20 696e 2061  ed traction in a
-00000bc0: 2076 6172 6965 7479 206f 6620 6469 6666   variety of diff
-00000bd0: 6572 656e 7420 616c 6c65 6c65 2063 616c  erent allele cal
-00000be0: 6c69 6e67 2073 6f66 7477 6172 6520 7375  ling software su
-00000bf0: 6368 2061 7320 0a5b 4368 6577 6262 6163  ch as .[Chewbbac
-00000c00: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-00000c10: 622e 636f 6d2f 422d 554d 4d49 2f63 6865  b.com/B-UMMI/che
-00000c20: 7742 4241 4341 2920 746f 200a 7072 6f76  wBBACA) to .prov
-00000c30: 6964 6520 6465 6365 6e74 7261 6c69 7a65  ide decentralize
-00000c40: 6420 616c 6c65 6c65 2069 6465 6e74 6966  d allele identif
-00000c50: 6965 7273 2e20 4861 7368 696e 6720 7468  iers. Hashing th
-00000c60: 6520 7365 7175 656e 6365 2079 6965 6c64  e sequence yield
-00000c70: 7320 6120 6465 7465 726d 696e 6973 7420  s a determinist 
-00000c80: 616e 6420 6669 7865 642d 7369 7a65 2068  and fixed-size h
-00000c90: 6173 6820 7661 6c75 6520 7768 6963 6820  ash value which 
-00000ca0: 0a63 616e 2062 6520 636f 6d70 6172 6564  .can be compared
-00000cb0: 2069 6e20 7468 6520 7361 6d65 206d 616e   in the same man
-00000cc0: 6e65 7220 6173 2069 6e74 6567 6572 732e  ner as integers.
-00000cd0: 2054 6865 7265 2061 7265 206e 756d 6572   There are numer
-00000ce0: 6f75 7320 6861 7368 2066 756e 6374 696f  ous hash functio
-00000cf0: 6e73 2077 6974 6820 6469 6666 6572 656e  ns with differen
-00000d00: 7420 7374 7265 6e67 7468 7320 616e 6420  t strengths and 
-00000d10: 7765 616b 6e65 7373 6573 200a 6275 7420  weaknesses .but 
-00000d20: 4d44 3520 6469 6765 7374 7320 6861 7665  MD5 digests have
-00000d30: 2062 726f 6164 2061 646f 7074 696f 6e20   broad adoption 
-00000d40: 696e 2074 6865 2073 6f66 7477 6172 6520  in the software 
-00000d50: 636f 6d6d 756e 6974 7920 616e 6420 6172  community and ar
-00000d60: 6520 726f 7574 696e 656c 7920 7573 6564  e routinely used
-00000d70: 2074 6f20 7072 6f76 6964 6520 736f 6d65   to provide some
-00000d80: 2061 7373 7572 616e 6365 2074 6861 7420   assurance that 
-00000d90: 6120 0a74 7261 6e73 6665 7272 6564 2066  a .transferred f
-00000da0: 696c 6520 6861 7320 6172 7269 7665 6420  ile has arrived 
-00000db0: 696e 7461 6374 2e20 2054 6865 2063 686f  intact.  The cho
-00000dc0: 6963 6520 6f66 206d 6435 2068 6173 6820  ice of md5 hash 
-00000dd0: 7072 6f76 6964 6573 2031 365e 3332 2c20  provides 16^32, 
-00000de0: 706f 7373 6962 6c65 2068 6173 6865 732e  possible hashes.
-00000df0: 200a 5468 6572 6520 6973 2061 2074 6865   .There is a the
-00000e00: 6f72 6574 6963 616c 2063 6861 6e63 6520  oretical chance 
-00000e10: 6f66 2068 6173 6820 636f 6c6c 6973 696f  of hash collisio
-00000e20: 6e73 2c20 692e 652e 2c20 6469 6666 6572  ns, i.e., differ
-00000e30: 656e 7420 7365 7175 656e 6365 7320 7265  ent sequences re
-00000e40: 7375 6c74 696e 6720 696e 2074 6865 2073  sulting in the s
-00000e50: 616d 6520 6861 7368 2c20 6275 7420 6173  ame hash, but as
-00000e60: 2074 6865 206e 756d 6265 7220 0a6f 6620   the number .of 
-00000e70: 616c 6c65 6c65 2073 6571 7565 6e63 6573  allele sequences
-00000e80: 2066 6f72 2065 6163 6820 6765 6e65 2069   for each gene i
-00000e90: 6e20 6461 7461 6261 7365 7320 6973 2072  n databases is r
-00000ea0: 656c 6174 6976 656c 7920 6c6f 772c 2074  elatively low, t
-00000eb0: 6869 7320 7368 6f75 6c64 2062 6520 616e  his should be an
-00000ec0: 2075 6e63 6f6d 6d6f 6e20 6f63 6375 7272   uncommon occurr
-00000ed0: 656e 6365 2e20 436f 6c6c 6973 696f 6e73  ence. Collisions
-00000ee0: 2069 6e20 0a74 6869 7320 6361 7365 2077   in .this case w
-00000ef0: 6f75 6c64 206a 7573 7420 6861 7665 2074  ould just have t
-00000f00: 6865 2063 6f6e 7365 7175 656e 6365 206f  he consequence o
-00000f10: 6620 6861 7669 6e67 2061 2070 726f 6669  f having a profi
-00000f20: 6c65 2061 7070 6561 7220 6d6f 7265 2073  le appear more s
-00000f30: 696d 696c 6172 2074 6861 6e20 7468 6579  imilar than they
-00000f40: 2074 7275 6c79 2061 7265 2061 7420 7468   truly are at th
-00000f50: 6520 7365 7175 656e 6365 200a 6c65 7665  e sequence .leve
-00000f60: 6c20 6275 7420 7468 6520 6368 616e 6365  l but the chance
-00000f70: 7320 6f66 206d 756c 7469 706c 6520 6f63  s of multiple oc
-00000f80: 6375 7272 656e 6365 7320 6f66 2063 6f6c  currences of col
-00000f90: 6c69 7369 6f6e 7320 7769 7468 696e 2061  lisions within a
-00000fa0: 2070 726f 6669 6c65 2077 6f75 6c64 2062   profile would b
-00000fb0: 6520 696e 6669 6e69 7465 6c79 2073 6d61  e infinitely sma
-00000fc0: 6c6c 2e20 200a 0a54 6865 206d 6f74 6976  ll.  ..The motiv
-00000fd0: 6174 696f 6e20 666f 7220 6465 7665 6c6f  ation for develo
-00000fe0: 7069 6e67 206c 6f63 6964 6578 2069 7320  ping locidex is 
-00000ff0: 7468 6520 6e65 6564 2061 2063 6f6d 6d6f  the need a commo
-00001000: 6e20 7365 6172 6368 696e 6720 656e 6769  n searching engi
-00001010: 6e65 2066 6f72 2076 6172 696f 7573 206c  ne for various l
-00001020: 6f63 6920 6261 7365 6420 7479 7069 6e67  oci based typing
-00001030: 2061 7070 6c69 6361 7469 6f6e 7320 0a73   applications .s
-00001040: 7563 6820 6173 3a20 6765 6e65 2d62 792d  uch as: gene-by-
-00001050: 6765 6e65 2028 6d6c 7374 2c20 6367 4d4c  gene (mlst, cgML
-00001060: 5354 2c20 7767 4d4c 5354 2c20 726d 6c73  ST, wgMLST, rmls
-00001070: 7429 2c20 696e 2073 696c 6963 6f20 7365  t), in silico se
-00001080: 726f 7479 7069 6e67 2c20 6765 6e65 2d62  rotyping, gene-b
-00001090: 6173 6564 2070 6865 6e6f 7479 7065 2070  ased phenotype p
-000010a0: 7265 6469 6374 696f 6e73 200a 2861 6d72  redictions .(amr
-000010b0: 2c20 7669 7275 6c65 6e63 652c 2070 6174  , virulence, pat
-000010c0: 686f 7479 7065 2c20 746f 7869 6e20 7479  hotype, toxin ty
-000010d0: 7069 6e67 292c 206d 6172 6b65 722d 6261  ping), marker-ba
-000010e0: 7365 6420 7479 7069 6e67 2028 3136 5329  sed typing (16S)
-000010f0: 2e20 2054 6865 2074 6f6f 6c20 6e65 6564  .  The tool need
-00001100: 7320 746f 2070 726f 7669 6465 2063 7573  s to provide cus
-00001110: 746f 6d20 6372 6974 6572 6961 2066 696c  tom criteria fil
-00001120: 7465 7269 6e67 200a 6279 206c 6f63 692c  tering .by loci,
-00001130: 2061 6e64 2061 6269 6c69 7479 2074 6f20   and ability to 
-00001140: 7072 6f64 7563 6520 6d75 6c74 6970 6c65  produce multiple
-00001150: 2066 6f72 6d61 7473 2066 6f72 2064 6966   formats for dif
-00001160: 6665 7265 6e74 2064 6f77 6e73 7472 6561  ferent downstrea
-00001170: 6d20 6170 706c 6963 6174 696f 6e73 2074  m applications t
-00001180: 6f20 7573 652e 2054 6865 2074 6f6f 6c20  o use. The tool 
-00001190: 6e65 6564 7320 746f 2062 6520 0a63 6f6d  needs to be .com
-000011a0: 7061 7469 626c 6520 7769 7468 2061 6e20  patible with an 
-000011b0: 4853 5020 656e 7669 726f 6e6d 656e 7420  HSP environment 
-000011c0: 616e 6420 6e6f 7420 656e 636f 756e 7465  and not encounte
-000011d0: 7220 616e 7920 6c6f 636b 696e 6720 6973  r any locking is
-000011e0: 7375 6573 2077 6865 7265 206d 756c 7469  sues where multi
-000011f0: 706c 6520 7072 6f63 6573 7365 7320 6d61  ple processes ma
-00001200: 7920 7472 7920 746f 2063 6861 6e67 6520  y try to change 
-00001210: 7468 6520 0a64 6174 6120 6174 2074 6865  the .data at the
-00001220: 2073 616d 6520 7469 6d65 2e20 2054 6865   same time.  The
-00001230: 206c 6f67 6963 2066 6f72 2061 6c6c 656c   logic for allel
-00001240: 6520 6361 6c6c 696e 6720 6973 2067 7265  e calling is gre
-00001250: 6174 6c79 2073 696d 706c 6966 6965 6420  atly simplified 
-00001260: 6279 206c 6576 6572 6167 696e 6720 6578  by leveraging ex
-00001270: 6973 7469 6e67 2061 6e6e 6f74 6174 696f  isting annotatio
-00001280: 6e73 2066 726f 6d20 746f 6f6c 7320 0a73  ns from tools .s
-00001290: 7563 6820 6173 205b 7072 6f64 6967 616c  uch as [prodigal
-000012a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000012b0: 2e63 6f6d 2f68 7961 7474 7064 2f50 726f  .com/hyattpd/Pro
-000012c0: 6469 6761 6c29 2c20 5b70 726f 6b6b 615d  digal), [prokka]
-000012d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000012e0: 636f 6d2f 7473 6565 6d61 6e6e 2f70 726f  com/tseemann/pro
-000012f0: 6b6b 6129 2c20 0a5b 6261 6b74 615d 2868  kka), .[bakta](h
-00001300: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001310: 6d2f 6f73 6368 7765 6e67 6572 732f 6261  m/oschwengers/ba
-00001320: 6b74 6129 2074 6f20 6465 6c69 6e61 7465  kta) to delinate
-00001330: 2074 6865 2062 6f75 6e64 6172 6965 7320   the boundaries 
-00001340: 6f66 2074 6865 2073 6571 7565 6e63 6573  of the sequences
-00001350: 2074 6f20 6265 2071 7565 7269 6564 2061   to be queried a
-00001360: 6e64 2068 6173 6865 6420 746f 2070 726f  nd hashed to pro
-00001370: 6475 6365 2061 6c6c 656c 6520 0a69 6465  duce allele .ide
-00001380: 6e74 6966 6965 7273 2e20 4120 636f 6d6d  ntifiers. A comm
-00001390: 6f6e 2069 7373 7565 2069 6e20 6d61 7463  on issue in matc
-000013a0: 6869 6e67 2061 7070 6c69 6361 7469 6f6e  hing application
-000013b0: 7320 6973 2074 6861 7420 7261 6e67 6573  s is that ranges
-000013c0: 206f 6620 6964 656e 7469 7479 2061 6e64   of identity and
-000013d0: 2063 6f76 6572 6167 6520 666f 7220 6120   coverage for a 
-000013e0: 6d61 7463 6820 7769 6c6c 2076 6172 7920  match will vary 
-000013f0: 6279 206c 6f63 7573 200a 616e 6420 736f  by locus .and so
-00001400: 206c 6f63 6964 6578 2062 7569 6c64 7320   locidex builds 
-00001410: 696e 746f 2069 7473 2064 6174 6162 6173  into its databas
-00001420: 6520 7374 7275 6374 7572 6520 636f 6e74  e structure cont
-00001430: 726f 6c20 6f76 6572 2074 6865 7365 2061  rol over these a
-00001440: 7474 7269 6275 7465 7320 6174 2061 206c  ttributes at a l
-00001450: 6f63 7573 206c 6576 656c 2077 6869 6368  ocus level which
-00001460: 2061 6c6c 6f77 7320 666f 7220 0a68 6967   allows for .hig
-00001470: 6820 7661 7269 6162 696c 6974 7920 6461  h variability da
-00001480: 7461 6261 7365 7320 746f 2062 6520 7573  tabases to be us
-00001490: 6564 2077 6974 686f 7574 2062 7569 6c64  ed without build
-000014a0: 696e 6720 6375 7374 6f6d 206c 6f67 6963  ing custom logic
-000014b0: 2064 6f77 6e73 7472 6561 6d2e 2054 6869   downstream. Thi
-000014c0: 7320 6973 2070 6172 7469 6375 6c61 726c  s is particularl
-000014d0: 7920 696d 706f 7274 616e 7420 7768 656e  y important when
-000014e0: 206c 656e 6774 6873 200a 6f66 206c 6f63   lengths .of loc
-000014f0: 6920 6361 6e20 6578 6869 6269 7420 636f  i can exhibit co
-00001500: 6e73 6964 6572 6162 6c65 2076 6172 6961  nsiderable varia
-00001510: 6269 6c69 7479 2061 7320 6973 2074 6865  bility as is the
-00001520: 2063 6173 6520 666f 7220 6765 6e65 7320   case for genes 
-00001530: 6f66 2069 6e74 6572 6573 7420 666f 7220  of interest for 
-00001540: 7479 7069 6e67 2061 7070 6c69 6361 7469  typing applicati
-00001550: 6f6e 732e 200a 5468 6973 2070 726f 7669  ons. .This provi
-00001560: 6465 7320 6772 6561 7465 7220 666c 6578  des greater flex
-00001570: 6962 696c 6974 7920 666f 7220 7468 6520  ibility for the 
-00001580: 6465 7369 676e 6174 696f 6e20 6f66 2069  designation of i
-00001590: 6465 616c 2074 6872 6573 686f 6c64 7320  deal thresholds 
-000015a0: 666f 7220 6120 6769 7665 6e20 6170 706c  for a given appl
-000015b0: 6963 6174 696f 6e2e 200a 486f 7765 7665  ication. .Howeve
-000015c0: 722c 2074 6865 7365 2076 616c 7565 7320  r, these values 
-000015d0: 6361 6e20 6265 206f 7665 7272 6964 6465  can be overridde
-000015e0: 6e20 7573 696e 6720 7468 6520 7265 706f  n using the repo
-000015f0: 7274 206d 6f64 756c 6520 6669 6c74 6572  rt module filter
-00001600: 696e 6720 7061 7261 6d65 7465 7273 2061  ing parameters a
-00001610: 7320 7765 6c6c 2061 7320 6279 206d 6f64  s well as by mod
-00001620: 6966 7969 6e67 2074 6865 2076 616c 7565  ifying the value
-00001630: 7320 0a77 6974 6869 6e20 7468 6520 6461  s .within the da
-00001640: 7461 6261 7365 2e20 0a0a 4c6f 6369 6465  tabase. ..Locide
-00001650: 7820 6973 206d 6561 6e74 2074 6f20 6265  x is meant to be
-00001660: 206f 7074 696d 697a 6564 2066 6f72 2072   optimized for r
-00001670: 6f75 7469 6e65 206f 7065 7261 7469 6f6e  outine operation
-00001680: 206c 6576 656c 2073 6561 7263 6869 6e67   level searching
-00001690: 2077 6865 7265 2069 7420 6973 2075 7365   where it is use
-000016a0: 6675 6c20 746f 2068 6176 6520 0a64 6566  ful to have .def
-000016b0: 6175 6c74 2070 6172 616d 6574 6572 7320  ault parameters 
-000016c0: 7468 6174 2061 7265 2073 6574 2066 6f72  that are set for
-000016d0: 2074 6865 2075 7365 7220 746f 2068 6176   the user to hav
-000016e0: 6520 7265 7072 6f64 7563 6962 696c 6974  e reproducibilit
-000016f0: 792c 2077 6869 6368 2069 7320 636f 6d62  y, which is comb
-00001700: 696e 6564 2077 6974 6820 666c 6578 6962  ined with flexib
-00001710: 696c 6974 7920 746f 2020 6170 706c 7920  ility to  apply 
-00001720: 0a6d 756c 7469 706c 6520 6669 6c74 6572  .multiple filter
-00001730: 696e 6720 7061 7261 6d65 7465 7273 206f  ing parameters o
-00001740: 6e20 7468 6520 7365 7175 656e 6365 2073  n the sequence s
-00001750: 746f 7265 2061 6674 6572 2074 6865 2066  tore after the f
-00001760: 6163 742e 2054 6869 7320 616c 6c6f 7773  act. This allows
-00001770: 2065 7870 6c6f 7269 6e67 2064 6966 6665   exploring diffe
-00001780: 7265 6e74 2074 6872 6573 686f 6c64 7320  rent thresholds 
-00001790: 0a77 6974 686f 7574 2074 6865 206e 6565  .without the nee
-000017a0: 6420 746f 2072 6563 6f6d 7075 7465 2062  d to recompute b
-000017b0: 6c61 7374 2073 6561 7263 6865 7320 6561  last searches ea
-000017c0: 6368 2074 696d 6520 616e 6420 616c 6c6f  ch time and allo
-000017d0: 7773 2066 6f72 2064 6966 6665 7265 6e74  ws for different
-000017e0: 2075 7365 2063 6173 6573 206f 6620 6461   use cases of da
-000017f0: 7461 2066 726f 6d20 6120 636f 6d6d 6f6e  ta from a common
-00001800: 2064 6174 6120 7374 6f72 652e 200a 4672   data store. .Fr
-00001810: 6571 7565 6e74 6c79 2074 6865 7265 2069  equently there i
-00001820: 7320 6120 6465 7369 7265 2074 6f20 696e  s a desire to in
-00001830: 636c 7564 6520 6164 6469 7469 6f6e 616c  clude additional
-00001840: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00001850: 7574 2067 6976 656e 206c 6f63 7573 2073  ut given locus s
-00001860: 7563 6820 6173 2064 6966 6665 7265 6e74  uch as different
-00001870: 2069 6465 6e74 6966 6965 7273 2c20 0a66   identifiers, .f
-00001880: 756e 6374 696f 6e61 6c20 7072 6f70 6572  unctional proper
-00001890: 7469 6573 2c20 616e 6420 7068 656e 6f74  ties, and phenot
-000018a0: 7970 6963 2065 6666 6563 7473 2e20 2054  ypic effects.  T
-000018b0: 6865 2064 6174 6162 6173 6520 666f 726d  he database form
-000018c0: 6174 206f 6620 6c6f 6369 6465 7820 616c  at of locidex al
-000018d0: 6c6f 7773 2069 6e63 6c75 7369 6f6e 206f  lows inclusion o
-000018e0: 6620 616e 7920 6e75 6d62 6572 206f 6620  f any number of 
-000018f0: 6669 656c 6473 200a 7468 6174 2061 6c6c  fields .that all
-00001900: 6f77 2074 6865 2075 7365 7220 746f 2064  ow the user to d
-00001910: 6573 6372 6962 6520 7468 6569 7220 6461  escribe their da
-00001920: 7461 2077 6869 6368 2069 7320 6275 6e64  ta which is bund
-00001930: 6c65 6420 696e 746f 2074 6865 2073 6561  led into the sea
-00001940: 7263 6820 7265 7375 6c74 206f 626a 6563  rch result objec
-00001950: 7420 666f 7220 636f 6e76 656e 6965 6e63  t for convenienc
-00001960: 6520 746f 2064 6f77 6e73 7472 6561 6d20  e to downstream 
-00001970: 616e 616c 7973 6573 2e0a 5b43 6865 7762  analyses..[Chewb
-00001980: 6261 6361 5d28 6874 7470 733a 2f2f 6769  baca](https://gi
-00001990: 7468 7562 2e63 6f6d 2f42 2d55 4d4d 492f  thub.com/B-UMMI/
-000019a0: 6368 6577 4242 4143 4129 2069 7320 616e  chewBBACA) is an
-000019b0: 2065 7863 656c 6c65 6e74 2063 686f 6963   excellent choic
-000019c0: 6520 666f 7220 616e 206f 7065 6e20 736f  e for an open so
-000019d0: 7572 6365 2061 6c6c 656c 6520 6361 6c6c  urce allele call
-000019e0: 6572 2061 6e64 2070 726f 7669 6465 7320  er and provides 
-000019f0: 6d61 6e79 2061 6476 616e 6365 6420 6665  many advanced fe
-00001a00: 6174 7572 6573 200a 666f 7220 6465 7665  atures .for deve
-00001a10: 6c6f 7069 6e67 2c20 6375 7261 7469 6e67  loping, curating
-00001a20: 2061 6e64 2075 7369 6e67 2067 656e 652d   and using gene-
-00001a30: 6279 2d67 656e 6520 7363 6865 6d65 732e  by-gene schemes.
-00001a40: 2020 4974 2070 726f 7669 6465 7320 6120    It provides a 
-00001a50: 6772 6561 7420 6465 6174 206f 6620 6164  great deat of ad
-00001a60: 6469 7469 6f6e 616c 2069 6e66 6f72 6d61  ditional informa
-00001a70: 7469 6f6e 2072 6567 6172 6469 6e67 2070  tion regarding p
-00001a80: 6172 7469 616c 2067 656e 6520 7365 7175  artial gene sequ
-00001a90: 656e 6365 732e 200a 466f 7220 5226 4420  ences. .For R&D 
-00001aa0: 6170 706c 6963 6174 696f 6e73 2c20 7468  applications, th
-00001ab0: 6973 2066 756e 6374 696f 6e61 6c69 7479  is functionality
-00001ac0: 2063 616e 2062 6520 6578 7472 656d 656c   can be extremel
-00001ad0: 7920 7573 6566 756c 2e20 486f 7765 7665  y useful. Howeve
-00001ae0: 722c 2066 6f72 2073 6f6d 6520 6f70 6572  r, for some oper
-00001af0: 6174 696f 6e61 6c20 636f 6e74 6578 7473  ational contexts
-00001b00: 2c20 7468 6520 6465 7369 676e 206f 6620  , the design of 
-00001b10: 5b43 6865 7762 6261 6361 5d28 6874 7470  [Chewbbaca](http
-00001b20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f42  s://github.com/B
-00001b30: 2d55 4d4d 492f 6368 6577 4242 4143 4129  -UMMI/chewBBACA)
-00001b40: 0a70 726f 7669 6465 7320 696e 666f 726d  .provides inform
-00001b50: 6174 696f 6e20 7468 6174 2069 7320 6e6f  ation that is no
-00001b60: 7420 6465 7369 7265 6162 6c65 2061 6e64  t desireable and
-00001b70: 2061 7420 7072 6573 656e 7420 6974 2068   at present it h
-00001b80: 6173 2069 7373 7565 7320 7769 7468 206d  as issues with m
-00001b90: 756c 7469 706c 6520 696e 7374 616e 6365  ultiple instance
-00001ba0: 7320 7573 696e 6720 7468 6520 7361 6d65  s using the same
-00001bb0: 2064 6174 6162 6173 6520 6174 206f 6e63   database at onc
-00001bc0: 6520 7769 7468 200a 6e6f 7665 6c20 616c  e with .novel al
-00001bd0: 6c65 6c65 2064 6574 6563 7469 6f6e 2065  lele detection e
-00001be0: 6e61 626c 6564 2028 6874 7470 733a 2f2f  nabled (https://
-00001bf0: 6769 7468 7562 2e63 6f6d 2f42 2d55 4d4d  github.com/B-UMM
-00001c00: 492f 6368 6577 4242 4143 412f 6973 7375  I/chewBBACA/issu
-00001c10: 6573 2f31 3638 292e 204c 6f63 6964 6578  es/168). Locidex
-00001c20: 2064 6f65 7320 6e6f 7420 6861 7665 2074   does not have t
-00001c30: 6865 2066 756c 6c20 6665 6174 7572 6573  he full features
-00001c40: 2066 6f72 2061 2067 656e 652d 6279 2d67   for a gene-by-g
-00001c50: 656e 6520 736f 6674 7761 7265 2070 6163  ene software pac
-00001c60: 6b61 6765 206c 696b 6520 5b43 6865 7762  kage like [Chewb
-00001c70: 6261 6361 5d28 6874 7470 733a 2f2f 6769  baca](https://gi
-00001c80: 7468 7562 2e63 6f6d 2f42 2d55 4d4d 492f  thub.com/B-UMMI/
-00001c90: 6368 6577 4242 4143 4129 0a62 7574 2063  chewBBACA).but c
-00001ca0: 616e 2062 6520 7573 6564 2074 6f20 6163  an be used to ac
-00001cb0: 6865 6976 6520 7369 6d69 6c61 7220 7265  heive similar re
-00001cc0: 7375 6c74 7320 7768 696c 6520 6265 696e  sults while bein
-00001cd0: 6720 6120 6d6f 7265 2067 656e 6572 6963  g a more generic
-00001ce0: 2074 6f6f 6c20 6b69 7420 666f 7220 626c   tool kit for bl
-00001cf0: 6173 7420 7365 6172 6368 6573 2073 7563  ast searches suc
-00001d00: 6820 6173 205b 6162 7269 6361 7465 5d28  h as [abricate](
-00001d10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001d20: 6f6d 2f74 7365 656d 616e 6e2f 6162 7269  om/tseemann/abri
-00001d30: 6361 7465 290a 0a0a 2323 2049 6e73 7461  cate)...## Insta
-00001d40: 6c6c 6174 696f 6e0a 0a49 6e73 7461 6c6c  llation..Install
-00001d50: 2074 6865 206c 6174 6573 7420 7265 6c65   the latest rele
-00001d60: 6173 6564 2076 6572 7369 6f6e 2066 726f  ased version fro
-00001d70: 6d20 636f 6e64 613a 0a0a 2020 2020 2020  m conda:..      
-00001d80: 2020 636f 6e64 6120 6372 6561 7465 202d    conda create -
-00001d90: 6320 6269 6f63 6f6e 6461 202d 6320 636f  c bioconda -c co
-00001da0: 6e64 612d 666f 7267 6520 2d6e 206c 6f63  nda-forge -n loc
-00001db0: 6964 6578 206c 6f63 6964 6578 0a0a 496e  idex locidex..In
-00001dc0: 7374 616c 6c20 7573 696e 6720 7069 703a  stall using pip:
-00001dd0: 0a0a 2020 2020 2020 2020 7069 7020 696e  ..        pip in
-00001de0: 7374 616c 6c20 6c6f 6369 6465 780a 0a49  stall locidex..I
-00001df0: 6e73 7461 6c6c 2074 6865 206c 6174 6573  nstall the lates
-00001e00: 7420 6d61 7374 6572 2062 7261 6e63 6820  t master branch 
-00001e10: 7665 7273 696f 6e20 6469 7265 6374 6c79  version directly
-00001e20: 2066 726f 6d20 4769 7468 7562 3a0a 0a20   from Github:.. 
-00001e30: 2020 2020 2020 2070 6970 2069 6e73 7461         pip insta
-00001e40: 6c6c 2067 6974 2b68 7474 7073 3a2f 2f67  ll git+https://g
-00001e50: 6974 6875 622e 636f 6d2f 7068 6163 2d6e  ithub.com/phac-n
-00001e60: 6d6c 2f6c 6f63 6964 6578 2e67 6974 0a0a  ml/locidex.git..
-00001e70: 0a0a 2323 2055 7361 6765 0a49 6620 796f  ..## Usage.If yo
-00001e80: 7520 7275 6e20 6060 6c6f 6369 6465 7860  u run ``locidex`
-00001e90: 602c 2079 6f75 2073 686f 756c 6420 7365  `, you should se
-00001ea0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-00001eb0: 7573 6167 6520 7374 6174 656d 656e 743a  usage statement:
-00001ec0: 0a0a 2020 2020 5573 6167 653a 206c 6f63  ..    Usage: loc
-00001ed0: 6964 6578 203c 636f 6d6d 616e 643e 205b  idex <command> [
-00001ee0: 6f70 7469 6f6e 735d 203c 7265 7175 6972  options] <requir
-00001ef0: 6564 2061 7267 756d 656e 7473 3e0a 2020  ed arguments>.  
-00001f00: 2020 0a20 2020 2054 6f20 6765 7420 6d69    .    To get mi
-00001f10: 6e69 6d61 6c20 7573 6167 6520 666f 7220  nimal usage for 
-00001f20: 6120 636f 6d6d 616e 6420 7573 653a 0a20  a command use:. 
-00001f30: 2020 2067 6173 2063 6f6d 6d61 6e64 0a20     gas command. 
-00001f40: 2020 200a 2020 2020 546f 2067 6574 2066     .    To get f
-00001f50: 756c 6c20 6865 6c70 2066 6f72 2061 2063  ull help for a c
-00001f60: 6f6d 6d61 6e64 2075 7365 206f 6e65 206f  ommand use one o
-00001f70: 663a 0a20 2020 206c 6f63 6964 6578 2063  f:.    locidex c
-00001f80: 6f6d 6d61 6e64 202d 680a 2020 2020 6c6f  ommand -h.    lo
-00001f90: 6369 6465 7820 636f 6d6d 616e 6420 2d2d  cidex command --
-00001fa0: 6865 6c70 0a20 2020 200a 2020 2020 0a20  help.    .    . 
-00001fb0: 2020 2041 7661 696c 6162 6c65 2063 6f6d     Available com
-00001fc0: 6d61 6e64 733a 0a20 2020 200a 2020 2020  mands:.    .    
-00001fd0: 7365 6172 6368 2020 5175 6572 7920 7365  search  Query se
-00001fe0: 7420 6f66 204f 5246 732c 2047 656e 6573  t of ORFs, Genes
-00001ff0: 2061 6761 696e 7374 2061 2064 6174 6162   against a datab
-00002000: 6173 6520 746f 2070 726f 6475 6365 2061  ase to produce a
-00002010: 2073 6571 7565 6e63 6520 7374 6f72 6520   sequence store 
-00002020: 666f 7220 646f 776e 7374 7265 616d 2070  for downstream p
-00002030: 726f 6365 7373 696e 670a 2020 2020 7265  rocessing.    re
-00002040: 706f 7274 2020 4669 6c74 6572 2061 2073  port  Filter a s
-00002050: 6571 7565 6e63 6520 7374 6f72 6520 616e  equence store an
-00002060: 6420 7072 6f64 7563 6520 616e 6420 6578  d produce and ex
-00002070: 7472 6163 7420 6f66 2062 6c61 7374 2072  tract of blast r
-00002080: 6573 756c 7473 2061 6e64 2067 656e 6520  esults and gene 
-00002090: 7072 6f66 696c 6520 2861 6c6c 656c 6520  profile (allele 
-000020a0: 6361 6c6c 696e 6729 0a20 2020 206d 6572  calling).    mer
-000020b0: 6765 2020 204d 6572 6765 2061 2073 6574  ge   Merge a set
-000020c0: 206f 6620 6765 6e65 2070 726f 6669 6c65   of gene profile
-000020d0: 7320 696e 746f 2061 2073 7461 6e64 6172  s into a standar
-000020e0: 6420 2261 6c6c 656c 6522 2070 726f 6669  d "allele" profi
-000020f0: 6c65 2066 6f72 6d61 7420 0a20 2020 2066  le format .    f
-00002100: 6f72 6d61 7420 2046 6f72 6d61 7420 6661  ormat  Format fa
-00002110: 7374 6120 6669 6c65 7320 6672 6f6d 206f  sta files from o
-00002120: 7468 6572 204d 4c53 5420 6461 7461 6261  ther MLST databa
-00002130: 7365 7320 666f 7220 7573 6520 7769 7468  ses for use with
-00002140: 206c 6f63 6964 6578 2062 7569 6c64 0a20   locidex build. 
-00002150: 2020 2062 7569 6c64 2020 2042 7569 6c64     build   Build
-00002160: 7320 6c6f 6369 6465 7820 6462 200a 0a0a  s locidex db ...
-00002170: 576f 726b 666c 6f77 730a 3d3d 3d3d 3d0a  Workflows.=====.
-00002180: 215b 616c 7420 7465 7874 5d28 6874 7470  ![alt text](http
-00002190: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000021a0: 6861 632d 6e6d 6c2f 6c6f 6369 6465 782f  hac-nml/locidex/
-000021b0: 626c 6f62 2f6d 6169 6e2f 4c6f 6369 6465  blob/main/Locide
-000021c0: 7857 6f72 6b66 6c6f 7773 2e70 6e67 3f72  xWorkflows.png?r
-000021d0: 6177 3d74 7275 6529 0a0a 4c6f 6369 6465  aw=true)..Locide
-000021e0: 7820 6973 2064 6573 6967 6e65 6420 746f  x is designed to
-000021f0: 2062 6520 7665 7279 206d 6f64 756c 6172   be very modular
-00002200: 2073 6f20 7468 6174 2064 6576 656c 6f70   so that develop
-00002210: 6572 7320 616e 6420 7573 6572 7320 6361  ers and users ca
-00002220: 6e20 6d69 7820 616e 6420 6d61 7463 6820  n mix and match 
-00002230: 6469 6666 6572 656e 7420 636f 6d70 6f6e  different compon
-00002240: 656e 7473 2066 6f72 2074 6865 6972 2069  ents for their i
-00002250: 6e64 6976 6964 7561 6c20 676f 616c 732e  ndividual goals.
-00002260: 0a45 6163 6820 746f 6f6c 2069 7320 6465  .Each tool is de
-00002270: 7369 676e 6564 2073 6f20 7468 6174 2069  signed so that i
-00002280: 7420 6361 6e20 6265 2069 6d70 6f72 7465  t can be importe
-00002290: 6420 6173 2061 2070 7974 686f 6e20 6c69  d as a python li
-000022a0: 6272 6172 7920 746f 2065 7874 656e 6420  brary to extend 
-000022b0: 616e 6420 696d 706c 656d 656e 7420 6375  and implement cu
-000022c0: 7374 6f6d 2062 6568 6176 696f 7572 2e20  stom behaviour. 
-000022d0: 4120 6465 7363 7269 7074 696f 6e20 6f66  A description of
-000022e0: 2065 6163 6820 746f 6f6c 2061 6e64 200a   each tool and .
-000022f0: 6974 7320 696e 7075 7473 2f6f 7574 7075  its inputs/outpu
-00002300: 7473 2069 7320 7072 6f76 6964 6564 2062  ts is provided b
-00002310: 656c 6f77 2e0a 0a2a 2a53 6561 7263 682a  elow...**Search*
-00002320: 2a0a 0a54 6865 2073 6561 7263 6820 6d6f  *..The search mo
-00002330: 6475 6c65 2069 7320 6d65 616e 7420 746f  dule is meant to
-00002340: 2075 7365 206c 6f63 6964 6578 2066 6f72   use locidex for
-00002350: 6d61 7465 6420 6461 7462 6173 6520 6469  mated datbase di
-00002360: 7265 6374 6f72 6965 730a 496e 7075 7420  rectories.Input 
-00002370: 4461 7461 2046 6f72 6d61 7473 3a20 4765  Data Formats: Ge
-00002380: 6e42 616e 6b2c 2046 6173 7461 2028 6f66  nBank, Fasta (of
-00002390: 2069 6e64 6976 6964 7561 6c20 6c6f 6369   individual loci
-000023a0: 2073 6571 7565 6e63 6573 290a 2d20 444e   sequences).- DN
-000023b0: 4120 616e 6420 7072 6f74 6569 6e20 626c  A and protein bl
-000023c0: 6173 7420 7365 6172 6368 6573 0a2d 204d  ast searches.- M
-000023d0: 6435 2068 6173 6869 6e67 206f 6620 616c  d5 hashing of al
-000023e0: 6c65 6c65 7320 0a2d 2053 746f 7261 6765  leles .- Storage
-000023f0: 206f 6620 7265 7375 6c74 7320 666f 7220   of results for 
-00002400: 706f 7374 2d70 726f 6365 7373 696e 6720  post-processing 
-00002410: 696e 206a 736f 6e20 666f 726d 6174 0a0a  in json format..
-00002420: 4765 6e65 2061 6e6e 6f74 6174 696f 6e20  Gene annotation 
-00002430: 6973 206e 6f74 6f72 696f 7573 6c79 2069  is notoriously i
-00002440: 6e63 6f6e 7369 7374 656e 7420 6265 7477  nconsistent betw
-00002450: 6565 6e20 6469 6666 6572 656e 7420 736f  een different so
-00002460: 6674 7761 7265 2061 6e64 2073 6f20 6974  ftware and so it
-00002470: 2069 7320 2a2a 5354 524f 4e47 4c59 2a2a   is **STRONGLY**
-00002480: 2072 6563 6f6d 6d65 6e64 6564 2074 6f20   recommended to 
-00002490: 7573 6520 7468 6520 7361 6d65 206d 6574  use the same met
-000024a0: 686f 640a 666f 7220 616e 6e6f 7461 7469  hod.for annotati
-000024b0: 6f6e 206f 6620 796f 7572 2064 6174 6162  on of your datab
-000024c0: 6173 6520 616e 6420 7768 6174 2079 6f75  ase and what you
-000024d0: 2077 696c 6c20 7573 6520 746f 2073 6561   will use to sea
-000024e0: 7263 682e 2069 652e 2069 6620 7573 696e  rch. ie. if usin
-000024f0: 6720 7072 6f64 6967 616c 2066 6f72 2073  g prodigal for s
-00002500: 6561 7263 6869 6e67 2c20 7573 6520 7072  earching, use pr
-00002510: 6f64 6967 616c 2066 6f72 2063 6f6e 7374  odigal for const
-00002520: 7275 6374 696e 6720 7468 6520 6461 7461  ructing the data
-00002530: 6261 7365 2e0a 0a20 0a0a 2020 2020 6c6f  base... ..    lo
-00002540: 6369 6465 7820 7365 6172 6368 202d 7120  cidex search -q 
-00002550: 2e2f 6578 616d 706c 652f 7365 6172 6368  ./example/search
-00002560: 2f4e 435f 3030 3331 3938 2e31 2e66 6173  /NC_003198.1.fas
-00002570: 7461 202d 6420 2e65 7861 6d70 6c65 2f62  ta -d .example/b
-00002580: 7569 6c64 5f64 625f 6d6c 7374 5f6f 7574  uild_db_mlst_out
-00002590: 202d 6f20 2e2f 6578 616d 706c 652f 7365   -o ./example/se
-000025a0: 6172 6368 2f4e 435f 3030 3331 3938 5f66  arch/NC_003198_f
-000025b0: 6173 7461 202d 6e20 3820 2d2d 616e 6e6f  asta -n 8 --anno
-000025c0: 7461 7465 0a20 2020 200a 2d72 756e 2069  tate.    .-run i
-000025d0: 6e20 616e 6e6f 7461 7469 6f6e 206d 6f64  n annotation mod
-000025e0: 6520 7769 7468 2061 2066 6173 7461 2069  e with a fasta i
-000025f0: 6e70 7574 0a0a 0a20 2020 206c 6f63 6964  nput...    locid
-00002600: 6578 2073 6561 7263 6820 2d71 202e 2f65  ex search -q ./e
-00002610: 7861 6d70 6c65 2f73 6561 7263 682f 4e43  xample/search/NC
-00002620: 5f30 3033 3139 382e 312e 6762 6b20 2d64  _003198.1.gbk -d
-00002630: 202e 6578 616d 706c 652f 6275 696c 645f   .example/build_
-00002640: 6462 5f6d 6c73 745f 6f75 7420 2d6f 202e  db_mlst_out -o .
-00002650: 2f65 7861 6d70 6c65 2f73 6561 7263 682f  /example/search/
-00002660: 4e43 5f30 3033 3139 385f 6661 7374 6120  NC_003198_fasta 
-00002670: 2d6e 2038 0a0a 2d72 756e 2077 6974 6820  -n 8..-run with 
-00002680: 6578 6973 7469 6e67 2061 6e6e 6f74 6174  existing annotat
-00002690: 696f 6e73 2069 6e20 4765 6e42 616e 6b20  ions in GenBank 
-000026a0: 666f 726d 6174 0a0a 2a2a 4f75 7470 7574  format..**Output
-000026b0: 2a2a 3a0a 6060 600a 7b6f 7574 2066 6f6c  **:.```.{out fol
-000026c0: 6465 7220 6e61 6d65 7d0a e294 9ce2 9480  der name}.......
-000026d0: e294 8020 626c 6173 740a 2020 e294 9ce2  ... blast.  ....
-000026e0: 9480 e294 8020 6e75 636c 656f 7469 6465  ..... nucleotide
-000026f0: 0a20 2020 20e2 949c e294 80e2 9480 2068  .    ......... h
-00002700: 7370 732e 7478 7420 2020 2020 2020 200a  sps.txt        .
-00002710: 2020 2020 e294 94e2 9480 e294 8020 7175      ......... qu
-00002720: 6572 6965 732e 6661 7374 610a 2020 e294  eries.fasta.  ..
-00002730: 9ce2 9480 e294 8020 7072 6f74 6569 6e0a  ....... protein.
-00002740: 2020 2020 e294 9ce2 9480 e294 8020 6873      ......... hs
-00002750: 7073 2e74 7874 2020 2020 2020 2020 0a20  ps.txt        . 
-00002760: 2020 20e2 9494 e294 80e2 9480 2071 7565     ......... que
-00002770: 7269 6573 2e66 6173 7461 2020 2020 2020  ries.fasta      
-00002780: 0ae2 949c e294 80e2 9480 2073 6571 5f73  .......... seq_s
-00002790: 746f 7265 2e6a 736f 6e0a e294 94e2 9480  tore.json.......
-000027a0: e294 8020 7265 7375 6c74 732e 6a73 6f6e  ... results.json
-000027b0: 2020 0a60 6060 0a53 6565 2022 5365 7175    .```.See "Sequ
-000027c0: 656e 6365 2053 746f 7265 2220 666f 7220  ence Store" for 
-000027d0: 6465 7363 7269 7074 696f 6e20 6f66 2074  description of t
-000027e0: 6865 2073 6571 5f73 746f 7265 2e6a 736f  he seq_store.jso
-000027f0: 6e20 6f75 7470 7574 2066 696c 650a 0a2a  n output file..*
-00002800: 2a52 6570 6f72 742a 2a0a 0a50 726f 6475  *Report**..Produ
-00002810: 6365 206c 6f63 6920 6861 7368 2070 726f  ce loci hash pro
-00002820: 6669 6c65 7320 696e 206d 756c 7469 706c  files in multipl
-00002830: 6520 666f 726d 6174 7320 286a 736f 6e2c  e formats (json,
-00002840: 2074 7376 2c20 7061 7271 7565 7429 0a2d   tsv, parquet).-
-00002850: 2046 696c 7465 7220 7265 7375 6c74 7320   Filter results 
-00002860: 6261 7365 6420 6f6e 2075 7365 7220 6372  based on user cr
-00002870: 6974 6572 6961 0a2d 204d 756c 7469 2d63  iteria.- Multi-c
-00002880: 6f70 7920 6c6f 6369 2068 616e 646c 696e  opy loci handlin
-00002890: 670a 0a0a 2020 2020 6c6f 6369 6465 7820  g...    locidex 
-000028a0: 7265 706f 7274 202d 6920 2e65 7861 6d70  report -i .examp
-000028b0: 6c65 2f73 6561 7263 682f 7365 715f 7374  le/search/seq_st
-000028c0: 6f72 652e 6a73 6f6e 202d 6f20 2e2f 6578  ore.json -o ./ex
-000028d0: 616d 706c 652f 7265 706f 7274 5f6f 7574  ample/report_out
-000028e0: 202d 2d6e 616d 6520 4e43 5f30 3033 3139   --name NC_00319
-000028f0: 380a 0a0a 0a4f 7074 696f 6e61 6c3a 2028  8....Optional: (
-00002900: 4e6f 7420 7265 7175 6972 6564 2066 6f72  Not required for
-00002910: 204d 5650 290a 5072 6f64 7563 6520 636f   MVP).Produce co
-00002920: 6e63 6174 656e 6174 6573 2066 6173 7461  ncatenates fasta
-00002930: 2073 6571 7565 6e63 6573 2062 6173 6564   sequences based
-00002940: 206f 6e20 616c 6c65 6c65 2070 726f 6669   on allele profi
-00002950: 6c65 730a 0a2a 2a4d 6572 6765 2a2a 0a0a  les..**Merge**..
-00002960: 4163 6365 7074 7320 6c69 7374 206f 6620  Accepts list of 
-00002970: 7265 706f 7274 2066 696c 6573 206f 6e20  report files on 
-00002980: 636f 6d6d 616e 6420 6c69 6e65 206f 7220  command line or 
-00002990: 6669 6c65 206f 6620 6669 6c65 7320 616e  file of files an
-000029a0: 6420 7265 6164 7320 616e 6420 636f 6e63  d reads and conc
-000029b0: 6174 656e 6174 6573 2074 6865 2066 696c  atenates the fil
-000029c0: 6573 2069 6e74 6f20 616e 2061 6c6c 656c  es into an allel
-000029d0: 6520 7072 6f66 696c 6520 696e 2054 5356  e profile in TSV
-000029e0: 2066 6f72 6d61 7420 2872 6561 6473 2067   format (reads g
-000029f0: 7a20 616e 6420 756e 636f 6d70 7265 7373  z and uncompress
-00002a00: 6564 2069 6e70 7574 7329 2e0a 0a20 2020  ed inputs)...   
-00002a10: 2020 2020 206c 6f63 6964 6578 206d 6572       locidex mer
-00002a20: 6765 202d 6920 2e2f 6578 616d 706c 652f  ge -i ./example/
-00002a30: 6d65 7267 655f 696e 2f70 726f 6669 6c65  merge_in/profile
-00002a40: 5f31 2e6a 736f 6e20 2e2f 6578 616d 706c  _1.json ./exampl
-00002a50: 652f 6d65 7267 655f 696e 2f70 726f 6669  e/merge_in/profi
-00002a60: 6c65 5f32 2e6a 736f 6e20 202d 6f20 2e2f  le_2.json  -o ./
-00002a70: 6578 616d 706c 652f 6d65 7267 655f 6f75  example/merge_ou
-00002a80: 742f 0a20 2020 2020 2020 200a 2d20 6d65  t/.        .- me
-00002a90: 7267 696e 6720 6d75 6c74 6970 6c65 2066  rging multiple f
-00002aa0: 696c 6573 2070 726f 7669 6465 6420 6f6e  iles provided on
-00002ab0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00002ac0: 6520 746f 202d 690a 0a0a 2020 2020 2020  e to -i...      
-00002ad0: 2020 6c6f 6369 6465 7820 6d65 7267 6520    locidex merge 
-00002ae0: 2d69 202e 2f65 7861 6d70 6c65 2f6d 6572  -i ./example/mer
-00002af0: 6765 5f69 6e2f 6669 6c65 5f6c 6973 742e  ge_in/file_list.
-00002b00: 7478 7420 2e2f 6578 616d 706c 652f 6d65  txt ./example/me
-00002b10: 7267 655f 6f75 742f 200a 0a2d 206d 6572  rge_out/ ..- mer
-00002b20: 6769 6e67 2061 2066 696c 6520 7768 6963  ging a file whic
-00002b30: 6820 6973 2061 206c 6973 7420 6f66 2070  h is a list of p
-00002b40: 6174 6873 2074 6f20 7265 706f 7274 2066  aths to report f
-00002b50: 696c 6573 0a0a 6060 600a 7b6f 7574 2066  iles..```.{out f
-00002b60: 6f6c 6465 7220 6e61 6d65 7d0a e294 9ce2  older name}.....
-00002b70: 9480 e294 8020 7072 6f66 696c 652e 7473  ..... profile.ts
-00002b80: 7620 2020 0ae2 9494 e294 80e2 9480 2072  v   .......... r
-00002b90: 6573 756c 7473 2e6a 736f 6e20 200a 6060  esults.json  .``
-00002ba0: 600a 0a2a 2a46 6f72 6d61 742a 2a0a 0a54  `..**Format**..T
-00002bb0: 616b 6573 2063 6f6d 6d6f 6e20 666f 726d  akes common form
-00002bc0: 6174 7320 6f66 2067 656e 652d 6279 2d67  ats of gene-by-g
-00002bd0: 656e 6520 6461 7461 6261 7365 7320 616e  ene databases an
-00002be0: 6420 666f 726d 6174 7320 7468 656d 2066  d formats them f
-00002bf0: 6f72 2075 7365 2077 6974 6820 6c6f 6369  or use with loci
-00002c00: 6465 7820 6275 696c 6420 6d6f 6475 6c65  dex build module
-00002c10: 2e20 4974 2061 6363 6570 7473 2061 2064  . It accepts a d
-00002c20: 6972 6563 746f 7279 206f 6620 0a66 6173  irectory of .fas
-00002c30: 7461 2066 696c 6573 3a20 5b22 6661 7374  ta files: ["fast
-00002c40: 6122 2c22 6661 7322 2c22 6661 222c 2266  a","fas","fa","f
-00002c50: 666e 222c 2266 6e61 222c 2266 6173 7461  fn","fna","fasta
-00002c60: 2e67 7a22 2c22 6661 732e 677a 222c 2266  .gz","fas.gz","f
-00002c70: 612e 677a 222c 2266 666e 2e67 7a22 2c22  a.gz","ffn.gz","
-00002c80: 666e 612e 677a 225d 2077 6869 6368 2068  fna.gz"] which h
-00002c90: 6176 6520 7468 6520 6c6f 6375 7320 6e61  ave the locus na
-00002ca0: 6d65 206f 6620 0a61 7320 7468 6520 6669  me of .as the fi
-00002cb0: 6c65 206e 616d 6520 616e 6420 616c 6c65  le name and alle
-00002cc0: 6c65 2069 6427 7320 6172 6520 7072 6573  le id's are pres
-00002cd0: 656e 7420 696e 2074 6865 2066 6173 7461  ent in the fasta
-00002ce0: 2068 6561 6465 7220 7365 7061 7261 7465   header separate
-00002cf0: 6420 6279 2061 6e20 756e 6465 7273 636f  d by an undersco
-00002d00: 7265 2e20 6965 2e20 6172 6f43 2077 6f75  re. ie. aroC wou
-00002d10: 6c64 2068 6176 6520 7468 650a 6669 6c65  ld have the.file
-00002d20: 206e 616d 6520 6172 6f43 2e66 6173 2061   name aroC.fas a
-00002d30: 6e64 2074 6865 2068 6561 6465 7220 6c69  nd the header li
-00002d40: 6e65 2077 6f75 6c64 2062 6520 3e61 726f  ne would be >aro
-00002d50: 435f 312e 2041 6464 6974 696f 6e61 6c6c  C_1. Additionall
-00002d60: 792c 2066 6f72 6d61 7420 7769 6c6c 2061  y, format will a
-00002d70: 6363 6570 7420 6120 636f 6e63 6174 6f6e  ccept a concaton
-00002d80: 6174 6564 2066 696c 6520 6f66 2061 6c6c  ated file of all
-00002d90: 200a 6c6f 6369 2069 6e20 6120 2073 696e   .loci in a  sin
-00002da0: 676c 6520 6661 7374 6120 6669 6c65 2077  gle fasta file w
-00002db0: 6869 6368 2068 6173 2074 6865 2066 6173  hich has the fas
-00002dc0: 7461 2064 6566 206c 696e 6520 6173 203e  ta def line as >
-00002dd0: 7b6c 6f63 7573 206e 616d 657d 5f7b 616c  {locus name}_{al
-00002de0: 6c65 6c65 2069 647d 2e20 5468 6573 6520  lele id}. These 
-00002df0: 7477 6f20 666f 726d 6174 7320 6172 6520  two formats are 
-00002e00: 636f 6d6d 6f6e 2077 6974 680a 6d6f 7374  common with.most
-00002e10: 206f 6620 7468 6520 6d61 6a6f 7220 4d4c   of the major ML
-00002e20: 5354 2064 6174 6162 6173 6573 2e0a 0a20  ST databases... 
-00002e30: 2020 2020 2020 206c 6f63 6964 6578 2066         locidex f
-00002e40: 6f72 6d61 7420 2d69 202e 2f65 7861 6d70  ormat -i ./examp
-00002e50: 6c65 2f66 6f72 6d61 745f 6462 5f6d 6c73  le/format_db_mls
-00002e60: 745f 696e 2f20 2d6f 202e 2f65 7861 6d70  t_in/ -o ./examp
-00002e70: 6c65 2f6d 6c73 745f 6f75 742f 200a 0a2a  le/mlst_out/ ..*
-00002e80: 2a4f 7574 7075 742a 2a3a 0a60 6060 0a7b  *Output**:.```.{
-00002e90: 6f75 7420 666f 6c64 6572 206e 616d 657d  out folder name}
-00002ea0: 0ae2 949c e294 80e2 9480 2072 6573 756c  .......... resul
-00002eb0: 7473 2e6a 736f 6e20 2020 2020 2020 2020  ts.json         
-00002ec0: 2020 2020 2020 2020 2020 200a e294 94e2             .....
-00002ed0: 9480 e294 8020 6c6f 6369 6465 782e 7478  ..... locidex.tx
-00002ee0: 740a 6060 600a 0a0a 0a2a 2a42 7569 6c64  t.```....**Build
-00002ef0: 2a2a 0a0a 4275 696c 6473 206c 6f63 6964  **..Builds locid
-00002f00: 6578 2064 6220 666f 6c64 6572 2073 7472  ex db folder str
-00002f10: 7563 7475 7265 0a2d 2043 7265 6174 6573  ucture.- Creates
-00002f20: 2064 6174 6162 6173 6520 636f 6e66 6967   database config
-00002f30: 7572 6174 696f 6e20 6669 6c65 0a2d 2043  uration file.- C
-00002f40: 7265 6174 6573 206c 6f63 6920 6d65 7461  reates loci meta
-00002f50: 6461 7461 2066 696c 650a 2d20 436f 6e73  data file.- Cons
-00002f60: 7472 7563 7420 626c 6173 7420 6461 7461  truct blast data
-00002f70: 6261 7365 7320 286e 7563 6c65 6f74 6964  bases (nucleotid
-00002f80: 6520 616e 642f 6f72 2070 726f 7465 696e  e and/or protein
-00002f90: 290a 0a54 616b 6573 2074 6865 206f 7574  )..Takes the out
-00002fa0: 7075 7420 6f66 206c 6f63 6964 6578 2066  put of locidex f
-00002fb0: 6f72 6d61 7420 7768 6963 6820 6d61 7920  ormat which may 
-00002fc0: 6f72 206d 6179 206e 6f74 2068 6176 6520  or may not have 
-00002fd0: 6164 6469 7469 6f6e 616c 2063 6f6c 756d  additional colum
-00002fe0: 6e73 2061 6464 6564 2e20 5468 6572 6520  ns added. There 
-00002ff0: 6172 6520 7370 6563 6966 6963 2066 6965  are specific fie
-00003000: 6c64 7320 6265 696e 6720 6c6f 6f6b 6564  lds being looked
-00003010: 2066 6f72 200a 696e 2074 6865 2066 696c   for .in the fil
-00003020: 6520 7768 6963 6820 6569 7468 6572 206f  e which either o
-00003030: 7220 626f 7468 2061 7265 2072 6571 7569  r both are requi
-00003040: 7265 6420 6465 7065 6e64 696e 6720 6f6e  red depending on
-00003050: 2074 6865 2074 7970 6520 6f66 2064 6220   the type of db 
-00003060: 6265 696e 6720 6275 696c 7420 2264 6e61  being built "dna
-00003070: 5f73 6571 222c 2022 6161 5f73 6571 222e  _seq", "aa_seq".
-00003080: 2049 7420 6578 7472 6163 7473 2074 6865   It extracts the
-00003090: 2073 6571 7565 6e63 650a 6461 7461 2028   sequence.data (
-000030a0: 6e75 636c 656f 7469 6465 7c70 726f 7465  nucleotide|prote
-000030b0: 696e 2920 616e 6420 696e 6974 6961 6c69  in) and initiali
-000030c0: 7a65 7320 7468 6520 636f 6e66 6967 2e6a  zes the config.j
-000030d0: 736f 6e2c 206d 6574 612e 6a73 6f6e 2061  son, meta.json a
-000030e0: 6e64 2062 6c61 7374 2064 6220 7374 7275  nd blast db stru
-000030f0: 6374 7572 6520 7768 6963 6820 6c6f 6369  cture which loci
-00003100: 6465 7820 7365 6172 6368 2072 6571 7569  dex search requi
-00003110: 7265 732e 0a0a 2020 2020 2020 2020 6c6f  res...        lo
-00003120: 6369 6465 7820 6275 696c 6420 2d69 202e  cidex build -i .
-00003130: 2f65 7861 6d70 6c65 2f62 7569 6c64 5f64  /example/build_d
-00003140: 625f 6d6c 7374 5f69 6e2f 7365 6e74 6572  b_mlst_in/senter
-00003150: 6963 612e 6d6c 7374 2e74 7874 202d 6f20  ica.mlst.txt -o 
-00003160: 2e2f 6578 616d 706c 652f 6d6c 7374 5f6f  ./example/mlst_o
-00003170: 7574 5f64 622f 200a 0a2a 2a4f 7574 7075  ut_db/ ..**Outpu
-00003180: 742a 2a3a 0a0a 5365 6520 2d20 5b44 6174  t**:..See - [Dat
-00003190: 6162 6173 6520 7374 7275 6374 7572 655d  abase structure]
-000031a0: 2823 4461 7461 6261 7365 290a 0a0a 2323  (#Database)...##
-000031b0: 2044 6174 6162 6173 650a 0a53 696d 696c   Database..Simil
-000031c0: 6172 2074 6f20 205b 6162 7269 6361 7465  ar to  [abricate
-000031d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000031e0: 2e63 6f6d 2f74 7365 656d 616e 6e2f 6162  .com/tseemann/ab
-000031f0: 7269 6361 7465 292c 204c 6f63 6964 6578  ricate), Locidex
-00003200: 2075 7365 7320 6120 6669 7865 6420 6461   uses a fixed da
-00003210: 7461 6261 7365 2073 7472 7563 7475 7265  tabase structure
-00003220: 206c 6179 6f75 742e 204c 6f63 6964 6578   layout. Locidex
-00003230: 2073 7570 706f 7274 730a 6e75 636c 656f   supports.nucleo
-00003240: 7469 6465 2028 626c 6173 746e 2920 616e  tide (blastn) an
-00003250: 6420 7072 6f74 6569 6e20 2862 6c61 7374  d protein (blast
-00003260: 7029 2062 6c61 7374 2073 6561 7263 6865  p) blast searche
-00003270: 732e 204c 6f63 6964 6578 2075 7469 6c69  s. Locidex utili
-00003280: 7a65 7320 6120 6665 7720 636f 6e74 726f  zes a few contro
-00003290: 6c6c 6564 2066 6965 6c64 7320 696e 2063  lled fields in c
-000032a0: 6f6e 6669 672e 6a73 6f6e 2061 6e64 206d  onfig.json and m
-000032b0: 6574 612e 6a73 6f6e 0a62 7574 2063 6f6d  eta.json.but com
-000032c0: 706c 6574 656c 7920 7375 7070 6f72 7473  pletely supports
-000032d0: 2074 6865 2061 6464 6974 6f6e 206f 6620   the additon of 
-000032e0: 616e 7920 6e75 6d62 6572 206f 6620 6164  any number of ad
-000032f0: 6469 7469 6f6e 616c 2066 6965 6c64 7320  ditional fields 
-00003300: 7468 6174 206d 6179 2062 6520 6465 7369  that may be desi
-00003310: 7265 6420 6279 2074 6865 2064 6174 6162  red by the datab
-00003320: 6173 6520 6275 696c 6465 722e 200a 5468  ase builder. .Th
-00003330: 6572 6520 6973 2061 206e 6573 7465 6420  ere is a nested 
-00003340: 666f 6c64 6572 2073 7472 7563 7475 7265  folder structure
-00003350: 2066 6f72 2074 6865 2062 6c61 7374 2064   for the blast d
-00003360: 6174 6162 6173 6573 2077 6869 6368 206d  atabases which m
-00003370: 7573 7420 636f 6e66 6f72 6d20 746f 2074  ust conform to t
-00003380: 6865 206c 6179 6f75 7420 6265 6c6f 772e  he layout below.
-00003390: 0a60 6060 0a7b 4442 2066 6f6c 6465 7220  .```.{DB folder 
-000033a0: 6e61 6d65 7d0a e294 9ce2 9480 e294 8020  name}.......... 
-000033b0: 636f 6e66 6967 2e6a 736f 6e20 2020 2020  config.json     
-000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033d0: 2372 6571 7569 7265 640a e294 9ce2 9480  #required.......
-000033e0: e294 8020 6d65 7461 2e6a 736f 6e20 2020  ... meta.json   
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 2372 6571 7569 7265 640a e294      #required...
-00003410: 94e2 9480 e294 8020 626c 6173 7420 2020  ....... blast   
-00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003430: 2020 2020 2020 2020 2372 6571 7569 7265          #require
-00003440: 640a 2020 2020 e294 94e2 9480 e294 8020  d.    ......... 
-00003450: 6e75 636c 656f 7469 6465 2020 2020 2020  nucleotide      
-00003460: 2020 2020 2020 2020 2020 2020 236f 7074              #opt
-00003470: 696f 6e61 6c20 6275 7420 3e3d 2031 6d75  ional but >= 1mu
-00003480: 7374 2062 6520 7072 6573 656e 740a 2020  st be present.  
-00003490: 2020 2020 2020 e294 9ce2 9480 e294 806e        .........n
-000034a0: 7563 6c65 6f74 6964 652e 6661 7374 610a  ucleotide.fasta.
-000034b0: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-000034c0: 806e 7563 6c65 6f74 6964 652e 6e64 620a  .nucleotide.ndb.
-000034d0: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-000034e0: 806e 7563 6c65 6f74 6964 652e 6e68 720a  .nucleotide.nhr.
-000034f0: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-00003500: 806e 7563 6c65 6f74 6964 652e 6e69 6e0a  .nucleotide.nin.
-00003510: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-00003520: 806e 7563 6c65 6f74 6964 652e 6e6a 730a  .nucleotide.njs.
-00003530: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-00003540: 806e 7563 6c65 6f74 6964 652e 6e73 710a  .nucleotide.nsq.
-00003550: 2020 2020 2020 2020 e294 9ce2 9480 e294          ........
-00003560: 806e 7563 6c65 6f74 6964 652e 6e74 660a  .nucleotide.ntf.
-00003570: 2020 2020 2020 2020 e294 94e2 9480 e294          ........
-00003580: 806e 7563 6c65 6f74 6964 652e 6e74 6f20  .nucleotide.nto 
-00003590: 0a20 2020 20e2 9494 e294 80e2 9480 7072  .    .........pr
-000035a0: 6f74 6569 6e20 2020 2020 2020 2020 2020  otein           
-000035b0: 2020 2020 2020 2020 2020 2023 6f70 7469             #opti
-000035c0: 6f6e 616c 2062 7574 203e 3d20 316d 7573  onal but >= 1mus
-000035d0: 7420 6265 2070 7265 7365 6e74 0a20 2020  t be present.   
-000035e0: 2020 2020 20e2 949c e294 80e2 9480 2070       ......... p
-000035f0: 726f 7465 696e 2e66 6173 7461 0a20 2020  rotein.fasta.   
-00003600: 2020 2020 20e2 949c e294 80e2 9480 2070       ......... p
-00003610: 726f 7465 696e 2e70 6462 0a20 2020 2020  rotein.pdb.     
-00003620: 2020 20e2 949c e294 80e2 9480 2070 726f     ......... pro
-00003630: 7465 696e 2e70 6872 0a20 2020 2020 2020  tein.phr.       
-00003640: 20e2 949c e294 80e2 9480 2070 726f 7465   ......... prote
-00003650: 696e 2e70 696e 0a20 2020 2020 2020 20e2  in.pin.        .
-00003660: 949c e294 80e2 9480 2070 726f 7465 696e  ........ protein
-00003670: 2e70 6a73 0a20 2020 2020 2020 20e2 949c  .pjs.        ...
-00003680: e294 80e2 9480 2070 726f 7465 696e 2e70  ...... protein.p
-00003690: 6f74 0a20 2020 2020 2020 20e2 949c e294  ot.        .....
-000036a0: 80e2 9480 2070 726f 7465 696e 2e70 7371  .... protein.psq
-000036b0: 0a20 2020 2020 2020 20e2 949c e294 80e2  .        .......
-000036c0: 9480 2070 726f 7465 696e 2e70 7466 0a20  .. protein.ptf. 
-000036d0: 2020 2020 2020 20e2 9494 e294 80e2 9480         .........
-000036e0: 7072 6f74 6569 6e2e 7074 6f0a 6060 600a  protein.pto.```.
-000036f0: 0a2a 2a63 6f6e 6669 672e 6a73 6f6e 2a2a  .**config.json**
-00003700: 0a0a 5468 6973 205b 4a53 4f4e 5d28 6874  ..This [JSON](ht
-00003710: 7470 733a 2f2f 7777 772e 6a73 6f6e 2e6f  tps://www.json.o
-00003720: 7267 2f6a 736f 6e2d 656e 2e68 746d 6c29  rg/json-en.html)
-00003730: 2066 696c 6520 6973 2072 6573 706f 6e73   file is respons
-00003740: 6962 6c65 2066 6f72 2065 6e63 6f64 696e  ible for encodin
-00003750: 6720 7468 6520 6d65 7461 6461 7461 2072  g the metadata r
-00003760: 6567 6172 6469 6e67 2074 6865 206c 6f63  egarding the loc
-00003770: 6964 6578 2064 6174 6162 6173 6520 7768  idex database wh
-00003780: 6963 6820 7769 6c6c 2062 6520 6275 6e64  ich will be bund
-00003790: 6c65 6420 696e 746f 2074 6865 2073 6571  led into the seq
-000037a0: 5f73 746f 7265 206f 7574 7075 740a 6f66  _store output.of
-000037b0: 2074 6865 2073 6561 7263 6820 6d6f 6475   the search modu
-000037c0: 6c65 2e20 4974 2061 6c73 6f20 6465 7465  le. It also dete
-000037d0: 726d 696e 6573 2077 6865 7468 6572 6520  rmines whethere 
-000037e0: 6120 6769 7665 6e20 6461 7461 6261 7365  a given database
-000037f0: 2069 7320 7573 6564 2066 6f72 206e 7563   is used for nuc
-00003800: 6c65 6f74 6964 6520 616e 642f 6f72 2070  leotide and/or p
-00003810: 726f 7465 696e 2062 6c61 7374 2073 6561  rotein blast sea
-00003820: 7263 6865 732e 0a54 6869 7320 6461 7461  rches..This data
-00003830: 2061 7373 6973 7473 2077 6974 6820 7072   assists with pr
-00003840: 6f76 656e 616e 6365 2069 6e66 6f72 6d61  ovenance informa
-00003850: 7469 6f6e 2072 6567 6172 6469 6e67 2073  tion regarding s
-00003860: 6561 7263 6820 7265 7375 6c74 732e 0a0a  earch results...
-00003870: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00003880: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00003890: 625f 6e61 6d65 223a 2022 5361 6c6d 6f6e  b_name": "Salmon
-000038a0: 656c 6c61 2043 6865 7762 6261 6361 2d4f  ella Chewbbaca-O
-000038b0: 6e6c 696e 6520 6367 4d4c 5354 222c 0a20  nline cgMLST",. 
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000038d0: 6462 5f76 6572 7369 6f6e 223a 2022 312e  db_version": "1.
-000038e0: 302e 3022 2c0a 2020 2020 2020 2020 2020  0.0",.          
-000038f0: 2020 2020 2020 2264 625f 6461 7465 223a        "db_date":
-00003900: 2022 3230 3234 2d30 322d 3031 222c 0a20   "2024-02-01",. 
-00003910: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003920: 6462 5f61 7574 686f 7222 3a20 224a 616d  db_author": "Jam
-00003930: 6573 2052 6f62 6572 7473 6f6e 222c 0a20  es Robertson",. 
-00003940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003950: 6462 5f64 6573 6322 3a20 2244 6174 6120  db_desc": "Data 
-00003960: 6f62 7461 696e 6564 2066 726f 6d3a 2068  obtained from: h
-00003970: 7474 7073 3a2f 2f63 6865 7762 6261 6361  ttps://chewbbaca
-00003980: 2e6f 6e6c 696e 652f 7370 6563 6965 732f  .online/species/
-00003990: 3822 2c0a 2020 2020 2020 2020 2020 2020  8",.            
-000039a0: 2020 2020 2264 625f 6e75 6d5f 7365 7173      "db_num_seqs
-000039b0: 223a 3835 3538 2c0a 2020 2020 2020 2020  ":8558,.        
-000039c0: 2020 2020 2020 2020 2269 735f 6e75 636c          "is_nucl
-000039d0: 223a 2022 5472 7565 222c 0a20 2020 2020  ": "True",.     
-000039e0: 2020 2020 2020 2020 2020 2022 6973 5f70             "is_p
-000039f0: 726f 7422 3a20 2254 7275 6522 2c0a 2020  rot": "True",.  
-00003a00: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00003a10: 7563 6c65 6f74 6964 655f 6462 5f6e 616d  ucleotide_db_nam
-00003a20: 6522 3a20 226e 7563 656c 6f74 6964 6522  e": "nucelotide"
-00003a30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003a40: 2020 2270 726f 7465 696e 5f64 625f 6e61    "protein_db_na
-00003a50: 6d65 223a 2022 7072 6f74 6569 6e22 0a20  me": "protein". 
-00003a60: 2020 2020 2020 2020 2020 207d 0a0a 0a2a             }...*
-00003a70: 2a6d 6574 612e 6a73 6f6e 2a2a 0a0a 4672  *meta.json**..Fr
-00003a80: 6571 7565 6e74 6c79 2c20 7468 6572 6520  equently, there 
-00003a90: 6973 2061 2064 6573 6972 6520 746f 2065  is a desire to e
-00003aa0: 6e63 6f64 6520 636f 6e74 6578 7475 616c  ncode contextual
-00003ab0: 206d 6574 6164 6174 6120 7769 7468 2073   metadata with s
-00003ac0: 6571 7565 6e63 6520 6461 7461 2066 6f72  equence data for
-00003ad0: 2064 6966 6665 7265 6e74 2061 6e61 6c79   different analy
-00003ae0: 7469 6361 6c20 6f70 6572 6174 696f 6e73  tical operations
-00003af0: 2e20 5468 6573 6520 6361 6e0a 7261 6e67  . These can.rang
-00003b00: 6520 6672 6f6d 2065 6e63 6f64 696e 6720  e from encoding 
-00003b10: 6765 6e65 2061 6e64 2061 6c6c 656c 6520  gene and allele 
-00003b20: 6964 656e 7469 6669 6572 7320 746f 2070  identifiers to p
-00003b30: 6865 6e6f 7479 7069 6320 6566 6665 6374  henotypic effect
-00003b40: 7320 616e 6420 6265 796f 6e64 2e20 5468  s and beyond. Th
-00003b50: 6520 6f70 7469 6f6e 7320 666f 7220 6465  e options for de
-00003b60: 7665 6c6f 7065 7273 2068 6173 2062 6565  velopers has bee
-00003b70: 6e20 746f 2065 6e63 6f64 6520 7468 6973  n to encode this
-00003b80: 2069 6e74 6f20 7468 6520 6661 7374 610a   into the fasta.
-00003b90: 6865 6164 6572 2064 6972 6563 7479 2077  header directy w
-00003ba0: 6974 6820 6469 6666 6572 656e 7420 6465  ith different de
-00003bb0: 6c69 6d65 7465 7273 2062 6574 7765 656e  limeters between
-00003bc0: 2066 6965 6c64 7320 6f72 2074 6f20 6861   fields or to ha
-00003bd0: 7665 2061 6e20 6164 6469 7469 6f6e 616c  ve an additional
-00003be0: 2066 696c 6520 7769 7468 2074 6865 2064   file with the d
-00003bf0: 6573 6972 6564 2063 6f6e 7465 7874 7561  esired contextua
-00003c00: 6c20 696e 666f 726d 6174 696f 6e20 7365  l information se
-00003c10: 7061 7261 7465 2066 726f 6d20 7468 6520  parate from the 
-00003c20: 7365 7175 656e 6365 2064 6174 612e 0a4c  sequence data..L
-00003c30: 6f63 6964 6578 2075 7469 6c69 7a65 7320  ocidex utilizes 
-00003c40: 7468 6520 6c61 7465 7220 6170 7072 6f61  the later approa
-00003c50: 6368 2077 6974 6820 616c 6c20 6f66 2074  ch with all of t
-00003c60: 6865 2064 6174 6120 656e 636f 6465 6420  he data encoded 
-00003c70: 696e 205b 4a53 4f4e 5d28 6874 7470 733a  in [JSON](https:
-00003c80: 2f2f 7777 772e 6a73 6f6e 2e6f 7267 2f6a  //www.json.org/j
-00003c90: 736f 6e2d 656e 2e68 746d 6c29 2066 6f72  son-en.html) for
-00003ca0: 2065 6173 7920 7061 7273 696e 6720 6279   easy parsing by
-00003cb0: 2064 6f77 6e73 7472 6561 6d20 6170 706c   downstream appl
-00003cc0: 6963 6174 696f 6e73 2e0a 5468 6973 2066  ications..This f
-00003cd0: 696c 6520 6973 2075 7365 6420 6279 2074  ile is used by t
-00003ce0: 6865 2073 6561 7263 6820 6d6f 6475 6c65  he search module
-00003cf0: 2074 6f20 6275 6e64 6c65 2074 6869 7320   to bundle this 
-00003d00: 636f 6e74 6578 7475 616c 2069 6e66 6f72  contextual infor
-00003d10: 6d61 7469 6f6e 2072 6567 6172 6469 6e67  mation regarding
-00003d20: 2074 6865 2064 6174 6162 6173 6520 7365   the database se
-00003d30: 7175 656e 6365 7320 666f 7220 6c61 7465  quences for late
-00003d40: 7220 7573 6520 7769 7468 6f75 7420 7468  r use without th
-00003d50: 6520 6e65 6564 2074 6f20 7061 7373 2074  e need to pass t
-00003d60: 6865 206f 7269 6769 6e61 6c0a 6d65 7461  he original.meta
-00003d70: 2e6a 736f 6e20 696e 666f 726d 6174 696f  .json informatio
-00003d80: 6e20 6265 7477 6565 6e20 7072 6f63 6573  n between proces
-00003d90: 7365 732e 2041 6e20 6578 616d 706c 6520  ses. An example 
-00003da0: 7374 7562 2069 7320 7368 6f77 6e20 6265  stub is shown be
-00003db0: 6c6f 7720 666f 7220 6d65 7461 6461 7461  low for metadata
-00003dc0: 2e20 616e 6420 616e 7920 6e75 6d62 6572  . and any number
-00003dd0: 206f 6620 6164 6469 7469 6f6e 616c 2066   of additional f
-00003de0: 6965 6c64 7320 6361 6e20 6265 2061 6464  ields can be add
-00003df0: 6564 2074 6f20 7265 636f 7264 732e 0a0a  ed to records...
-00003e00: 2020 2020 7b0a 2020 2020 2020 2020 2269      {.        "i
-00003e10: 6e66 6f22 3a20 7b0a 2020 2020 2020 2020  nfo": {.        
-00003e20: 2020 2020 226e 756d 5f73 6571 7322 3a20      "num_seqs": 
-00003e30: 3835 3538 2c0a 2020 2020 2020 2020 2020  8558,.          
-00003e40: 2020 2269 735f 6364 7322 3a20 2254 7275    "is_cds": "Tru
-00003e50: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00003e60: 2274 7261 6e73 5f74 6162 6c65 223a 2031  "trans_table": 1
-00003e70: 312c 0a20 2020 2020 2020 2020 2020 2022  1,.            "
-00003e80: 646e 615f 6d69 6e5f 6c65 6e22 3a20 3732  dna_min_len": 72
-00003e90: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-00003ea0: 6e61 5f6d 6178 5f6c 656e 223a 2031 3036  na_max_len": 106
-00003eb0: 3434 2c0a 2020 2020 2020 2020 2020 2020  44,.            
-00003ec0: 2264 6e61 5f6d 696e 5f69 6465 6e74 223a  "dna_min_ident":
-00003ed0: 2038 302c 0a20 2020 2020 2020 2020 2020   80,.           
-00003ee0: 2022 6161 5f6d 696e 5f6c 656e 223a 2032   "aa_min_len": 2
-00003ef0: 342c 0a20 2020 2020 2020 2020 2020 2022  4,.            "
-00003f00: 6161 5f6d 6178 5f6c 656e 223a 2033 3534  aa_max_len": 354
-00003f10: 382c 0a20 2020 2020 2020 2020 2020 2022  8,.            "
-00003f20: 6161 5f6d 696e 5f69 6465 6e74 223a 2038  aa_min_ident": 8
-00003f30: 300a 2020 2020 2020 2020 7d2c 0a20 2020  0.        },.   
-00003f40: 2020 2020 2022 6d65 7461 223a 207b 0a20       "meta": {. 
-00003f50: 2020 2020 2020 2020 2020 2022 3022 3a20             "0": 
-00003f60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003f70: 2020 226c 6f63 7573 5f6e 616d 6522 3a20    "locus_name": 
-00003f80: 2253 414c 5f43 474d 4c53 545f 3030 3030  "SAL_CGMLST_0000
-00003f90: 3030 3030 3122 2c0a 2020 2020 2020 2020  00001",.        
-00003fa0: 2020 2020 2020 2020 226c 6f63 7573 5f6e          "locus_n
-00003fb0: 616d 655f 616c 7422 3a20 2249 4e4e 5545  ame_alt": "INNUE
-00003fc0: 4e44 4f5f 6367 4d4c 5354 2d30 3030 3338  NDO_cgMLST-00038
-00003fd0: 3330 315f 3122 2c0a 2020 2020 2020 2020  301_1",.        
-00003fe0: 2020 2020 2020 2020 226c 6f63 7573 5f70          "locus_p
-00003ff0: 726f 6475 6374 223a 204e 614e 2c0a 2020  roduct": NaN,.  
-00004000: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00004010: 6f63 7573 5f64 6573 6372 6970 7469 6f6e  ocus_description
-00004020: 223a 204e 614e 2c0a 2020 2020 2020 2020  ": NaN,.        
-00004030: 2020 2020 2020 2020 226c 6f63 7573 5f75          "locus_u
-00004040: 6964 223a 204e 614e 2c0a 2020 2020 2020  id": NaN,.      
-00004050: 2020 2020 2020 2020 2020 2264 6e61 5f73            "dna_s
-00004060: 6571 5f6c 656e 223a 2031 3532 312c 0a20  eq_len": 1521,. 
-00004070: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004080: 646e 615f 7365 715f 6861 7368 223a 2022  dna_seq_hash": "
-00004090: 6331 3732 3430 3465 6333 3439 3437 6337  c172404ec34947c7
-000040a0: 6438 3566 3064 3365 3766 6133 6238 3038  d85f0d3e7fa3b808
-000040b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000040c0: 2020 2022 6161 5f73 6571 5f6c 656e 223a     "aa_seq_len":
-000040d0: 2035 3037 2c0a 2020 2020 2020 2020 2020   507,.          
-000040e0: 2020 2020 2020 2261 615f 7365 715f 6861        "aa_seq_ha
-000040f0: 7368 223a 2022 3861 3238 6163 6131 3262  sh": "8a28aca12b
-00004100: 6366 3136 3038 3536 3432 3434 6136 3838  cf1608564244a688
-00004110: 6537 3964 6236 222c 0a20 2020 2020 2020  e79db6",.       
-00004120: 2020 2020 2020 2020 2022 646e 615f 6d69           "dna_mi
-00004130: 6e5f 6c65 6e22 3a20 3132 3137 2c0a 2020  n_len": 1217,.  
-00004140: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00004150: 6e61 5f6d 6178 5f6c 656e 223a 2031 3832  na_max_len": 182
-00004160: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00004170: 2020 2022 6161 5f6d 696e 5f6c 656e 223a     "aa_min_len":
-00004180: 2034 3036 2c0a 2020 2020 2020 2020 2020   406,.          
-00004190: 2020 2020 2020 2261 615f 6d61 785f 6c65        "aa_max_le
-000041a0: 6e22 3a20 3630 382c 0a20 2020 2020 2020  n": 608,.       
-000041b0: 2020 2020 2020 2020 2022 646e 615f 6d69           "dna_mi
-000041c0: 6e5f 6964 656e 7422 3a20 3830 2c0a 2020  n_ident": 80,.  
-000041d0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-000041e0: 615f 6d69 6e5f 6964 656e 7422 3a20 3830  a_min_ident": 80
-000041f0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00004200: 2020 2020 2020 207d 0a20 2020 207d 0a0a         }.    }..
-00004210: 2a2a 626c 6173 7420 6461 7461 6261 7365  **blast database
-00004220: 732a 2a0a 0a54 6865 2062 6c61 7374 2066  s**..The blast f
-00004230: 6f6c 6465 7220 6d75 7374 2062 6520 7072  older must be pr
-00004240: 6573 656e 7420 666f 7220 6120 6c6f 6369  esent for a loci
-00004250: 6465 7820 6461 7461 6261 7365 2074 6f20  dex database to 
-00004260: 6265 2076 616c 6964 2077 6974 6820 6e75  be valid with nu
-00004270: 636c 656f 7469 6465 2061 6e64 2f6f 7220  cleotide and/or 
-00004280: 7072 6f74 6569 6e20 7375 6266 6f6c 6465  protein subfolde
-00004290: 7273 2070 7265 7365 6e74 2e20 0a46 6f72  rs present. .For
-000042a0: 2065 6163 6820 666f 6c64 6572 2070 7265   each folder pre
-000042b0: 7365 6e74 2069 7420 6d75 7374 2063 6f6e  sent it must con
-000042c0: 7461 696e 2074 6865 2066 6173 7461 2066  tain the fasta f
-000042d0: 696c 6520 7573 6564 2074 6f20 6765 6e65  ile used to gene
-000042e0: 7261 7465 2074 6865 2064 6174 6162 6173  rate the databas
-000042f0: 6520 286e 7563 6c65 6f74 6964 652e 6661  e (nucleotide.fa
-00004300: 7374 617c 7072 6f74 6569 6e2e 6661 7374  sta|protein.fast
-00004310: 6129 2061 6e64 0a61 2063 6f72 7265 7370  a) and.a corresp
-00004320: 6f6e 6469 6e67 2062 6c61 7374 2064 6174  onding blast dat
-00004330: 6162 6173 6520 7769 7468 2074 6865 2066  abase with the f
-00004340: 6f6c 6465 7220 6e61 6d65 2077 6974 686f  older name witho
-00004350: 7574 2022 2e66 6173 7461 2220 7072 6573  ut ".fasta" pres
-00004360: 656e 742e 2054 6865 2073 7472 7563 7475  ent. The structu
-00004370: 7265 2069 7320 6465 7369 676e 6564 2074  re is designed t
-00004380: 6f20 616c 6c6f 7720 666f 7220 7468 6520  o allow for the 
-00004390: 0a69 6e63 6c75 7369 6f6e 206f 6620 6f74  .inclusion of ot
-000043a0: 6865 7220 7365 7175 656e 6365 2073 696d  her sequence sim
-000043b0: 696c 6172 6974 7920 7365 6172 6368 2074  ilarity search t
-000043c0: 6f6f 6c73 2061 7420 6120 6c61 7465 7220  ools at a later 
-000043d0: 6461 7465 2077 6974 6820 6d69 6e69 6d61  date with minima
-000043e0: 6c20 6d6f 6469 6669 6361 7469 6f6e 732e  l modifications.
-000043f0: 2050 726f 7465 696e 2073 6561 7263 6869   Protein searchi
-00004400: 6e67 2076 6961 2048 4d4d 730a 616e 6420  ng via HMMs.and 
-00004410: 6f74 6865 7220 746f 6f6c 7320 7375 6368  other tools such
-00004420: 2061 7320 5b64 6961 6d6f 6e64 5d28 6874   as [diamond](ht
-00004430: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004440: 2f62 6275 6368 6669 6e6b 2f64 6961 6d6f  /bbuchfink/diamo
-00004450: 6e64 2920 6d61 7920 6265 2069 6e63 6c75  nd) may be inclu
-00004460: 6465 6420 696e 206c 6174 6572 2072 656c  ded in later rel
-00004470: 6561 7365 732e 0a0a 0a0a 5375 7070 6f72  eases.....Suppor
-00004480: 7465 6420 696e 7075 7420 666f 726d 6174  ted input format
-00004490: 730a 3d3d 3d3d 3d0a 2a2a 4765 6e42 616e  s.=====.**GenBan
-000044a0: 6b2a 2a0a 0a5b 4765 6e42 616e 6b20 666f  k**..[GenBank fo
-000044b0: 726d 6174 5d28 6874 7470 733a 2f2f 7777  rmat](https://ww
-000044c0: 772e 6e63 6269 2e6e 6c6d 2e6e 6968 2e67  w.ncbi.nlm.nih.g
-000044d0: 6f76 2f67 656e 6261 6e6b 2f73 616d 706c  ov/genbank/sampl
-000044e0: 6572 6563 6f72 642f 2920 6973 2061 2077  erecord/) is a w
-000044f0: 6964 656c 7920 7573 6564 2066 6f72 6d61  idely used forma
-00004500: 7420 666f 7220 7374 6f72 696e 6720 616e  t for storing an
-00004510: 6420 7368 6172 696e 6720 0a62 696f 6c6f  d sharing .biolo
-00004520: 6769 6361 6c20 7365 7175 656e 6365 2064  gical sequence d
-00004530: 6174 612c 2070 7269 6d61 7269 6c79 2044  ata, primarily D
-00004540: 4e41 2073 6571 7565 6e63 6573 2e20 4974  NA sequences. It
-00004550: 2077 6173 2064 6576 656c 6f70 6564 2062   was developed b
-00004560: 7920 7468 6520 4e61 7469 6f6e 616c 2043  y the National C
-00004570: 656e 7465 7220 666f 7220 4269 6f74 6563  enter for Biotec
-00004580: 686e 6f6c 6f67 7920 496e 666f 726d 6174  hnology Informat
-00004590: 696f 6e20 0a28 4e43 4249 292e 2047 656e  ion .(NCBI). Gen
-000045a0: 4261 6e6b 2066 6f72 6d61 7420 6669 6c65  Bank format file
-000045b0: 7320 7479 7069 6361 6c6c 7920 6861 7665  s typically have
-000045c0: 2061 202e 6762 206f 7220 2e67 626b 2065   a .gb or .gbk e
-000045d0: 7874 656e 7369 6f6e 2e20 5768 656e 2075  xtension. When u
-000045e0: 7369 6e67 2047 656e 4261 6e6b 2066 6f72  sing GenBank for
-000045f0: 6d61 7420 6173 2069 6e70 7574 2074 6f20  mat as input to 
-00004600: 6c6f 6369 6465 782c 2074 6865 0a74 7261  locidex, the.tra
-00004610: 6e73 6c61 7469 6f6e 7320 2869 6620 6170  nslations (if ap
-00004620: 706c 6963 6162 6c65 2920 6172 6520 7072  plicable) are pr
-00004630: 6f76 6964 6564 2062 7920 7468 6520 6669  ovided by the fi
-00004640: 6c65 2072 6174 6865 7220 7468 616e 2062  le rather than b
-00004650: 6569 6e67 2074 7261 6e73 6c61 7465 6420  eing translated 
-00004660: 6279 206c 6f63 6964 6578 2e20 5468 6973  by locidex. This
-00004670: 2066 6f72 6d61 7420 6973 2075 7365 6420   format is used 
-00004680: 6173 2069 6e70 7574 0a74 6f20 6c6f 6369  as input.to loci
-00004690: 6465 7820 7365 6172 6368 2e0a 0a54 6865  dex search...The
-000046a0: 2047 656e 4261 6e6b 2066 6f72 6d61 7420   GenBank format 
-000046b0: 636f 6e73 6973 7473 206f 6620 6d75 6c74  consists of mult
-000046c0: 6970 6c65 2063 6f6d 706f 6e65 7473 2062  iple componets b
-000046d0: 7574 2074 6865 2072 656c 6576 616e 7420  ut the relevant 
-000046e0: 6f6e 6573 2066 6f72 206c 6f63 6964 6578  ones for locidex
-000046f0: 2061 7265 3a0a 0a53 6571 7565 6e63 6520   are:..Sequence 
-00004700: 4461 7461 3a20 5468 6520 636f 6d70 6c65  Data: The comple
-00004710: 7465 206e 7563 6c65 6f74 6964 6520 7365  te nucleotide se
-00004720: 7175 656e 6365 2077 6869 6368 2068 6173  quence which has
-00004730: 2062 6565 6e20 616e 6e6f 7461 7465 642e   been annotated.
-00004740: 0a0a 4665 6174 7572 6573 3a20 416e 6e6f  ..Features: Anno
-00004750: 7461 7469 6f6e 7320 6465 7363 7269 6269  tations describi
-00004760: 6e67 2064 6966 6665 7265 6e74 2072 6567  ng different reg
-00004770: 696f 6e73 206f 7220 6665 6174 7572 6573  ions or features
-00004780: 206f 6620 7468 6520 7365 7175 656e 6365   of the sequence
-00004790: 2c20 7375 6368 2061 7320 636f 6469 6e67  , such as coding
-000047a0: 2073 6571 7565 6e63 6573 2028 4344 5329   sequences (CDS)
-000047b0: 2c20 0a72 6567 756c 6174 6f72 7920 656c  , .regulatory el
-000047c0: 656d 656e 7473 2c20 616e 6420 6f74 6865  ements, and othe
-000047d0: 7220 6675 6e63 7469 6f6e 616c 2065 6c65  r functional ele
-000047e0: 6d65 6e74 732e 2045 6163 6820 6665 6174  ments. Each feat
-000047f0: 7572 6520 6973 2064 6566 696e 6564 2062  ure is defined b
-00004800: 7920 6120 6c6f 6361 7469 6f6e 2028 7374  y a location (st
-00004810: 6172 7420 616e 6420 656e 6420 706f 7369  art and end posi
-00004820: 7469 6f6e 7329 200a 6f6e 2074 6865 2073  tions) .on the s
-00004830: 6571 7565 6e63 6520 616e 6420 6164 6469  equence and addi
-00004840: 7469 6f6e 616c 2071 7561 6c69 6669 6572  tional qualifier
-00004850: 7320 7072 6f76 6964 696e 6720 6465 7461  s providing deta
-00004860: 696c 7320 6162 6f75 7420 7468 6520 6665  ils about the fe
-00004870: 6174 7572 652e 0a0a 2a2a 4661 7374 612a  ature...**Fasta*
-00004880: 2a0a 0a5b 4641 5354 415d 2868 7474 7073  *..[FASTA](https
-00004890: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-000048a0: 6f72 672f 7769 6b69 2f46 4153 5441 5f66  org/wiki/FASTA_f
-000048b0: 6f72 6d61 7429 2066 6f72 6d61 7420 6973  ormat) format is
-000048c0: 2061 2073 696d 706c 6520 616e 6420 7769   a simple and wi
-000048d0: 6465 6c79 2075 7365 6420 7465 7874 2d62  dely used text-b
-000048e0: 6173 6564 2066 6f72 6d61 7420 666f 7220  ased format for 
-000048f0: 7265 7072 6573 656e 7469 6e67 2062 696f  representing bio
-00004900: 6c6f 6769 6361 6c20 7365 7175 656e 6365  logical sequence
-00004910: 732c 200a 7375 6368 2061 7320 444e 412c  s, .such as DNA,
-00004920: 2052 4e41 2c20 6f72 2070 726f 7465 696e   RNA, or protein
-00004930: 2073 6571 7565 6e63 6573 2e20 4974 2069   sequences. It i
-00004940: 7320 6e61 6d65 6420 6166 7465 7220 7468  s named after th
-00004950: 6520 4641 5354 4120 736f 6674 7761 7265  e FASTA software
-00004960: 2070 6163 6b61 6765 2c20 7768 6963 6820   package, which 
-00004970: 6669 7273 7420 696e 7472 6f64 7563 6564  first introduced
-00004980: 2074 6869 7320 666f 726d 6174 2e20 0a46   this format. .F
-00004990: 4153 5441 2066 696c 6573 2074 7970 6963  ASTA files typic
-000049a0: 616c 6c79 2068 6176 6520 6120 2e66 6173  ally have a .fas
-000049b0: 7461 206f 7220 2e66 6120 6578 7465 6e73  ta or .fa extens
-000049c0: 696f 6e2e 204c 6f63 6964 6578 2073 7570  ion. Locidex sup
-000049d0: 706f 7274 7320 626f 7468 206e 7563 6c65  ports both nucle
-000049e0: 6f74 6964 6520 616e 6420 7072 6f74 6569  otide and protei
-000049f0: 6e20 7365 7175 656e 6365 7320 6173 2069  n sequences as i
-00004a00: 6e70 7574 2062 7574 200a 6974 206d 7573  nput but .it mus
-00004a10: 7420 636f 6e73 6973 7420 6f66 2065 7874  t consist of ext
-00004a20: 7261 6374 6564 2043 4453 2c20 4f52 4673  racted CDS, ORFs
-00004a30: 2c20 4765 6e65 7320 7768 6963 6820 6172  , Genes which ar
-00004a40: 6520 746f 2062 6520 6861 7368 6564 2e20  e to be hashed. 
-00004a50: 596f 7520 6361 6e20 7072 6f76 6964 6520  You can provide 
-00004a60: 7468 6520 6578 7472 6163 7465 6420 6765  the extracted ge
-00004a70: 6e65 2073 6571 7565 6e63 6573 2066 726f  ne sequences fro
-00004a80: 6d20 6120 746f 6f6c 2073 7563 6820 6173  m a tool such as
-00004a90: 205b 7072 6f64 6967 616c 5d28 6874 7470   [prodigal](http
-00004aa0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-00004ab0: 7961 7474 7064 2f50 726f 6469 6761 6c29  yattpd/Prodigal)
-00004ac0: 2c20 5b70 726f 6b6b 615d 2868 7474 7073  , [prokka](https
-00004ad0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7473  ://github.com/ts
-00004ae0: 6565 6d61 6e6e 2f70 726f 6b6b 6129 2c20  eemann/prokka), 
-00004af0: 0a5b 6261 6b74 615d 2868 7474 7073 3a2f  .[bakta](https:/
-00004b00: 2f67 6974 6875 622e 636f 6d2f 6f73 6368  /github.com/osch
-00004b10: 7765 6e67 6572 732f 6261 6b74 6129 2061  wengers/bakta) a
-00004b20: 6e64 2061 6e20 6170 7072 6f70 7269 6174  nd an appropriat
-00004b30: 6520 7472 616e 736c 6174 696f 6e20 7461  e translation ta
-00004b40: 626c 6520 6966 2074 6865 2070 726f 7465  ble if the prote
-00004b50: 696e 2063 6f64 696e 6720 7365 7175 656e  in coding sequen
-00004b60: 6365 732e 200a 596f 7520 6361 6e20 7375  ces. .You can su
-00004b70: 7070 6c79 2063 6f6e 7469 6773 2062 7574  pply contigs but
-00004b80: 2075 6e6c 6573 7320 796f 7520 7370 6563   unless you spec
-00004b90: 6966 7920 2d2d 616e 6e6f 7461 7465 2028  ify --annotate (
-00004ba0: 6765 6e65 2061 6e6e 6f74 6174 696f 6e20  gene annotation 
-00004bb0: 7573 696e 6720 7079 726f 6469 6761 6c29  using pyrodigal)
-00004bc0: 206e 6f20 6578 7472 6163 7469 6f6e 2077   no extraction w
-00004bd0: 696c 6c20 6f63 6375 7220 616e 640a 7468  ill occur and.th
-00004be0: 6520 656e 7469 7265 2073 6571 7565 6e63  e entire sequenc
-00004bf0: 6520 7769 6c6c 2062 6520 7472 6561 7465  e will be treate
-00004c00: 6420 6173 2061 2073 696e 676c 6520 7175  d as a single qu
-00004c10: 6572 792e 2020 5468 6973 2066 6f72 6d61  ery.  This forma
-00004c20: 7420 6973 2063 616e 2062 6520 7573 6564  t is can be used
-00004c30: 2061 7320 696e 7075 7420 746f 206c 6f63   as input to loc
-00004c40: 6964 6578 2073 6561 7263 682e 0a0a 0a0a  idex search.....
-00004c50: 0a2a 2a53 6571 7565 6e63 6520 7374 6f72  .**Sequence stor
-00004c60: 652a 2a0a 0a54 6869 7320 6973 2061 206c  e**..This is a l
-00004c70: 6f63 6964 6578 2064 6566 696e 6564 2066  ocidex defined f
-00004c80: 696c 6574 7970 6520 7768 6963 6820 7573  iletype which us
-00004c90: 6573 205b 4a53 4f4e 5d28 6874 7470 733a  es [JSON](https:
-00004ca0: 2f2f 7777 772e 6a73 6f6e 2e6f 7267 2f6a  //www.json.org/j
-00004cb0: 736f 6e2d 656e 2e68 746d 6c29 2074 6f20  son-en.html) to 
-00004cc0: 7374 6f72 6520 696e 666f 726d 6174 696f  store informatio
-00004cd0: 6e20 6162 6f75 7420 7468 6520 0a71 7565  n about the .que
-00004ce0: 7279 2073 6571 7565 6e63 6573 2069 6e63  ry sequences inc
-00004cf0: 6c75 6469 6e67 2074 6865 6972 2068 6173  luding their has
-00004d00: 6820 7661 6c75 6573 2061 6c6f 6e67 2077  h values along w
-00004d10: 6974 6820 7468 6520 6d65 7461 6461 7461  ith the metadata
-00004d20: 2072 6567 6172 6469 6e67 2074 6865 2064   regarding the d
-00004d30: 6174 6162 6173 6520 7768 6963 6820 7761  atabase which wa
-00004d40: 7320 7175 6572 6965 6420 616e 6420 6974  s queried and it
-00004d50: 7320 0a73 6571 7565 6e63 6573 2028 7365  s .sequences (se
-00004d60: 715f 7374 6f72 652e 6a73 6f6e 292e 2054  q_store.json). T
-00004d70: 6869 7320 666f 726d 6174 2069 7320 7573  his format is us
-00004d80: 6564 2061 7320 696e 7075 7420 746f 206c  ed as input to l
-00004d90: 6f63 6964 6578 2072 6570 6f72 742e 0a0a  ocidex report...
-00004da0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00004db0: 2020 2764 625f 696e 666f 273a 207b 2064    'db_info': { d
-00004dc0: 6174 6162 6173 6520 636f 6e66 6967 7572  atabase configur
-00004dd0: 6174 696f 6e20 6669 6c65 2064 6174 617d  ation file data}
-00004de0: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
-00004df0: 625f 7365 715f 696e 666f 273a 207b 2064  b_seq_info': { d
-00004e00: 6174 6162 6173 6520 7365 7175 656e 6365  atabase sequence
-00004e10: 206d 6574 6164 6174 6120 7d2c 0a20 2020   metadata },.   
-00004e20: 2020 2020 2020 2020 2027 7175 6572 795f           'query_
-00004e30: 6461 7461 273a 207b 0a20 2020 2020 2020  data': {.       
-00004e40: 2020 2020 2020 2020 2027 7361 6d70 6c65           'sample
-00004e50: 5f6e 616d 6527 3a27 5573 6572 2073 7570  _name':'User sup
-00004e60: 706c 6965 6420 6f72 2071 7565 7279 2066  plied or query f
-00004e70: 696c 656e 616d 6527 2c0a 2020 2020 2020  ilename',.      
-00004e80: 2020 2020 2020 2020 2020 2771 7565 7279            'query
-00004e90: 5f73 6571 5f64 6174 6127 3a20 7b20 6861  _seq_data': { ha
-00004ea0: 7368 2076 616c 7565 7320 616e 6420 6578  sh values and ex
-00004eb0: 7472 6163 7465 6420 6461 7461 206f 6e20  tracted data on 
-00004ec0: 7175 6572 7920 7365 7175 656e 6365 737d  query sequences}
-00004ed0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004ee0: 2020 2771 7565 7279 5f68 6974 5f63 6f6c    'query_hit_col
-00004ef0: 756d 6e73 273a 205b 6e61 6d65 7320 6f66  umns': [names of
-00004f00: 2062 6c61 7374 2066 6965 6c64 7320 7573   blast fields us
-00004f10: 6564 2069 6e20 7365 6172 6368 5d2c 0a20  ed in search],. 
-00004f20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00004f30: 7175 6572 795f 6869 7473 273a 207b 2062  query_hits': { b
-00004f40: 6c61 7374 2068 6974 2064 6174 6120 696e  last hit data in
-00004f50: 6465 7865 6420 6279 2071 7565 7279 2073  dexed by query s
-00004f60: 6571 7565 6e63 6520 7d2c 0a20 2020 2020  equence },.     
-00004f70: 2020 2020 2020 2020 2020 2022 6c6f 6375             "locu
-00004f80: 735f 7072 6f66 696c 6522 3a7b 2061 7373  s_profile":{ ass
-00004f90: 6967 6e6d 656e 7420 6f66 2071 7565 7279  ignment of query
-00004fa0: 2073 6571 7565 6e63 6573 2074 6f20 6461   sequences to da
-00004fb0: 7461 6261 7365 206c 6f63 6920 7d0a 2020  tabase loci }.  
-00004fc0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00004fd0: 7d0a 0a0a 2a2a 4765 6e65 2050 726f 6669  }...**Gene Profi
-00004fe0: 6c65 2a2a 0a0a 5468 6973 2069 7320 6120  le**..This is a 
-00004ff0: 6c6f 6369 6465 7820 6465 6669 6e65 6420  locidex defined 
-00005000: 6669 6c65 7479 7065 2077 6869 6368 2075  filetype which u
-00005010: 7365 7320 5b4a 534f 4e5d 2868 7474 7073  ses [JSON](https
-00005020: 3a2f 2f77 7777 2e6a 736f 6e2e 6f72 672f  ://www.json.org/
-00005030: 6a73 6f6e 2d65 6e2e 6874 6d6c 2920 746f  json-en.html) to
-00005040: 2073 746f 7265 2069 6e66 6f72 6d61 7469   store informati
-00005050: 6f6e 2061 626f 7574 2074 6865 200a 7175  on about the .qu
-00005060: 6572 7920 7365 7175 656e 6365 2068 6173  ery sequence has
-00005070: 6865 7320 7468 6174 2061 7265 2061 7373  hes that are ass
-00005080: 6f63 6961 7465 6420 746f 2061 206c 6f63  ociated to a loc
-00005090: 7573 2e20 416c 6c20 6c6f 6369 2069 6e20  us. All loci in 
-000050a0: 7468 6520 6461 7461 6261 7365 2077 696c  the database wil
-000050b0: 6c20 6170 7065 6172 2069 6e20 6461 7461  l appear in data
-000050c0: 6261 7365 206f 7264 6572 0a61 6e64 2061  base order.and a
-000050d0: 7265 2069 6e63 6c75 6465 6420 7768 6574  re included whet
-000050e0: 6865 7220 7468 6579 2068 6176 6520 6120  her they have a 
-000050f0: 7175 6572 7920 6d61 7463 6820 6f72 206e  query match or n
-00005100: 6f74 2e20 5468 6973 2066 6f72 6d61 7420  ot. This format 
-00005110: 6973 2075 7365 6420 6173 2069 6e70 7574  is used as input
-00005120: 2074 6f20 6c6f 6369 6465 7820 6d65 7267   to locidex merg
-00005130: 652e 0a0a 2020 2020 7361 6d70 6c65 5f6e  e...    sample_n
-00005140: 616d 6520 3a20 7b0a 2020 2020 2020 2020  ame : {.        
-00005150: 2020 2020 2020 2020 276c 6f63 7573 5f31          'locus_1
-00005160: 273a 2027 3231 3936 3939 6565 6366 6431  ': '219699eecfd1
-00005170: 3137 3664 3663 3664 3534 3039 6236 3065  176d6c6d5409b60e
-00005180: 6435 3536 272c 0a20 2020 2020 2020 2020  d556',.         
-00005190: 2020 2020 2020 2027 6c6f 6375 735f 3227         'locus_2'
-000051a0: 3a20 2737 3538 3134 3662 6436 3937 6138  : '758146bd697a8
-000051b0: 3538 6338 6364 6361 3733 3232 6235 3432  58c8cdca7322b542
-000051c0: 3838 3127 2c0a 2020 2020 2020 2020 2020  881',.          
-000051d0: 2020 2020 2020 276c 6f63 7573 5f33 273a        'locus_3':
-000051e0: 2027 272c 2020 2020 2020 2020 2020 2020   '',            
-000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005200: 2020 2020 2020 2020 2020 2020 2020 234d                #M
-00005210: 6973 7369 6e67 206c 6f63 7573 0a20 2020  issing locus.   
-00005220: 2020 2020 2020 2020 2020 2020 2027 6c6f               'lo
-00005230: 6375 735f 3427 3a20 2765 3230 6161 6362  cus_4': 'e20aacb
-00005240: 3765 6665 3532 3839 6135 3632 3633 3737  7efe5289a5626377
-00005250: 6134 3564 6463 6661 3727 2c0a 2020 2020  a45ddcfa7',.    
-00005260: 2020 2020 2020 2020 2020 2020 276c 6f63              'loc
-00005270: 7573 5f35 273a 2027 3965 3562 6262 6462  us_5': '9e5bbbdb
-00005280: 3061 6232 6635 6563 3835 3038 3862 6163  0ab2f5ec85088bac
-00005290: 6430 3136 3762 3835 272c 0a20 2020 2020  d0167b85',.     
-000052a0: 2020 2020 2020 2020 2020 2027 6c6f 6375             'locu
-000052b0: 735f 3627 3a20 2732 3732 6538 3461 3463  s_6': '272e84a4c
-000052c0: 6534 6438 6133 3736 6664 3561 3431 6265  e4d8a376fd5a41be
-000052d0: 6339 3461 6433 3627 2c0a 2020 2020 2020  c94ad36',.      
-000052e0: 2020 2020 2020 2020 2020 276c 6f63 7573            'locus
-000052f0: 5f37 273a 2027 6363 3133 3131 3335 3966  _7': 'cc1311359f
-00005300: 6431 6364 3138 3033 3732 3265 6366 6665  d1cd1803722ecffe
-00005310: 6332 3739 6663 2c35 3036 3035 3332 3761  c279fc,50605327a
-00005320: 3334 3763 6137 6435 3430 3732 3265 3639  347ca7d540722e69
-00005330: 6266 3232 3034 6627 2c20 234d 756c 7469  bf2204f', #Multi
-00005340: 706c 6520 7175 6572 6965 7320 6d61 7463  ple queries matc
-00005350: 6820 6c6f 6375 730a 2020 2020 7d0a 0a23  h locus.    }..#
-00005360: 2320 5175 6963 6b20 5374 6172 740a 0a4d  # Quick Start..M
-00005370: 4c53 5420 4578 616d 706c 653a 2054 6865  LST Example: The
-00005380: 2037 2d67 656e 6520 4d4c 5354 2073 6368   7-gene MLST sch
-00005390: 656d 6520 7461 7267 6574 7320 6672 6f6d  eme targets from
-000053a0: 2068 7474 7073 3a2f 2f70 7562 6d6c 7374   https://pubmlst
-000053b0: 2e6f 7267 2f6f 7267 616e 6973 6d73 2f73  .org/organisms/s
-000053c0: 616c 6d6f 6e65 6c6c 612d 7370 7020 7765  almonella-spp we
-000053d0: 7265 2075 7365 6420 6173 2074 6172 6765  re used as targe
-000053e0: 7473 2074 6f20 6578 7472 6163 740a 7468  ts to extract.th
-000053f0: 6520 6675 6c6c 206c 656e 6774 6820 4344  e full length CD
-00005400: 5320 616e 6e6f 7461 7469 6f6e 7320 6672  S annotations fr
-00005410: 6f6d 204e 435f 3030 3331 3938 2e31 2028  om NC_003198.1 (
-00005420: 5361 6c6d 6f6e 656c 6c61 2054 7970 6869  Salmonella Typhi
-00005430: 2043 5431 3829 2e20 4e6f 7465 2074 6861   CT18). Note tha
-00005440: 7420 7468 6573 6520 6172 6520 6e6f 7420  t these are not 
-00005450: 6a75 7374 2074 6865 204d 4c53 5420 7461  just the MLST ta
-00005460: 7267 6574 2073 6571 7565 6e63 6573 0a62  rget sequences.b
-00005470: 7574 2074 6865 2066 756c 6c20 6f72 6620  ut the full orf 
-00005480: 616e 6420 736f 2074 6869 7320 7769 6c6c  and so this will
-00005490: 2064 6966 6665 7220 6672 6f6d 206e 6f72   differ from nor
-000054a0: 6d61 6c20 4d4c 5354 2072 6573 756c 7473  mal MLST results
-000054b0: 2e20 4966 2079 6f75 2077 616e 7420 746f  . If you want to
-000054c0: 2075 7365 2074 6865 2073 7562 7365 6374   use the subsect
-000054d0: 696f 6e73 206f 6620 7468 6520 6c6f 6369  ions of the loci
-000054e0: 2c20 796f 7520 7769 6c6c 206e 6565 640a  , you will need.
-000054f0: 746f 2065 7874 7261 6374 2074 6865 7365  to extract these
-00005500: 2075 7369 6e67 2061 6e6f 7468 6572 206d   using another m
-00005510: 6574 686f 642e 2054 6865 7365 2077 6572  ethod. These wer
-00005520: 6520 7365 7061 7261 7465 6420 696e 746f  e separated into
-00005530: 2069 6e64 6976 6964 7561 6c20 6661 7374   individual fast
-00005540: 6120 6669 6c65 730a 666f 7220 6561 6368  a files.for each
-00005550: 2067 656e 6520 6275 7420 6120 636f 6e63   gene but a conc
-00005560: 6174 6f6e 6174 6564 2076 6572 7369 6f6e  atonated version
-00005570: 2077 6f75 6c64 2061 6c73 6f20 776f 726b   would also work
-00005580: 2061 7320 6c6f 6e67 2061 7320 7468 6520   as long as the 
-00005590: 6661 7374 6120 6865 6164 6572 2062 6567  fasta header beg
-000055a0: 616e 2077 6974 6820 7468 6520 6c6f 6375  an with the locu
-000055b0: 7320 6964 656e 7469 6669 6572 2e0a 466f  s identifier..Fo
-000055c0: 726d 6174 2069 7320 7573 6564 2074 6f20  rmat is used to 
-000055d0: 7461 6b65 2074 6865 2066 6173 7461 2066  take the fasta f
-000055e0: 696c 6573 2074 6f20 6372 6561 7465 2061  iles to create a
-000055f0: 2054 5356 2066 696c 6520 7769 7468 2065   TSV file with e
-00005600: 6163 6820 6f66 2074 6865 2074 6172 6765  ach of the targe
-00005610: 7473 2061 6e64 2069 6e64 6976 6964 7561  ts and individua
-00005620: 6c20 6d61 7463 6820 7468 7265 7368 6f6c  l match threshol
-00005630: 6473 2066 6f72 2065 6163 6820 7175 6572  ds for each quer
-00005640: 792e 0a54 6865 7365 2063 616e 2062 6520  y..These can be 
-00005650: 6d6f 6469 6669 6564 2062 7920 7468 6520  modified by the 
-00005660: 7573 6572 2062 6566 6f72 6520 6275 696c  user before buil
-00005670: 6469 6e67 2074 6865 2064 6174 6162 6173  ding the databas
-00005680: 652e 2054 6865 2062 7569 6c64 2066 756e  e. The build fun
-00005690: 6374 696f 6e20 636f 6e76 6572 7473 2074  ction converts t
-000056a0: 6861 7420 5453 5620 696e 746f 2061 2066  hat TSV into a f
-000056b0: 6f72 6d20 7468 6174 206c 6f63 6964 6578  orm that locidex
-000056c0: 2073 6561 7263 6820 6361 6e20 7573 652e   search can use.
-000056d0: 0a49 6e20 6f72 6465 7220 746f 2063 616c  .In order to cal
-000056e0: 6c20 7468 6520 616c 6c65 6c65 7320 6672  l the alleles fr
-000056f0: 6f6d 2074 6865 2062 6c61 7374 2072 6573  om the blast res
-00005700: 756c 7473 206f 6620 7468 6520 7365 6172  ults of the sear
-00005710: 6368 206d 6f64 756c 652c 2074 6865 2072  ch module, the r
-00005720: 6570 6f72 7420 6d6f 6475 6c65 2069 7320  eport module is 
-00005730: 6361 6c6c 6564 2061 6e64 2074 6865 2073  called and the s
-00005740: 616d 706c 6573 2061 7265 206e 616d 6564  amples are named
-00005750: 2062 6173 6564 206f 6e20 7468 6520 0a75   based on the .u
-00005760: 7365 7220 696e 7075 742e 2049 6620 6e6f  ser input. If no
-00005770: 206e 616d 6520 6973 2073 7065 6369 6669   name is specifi
-00005780: 6564 2074 6865 6e20 7468 6520 6261 7365  ed then the base
-00005790: 206e 616d 6520 6f66 2074 6865 2066 696c   name of the fil
-000057a0: 6520 6973 2075 7365 642e 2046 696e 616c  e is used. Final
-000057b0: 6c79 2c20 7468 6520 696e 6469 7669 6475  ly, the individu
-000057c0: 616c 2070 726f 6669 6c65 7320 6172 6520  al profiles are 
-000057d0: 6d65 7267 6564 2069 6e74 6f20 6120 5453  merged into a TS
-000057e0: 5620 6669 6c65 2077 6869 6368 200a 6973  V file which .is
-000057f0: 2063 6f6d 7061 7469 626c 6520 7769 7468   compatible with
-00005800: 2064 6f77 6e73 7472 6561 6d20 6765 6e65   downstream gene
-00005810: 2070 726f 6669 6c65 2069 6e70 7574 2e0a   profile input..
-00005820: 0a20 2020 206c 6f63 6964 6578 2066 6f72  .    locidex for
-00005830: 6d61 7420 2d69 207e 2f65 7861 6d70 6c65  mat -i ~/example
-00005840: 2f66 6f72 6d61 745f 6462 5f6d 6c73 745f  /format_db_mlst_
-00005850: 696e 2f20 2d6f 207e 2f65 7861 6d70 6c65  in/ -o ~/example
-00005860: 2f66 6f72 6d61 745f 6462 5f6d 6c73 745f  /format_db_mlst_
-00005870: 6f75 742f 202d 2d66 6f72 6365 0a20 2020  out/ --force.   
-00005880: 206c 6f63 6964 6578 2062 7569 6c64 202d   locidex build -
-00005890: 6920 7e2f 6578 616d 706c 652f 666f 726d  i ~/example/form
-000058a0: 6174 5f64 625f 6d6c 7374 5f6f 7574 2f6c  at_db_mlst_out/l
-000058b0: 6f63 6964 6578 2e74 7874 202d 6f20 7e2f  ocidex.txt -o ~/
-000058c0: 6578 616d 706c 652f 6275 696c 645f 6462  example/build_db
-000058d0: 5f6d 6c73 745f 6f75 742f 202d 2d66 6f72  _mlst_out/ --for
-000058e0: 6365 0a20 2020 200a 2020 2020 6c6f 6369  ce.    .    loci
-000058f0: 6465 7820 7365 6172 6368 202d 7120 7e2f  dex search -q ~/
-00005900: 6578 616d 706c 652f 7365 6172 6368 2f4e  example/search/N
-00005910: 435f 3030 3331 3938 2e31 2e67 626b 202d  C_003198.1.gbk -
-00005920: 6420 7e2f 6578 616d 706c 652f 6275 696c  d ~/example/buil
-00005930: 645f 6462 5f6d 6c73 745f 6f75 742f 202d  d_db_mlst_out/ -
-00005940: 6f20 2e2f 6d6c 7374 5f6e 6362 695f 616e  o ./mlst_ncbi_an
-00005950: 6e6f 7461 7465 6420 2d2d 666f 7263 6520  notated --force 
-00005960: 0a20 2020 206c 6f63 6964 6578 2073 6561  .    locidex sea
-00005970: 7263 6820 2d71 207e 2f65 7861 6d70 6c65  rch -q ~/example
-00005980: 2f73 6561 7263 682f 4e43 5f30 3033 3139  /search/NC_00319
-00005990: 382e 312e 6661 7374 6120 2d64 207e 2f65  8.1.fasta -d ~/e
-000059a0: 7861 6d70 6c65 2f62 7569 6c64 5f64 625f  xample/build_db_
-000059b0: 6d6c 7374 5f6f 7574 2f20 2d6f 202e 2f6d  mlst_out/ -o ./m
-000059c0: 6c73 745f 7072 6f64 6967 616c 202d 2d66  lst_prodigal --f
-000059d0: 6f72 6365 202d 2d61 6e6e 6f74 6174 650a  orce --annotate.
-000059e0: 2020 2020 0a20 2020 206c 6f63 6964 6578      .    locidex
-000059f0: 2072 6570 6f72 7420 2d69 202e 2f6d 6c73   report -i ./mls
-00005a00: 745f 6e63 6269 5f61 6e6e 6f74 6174 6564  t_ncbi_annotated
-00005a10: 2f73 6571 5f73 746f 7265 2e6a 736f 6e20  /seq_store.json 
-00005a20: 2d6f 202e 2f6d 6c73 745f 6e63 6269 5f61  -o ./mlst_ncbi_a
-00005a30: 6e6e 6f74 6174 6564 2f72 6570 6f72 7420  nnotated/report 
-00005a40: 2d2d 6e61 6d65 206e 6362 6920 2d2d 666f  --name ncbi --fo
-00005a50: 7263 650a 2020 2020 6c6f 6369 6465 7820  rce.    locidex 
-00005a60: 7265 706f 7274 202d 6920 2e2f 6d6c 7374  report -i ./mlst
-00005a70: 5f70 726f 6469 6761 6c2f 7365 715f 7374  _prodigal/seq_st
-00005a80: 6f72 652e 6a73 6f6e 202d 6f20 2e2f 6d6c  ore.json -o ./ml
-00005a90: 7374 5f70 726f 6469 6761 6c2f 7265 706f  st_prodigal/repo
-00005aa0: 7274 202d 2d6e 616d 6520 7072 6f64 6967  rt --name prodig
-00005ab0: 616c 202d 2d66 6f72 6365 0a20 2020 200a  al --force.    .
-00005ac0: 2020 2020 6c6f 6369 6465 7820 6d65 7267      locidex merg
-00005ad0: 6520 2d69 202e 2f6d 6c73 745f 6e63 6269  e -i ./mlst_ncbi
-00005ae0: 5f61 6e6e 6f74 6174 6564 2f72 6570 6f72  _annotated/repor
-00005af0: 742f 7072 6f66 696c 652e 6a73 6f6e 202e  t/profile.json .
-00005b00: 2f2f 6d6c 7374 5f70 726f 6469 6761 6c2f  //mlst_prodigal/
-00005b10: 7265 706f 7274 2f70 726f 6669 6c65 2e6a  report/profile.j
-00005b20: 736f 6e20 2d6f 202e 2f6d 6572 6765 6420  son -o ./merged 
-00005b30: 2d2d 666f 7263 650a 2020 2020 0a20 2020  --force.    .   
-00005b40: 200a 0a0a 2323 2042 656e 6368 6d61 726b   ...## Benchmark
-00005b50: 730a 0a43 6f6d 696e 6720 736f 6f6e 0a0a  s..Coming soon..
-00005b60: 2323 2046 4151 0a0a 2a2a 4361 6e20 4920  ## FAQ..**Can I 
-00005b70: 7573 6520 6e6f 6e2d 636f 6469 6e67 2073  use non-coding s
-00005b80: 6571 7565 6e63 6573 2061 7320 696e 7075  equences as inpu
-00005b90: 7420 746f 206c 6f63 6964 6578 3f2a 2a0a  t to locidex?**.
-00005ba0: 0a59 6573 2c20 796f 7520 6361 6e20 746f  .Yes, you can to
-00005bb0: 6767 6c65 206f 6666 2070 726f 7465 696e  ggle off protein
-00005bc0: 2063 6f64 696e 6720 7769 7468 696e 2074   coding within t
-00005bd0: 6865 2064 6174 6162 6173 6520 636f 6e66  he database conf
-00005be0: 6967 2074 6f20 6176 6f69 6420 7472 616e  ig to avoid tran
-00005bf0: 736c 6174 696f 6e20 616e 6420 7072 6f74  slation and prot
-00005c00: 6569 6e20 626c 6173 7420 7365 6172 6368  ein blast search
-00005c10: 6573 2e0a 486f 7765 7665 722c 2069 6620  es..However, if 
-00005c20: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-00005c30: 7468 6520 2261 6c6c 656c 6522 2069 6465  the "allele" ide
-00005c40: 6e74 6974 7920 6f66 2079 6f75 7220 6c6f  ntity of your lo
-00005c50: 6375 7320 7375 6368 2061 7320 616e 2072  cus such as an r
-00005c60: 524e 4120 6765 6e65 2c20 7468 656e 2079  RNA gene, then y
-00005c70: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
-00005c80: 6578 7472 6163 7420 6f75 7420 7468 6520  extract out the 
-00005c90: 7365 7175 656e 6365 730a 796f 7520 7761  sequences.you wa
-00005ca0: 6e74 2074 6f20 6d61 7463 682e 0a0a 2a2a  nt to match...**
-00005cb0: 446f 2049 206e 6565 6420 746f 2068 6176  Do I need to hav
-00005cc0: 6520 6120 7265 7072 6573 656e 7469 7469  e a representiti
-00005cd0: 7665 206f 6620 6576 6572 7920 616c 6c65  ve of every alle
-00005ce0: 6c65 2049 2077 616e 7420 746f 206d 6174  le I want to mat
-00005cf0: 6368 2069 6e20 6d79 2064 6174 6162 6173  ch in my databas
-00005d00: 653f 2a2a 0a0a 4e6f 2c20 7468 6520 6265  e?**..No, the be
-00005d10: 6e65 6669 7420 6f66 2068 6176 696e 6720  nefit of having 
-00005d20: 6475 616c 2073 6561 7263 6869 6e67 2077  dual searching w
-00005d30: 6974 6820 7072 6f74 6569 6e20 616e 6420  ith protein and 
-00005d40: 646e 6120 6973 2074 6861 7420 796f 7520  dna is that you 
-00005d50: 6361 6e20 6861 7665 2061 2073 7061 7273  can have a spars
-00005d60: 656c 7920 706f 7075 6c61 7465 6420 6461  ely populated da
-00005d70: 7461 6261 7365 206f 6620 7365 7175 656e  tabase of sequen
-00005d80: 6365 7320 7468 6174 200a 6d65 6574 2079  ces that .meet y
-00005d90: 6f75 7220 6170 706c 6963 6174 696f 6e73  our applications
-00005da0: 2073 7065 6369 6669 6320 6e65 6564 2e20   specific need. 
-00005db0: 2054 6869 7320 6d65 616e 7320 796f 7520   This means you 
-00005dc0: 6361 6e20 6465 6475 706c 6963 6174 6520  can deduplicate 
-00005dd0: 7573 696e 6720 6120 746f 6f6c 2073 7563  using a tool suc
-00005de0: 6820 6173 205b 6364 2d68 6974 5d28 6874  h as [cd-hit](ht
-00005df0: 7470 733a 2f2f 7369 7465 732e 676f 6f67  tps://sites.goog
-00005e00: 6c65 2e63 6f6d 2f76 6965 772f 6364 2d68  le.com/view/cd-h
-00005e10: 6974 2920 746f 2072 656d 6f76 6520 6869  it) to remove hi
-00005e20: 6768 6c79 2073 696d 696c 6172 2073 6571  ghly similar seq
-00005e30: 7565 6e63 6573 0a66 726f 6d20 796f 7572  uences.from your
-00005e40: 2064 6174 6162 6173 6520 746f 2072 6564   database to red
-00005e50: 7563 6520 7275 6e74 696d 6520 616e 6420  uce runtime and 
-00005e60: 636f 6d70 6c65 7869 7479 2e20 596f 7520  complexity. You 
-00005e70: 7769 6c6c 206e 6565 6420 746f 2065 6d70  will need to emp
-00005e80: 6972 6163 6c79 2064 6574 6572 6d69 6e65  iracly determine
-00005e90: 2077 6861 7420 6c65 7665 6c20 6f66 2064   what level of d
-00005ea0: 6976 6572 7369 7479 2069 7320 7375 6666  iversity is suff
-00005eb0: 6963 6965 6e74 0a66 6f72 2079 6f75 7220  icient.for your 
-00005ec0: 7370 6563 6966 6963 2061 7070 6c69 6361  specific applica
-00005ed0: 7469 6f6e 2e0a 0a2a 2a48 6f77 2064 6f65  tion...**How doe
-00005ee0: 7320 4c6f 6369 6465 7820 6861 6e64 656c  s Locidex handel
-00005ef0: 206d 756c 7469 636f 7079 206c 6f63 693f   multicopy loci?
-00005f00: 2a2a 0a0a 4964 6561 6c6c 7920 6120 6765  **..Ideally a ge
-00005f10: 6e65 2d62 792d 6765 6e65 2073 6368 656d  ne-by-gene schem
-00005f20: 6520 636f 6e73 6973 7473 206f 6620 6f6e  e consists of on
-00005f30: 6c79 2073 696e 676c 6520 636f 7079 2067  ly single copy g
-00005f40: 656e 6573 2062 7574 2062 6163 7465 7269  enes but bacteri
-00005f50: 616c 2067 656e 6f6d 6573 2061 7265 2064  al genomes are d
-00005f60: 796e 616d 6963 2061 6e64 200a 6765 6e75  ynamic and .genu
-00005f70: 696e 6520 6475 6c70 6c69 6361 7469 6f6e  ine dulplication
-00005f80: 7320 6361 6e20 6f63 6375 722c 2069 6e20  s can occur, in 
-00005f90: 6164 6469 7469 6f6e 2074 6f20 6173 7365  addition to asse
-00005fa0: 6d62 6c79 2061 7274 6966 6163 7473 2061  mbly artifacts a
-00005fb0: 6e64 2063 6f6e 7461 6d69 6e61 7469 6f6e  nd contamination
-00005fc0: 2e20 5468 6572 6520 6172 6520 6120 7661  . There are a va
-00005fd0: 7269 6574 7920 6f66 2061 7070 726f 6163  riety of approac
-00005fe0: 6865 730a 6176 6169 6c61 626c 6520 746f  hes.available to
-00005ff0: 206d 616e 6167 6573 2074 6865 7365 2063   manages these c
-00006000: 6173 6573 2e20 5769 7468 696e 2074 6865  ases. Within the
-00006010: 2037 2d67 656e 6520 5b6d 6c73 745d 2868   7-gene [mlst](h
-00006020: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00006030: 6d2f 7473 6565 6d61 6e6e 2f6d 6c73 7429  m/tseemann/mlst)
-00006040: 2074 6f6f 6c20 6d75 6c74 6970 6c65 2061   tool multiple a
-00006050: 6c6c 656c 6573 2066 6f72 2061 2067 6976  lleles for a giv
-00006060: 656e 206c 6f63 7573 2061 7265 2072 6570  en locus are rep
-00006070: 6f72 7465 6420 0a77 6974 6820 6120 636f  orted .with a co
-00006080: 6d6d 6120 6465 6c69 6d69 7469 6e67 2065  mma delimiting e
-00006090: 6163 6820 616c 6c65 6c65 2e20 486f 7765  ach allele. Howe
-000060a0: 7665 722c 2074 6869 7320 706f 7365 7320  ver, this poses 
-000060b0: 616e 2069 7373 7565 2066 6f72 2063 616c  an issue for cal
-000060c0: 6375 6c61 7469 6e67 2067 656e 6574 6963  culating genetic
-000060d0: 2064 6973 7461 6e63 6573 2073 696e 6365   distances since
-000060e0: 2069 7420 6973 2075 6e63 6c65 6172 2068   it is unclear h
-000060f0: 6f77 2074 6f20 7472 6561 740a 7468 6520  ow to treat.the 
-00006100: 6d75 6c74 6970 6c65 2061 6c6c 656c 6573  multiple alleles
-00006110: 2e20 3129 2074 7265 6174 2074 6865 2063  . 1) treat the c
-00006120: 6f6d 6269 6e61 7469 6f6e 2061 7320 6120  ombination as a 
-00006130: 6e6f 7665 6c20 616c 6c65 6c65 2032 2920  novel allele 2) 
-00006140: 626c 616e 6b20 7468 6520 636f 6c75 6d6e  blank the column
-00006150: 2033 2920 7365 6c65 6374 2074 6865 2065   3) select the e
-00006160: 6172 6c69 6573 7420 616c 6c65 6c65 2069  arliest allele i
-00006170: 6e20 7468 6520 6461 7461 6261 7365 2034  n the database 4
-00006180: 290a 5573 6520 6120 7369 6d69 6c61 7269  ).Use a similari
-00006190: 7479 2073 636f 7265 2074 6f20 7261 7465  ty score to rate
-000061a0: 2077 6869 6368 2069 7320 7468 6520 6265   which is the be
-000061b0: 7374 2061 6c6c 656c 6520 746f 2069 6e63  st allele to inc
-000061c0: 6c75 6465 2e20 5468 6520 6d6f 7374 2063  lude. The most c
-000061d0: 6f6e 7365 7276 6174 6976 6520 6170 7072  onservative appr
-000061e0: 6f61 6368 2069 7320 746f 206e 6f74 2069  oach is to not i
-000061f0: 6e74 6572 7072 6574 2074 6861 7420 636f  nterpret that co
-00006200: 6c75 6d6e 0a62 7920 626c 616e 6b69 6e67  lumn.by blanking
-00006210: 2069 7420 696e 2064 6973 7461 6e63 6520   it in distance 
-00006220: 6361 6c63 756c 6174 696f 6e73 2077 6869  calculations whi
-00006230: 6368 2072 6573 756c 7473 2069 6e20 626c  ch results in bl
-00006240: 756e 7469 6e67 2072 6573 6f6c 7574 696f  unting resolutio
-00006250: 6e20 7768 6963 6820 6973 2069 6d70 6c65  n which is imple
-00006260: 6d65 6e74 6564 2077 6974 6869 6e67 206c  mented withing l
-00006270: 6f63 6964 6578 2061 7320 7468 6520 636f  ocidex as the co
-00006280: 6e73 6572 7661 7469 7665 206d 6f64 652e  nservative mode.
-00006290: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
-000062a0: 6279 2075 7369 6e67 2061 6e20 6170 7072  by using an appr
-000062b0: 6f61 6368 2074 6f20 7365 6c65 6374 206f  oach to select o
-000062c0: 6e6c 7920 6f6e 6520 6f66 2074 6865 206c  nly one of the l
-000062d0: 6f63 6920 746f 206d 6174 6368 2077 696c  oci to match wil
-000062e0: 6c20 6861 7665 206d 6978 6564 2065 6666  l have mixed eff
-000062f0: 6563 7420 286f 7074 696f 6e73 2033 2c20  ect (options 3, 
-00006300: 3429 2074 6861 7420 6361 6e20 7265 7375  4) that can resu
-00006310: 6c74 2069 6e0a 696e 636f 6e73 6973 7465  lt in.inconsiste
-00006320: 6e63 6965 7320 7768 6572 6520 736f 6d65  ncies where some
-00006330: 2069 736f 6c61 7465 7320 6170 7065 6172   isolates appear
-00006340: 6520 6d6f 7265 2073 696d 696c 6172 206f  e more similar o
-00006350: 7220 6469 7373 696d 696c 6172 2074 6861  r dissimilar tha
-00006360: 6e20 7468 6579 2061 7265 2e20 2054 6865  n they are.  The
-00006370: 2070 7265 6665 7265 6420 6d65 7468 6f64   prefered method
-00006380: 2074 6861 7420 6c6f 6369 6465 7820 6861   that locidex ha
-00006390: 7320 696d 706c 656e 7465 6420 6173 2069  s implented as i
-000063a0: 7473 2064 6566 6175 6c74 2028 6e6f 726d  ts default (norm
-000063b0: 616c 290a 6d6f 6465 2069 7320 746f 2063  al).mode is to c
-000063c0: 6f6d 6269 6e65 2074 6865 2072 6573 756c  ombine the resul
-000063d0: 7420 696e 746f 2061 206e 6577 2022 616c  t into a new "al
-000063e0: 6c65 6c65 2220 6861 7368 2074 6861 7420  lele" hash that 
-000063f0: 6973 2064 6572 6976 6564 2066 726f 6d20  is derived from 
-00006400: 6361 6c63 756c 6174 696e 6720 7468 6520  calculating the 
-00006410: 6d64 3520 6861 7368 206f 6620 7468 6520  md5 hash of the 
-00006420: 636f 6e63 6174 6f6e 6174 6564 2061 6c6c  concatonated all
-00006430: 656c 6520 6d64 3520 6861 7368 6573 2077  ele md5 hashes w
-00006440: 6869 6368 0a68 6176 6520 6265 656e 2073  hich.have been s
-00006450: 6f72 7465 6420 616c 7068 6162 6574 6963  orted alphabetic
-00006460: 616c 6c79 2e20 5468 6973 2068 6173 2074  ally. This has t
-00006470: 6865 2062 656e 6566 6974 206f 6620 7468  he benefit of th
-00006480: 6520 7361 6d65 2063 6f6d 6269 6e61 7469  e same combinati
-00006490: 6f6e 206f 6620 616c 6c65 6c65 7320 7769  on of alleles wi
-000064a0: 6c6c 2061 6c77 6179 7320 7265 7375 6c74  ll always result
-000064b0: 2069 6e20 7468 6520 7361 6d65 2068 6173   in the same has
-000064c0: 6820 636f 6465 2061 6e64 2077 696c 6c20  h code and will 
-000064d0: 6d61 7463 6820 7768 656e 2074 6869 7320  match when this 
-000064e0: 6f63 6375 7273 2e0a 436f 6e76 6572 7365  occurs..Converse
-000064f0: 6c79 2c20 6974 2077 696c 6c20 636f 756e  ly, it will coun
-00006500: 7420 6120 6469 6666 6572 656e 6365 2065  t a difference e
-00006510: 7665 6e20 7768 656e 2074 6865 2063 6f6d  ven when the com
-00006520: 706f 6e65 6e74 2061 6c6c 656c 6573 206d  ponent alleles m
-00006530: 6179 206d 6174 6368 2062 6574 7765 656e  ay match between
-00006540: 2074 776f 2073 616d 706c 6573 2e0a 0a0a   two samples....
-00006550: 2323 2043 6974 6174 696f 6e0a 0a52 6f62  ## Citation..Rob
-00006560: 6572 7473 6f6e 2c20 4a61 6d65 732c 2057  ertson, James, W
-00006570: 656c 6c73 2c20 4d61 7474 6865 772c 2043  ells, Matthew, C
-00006580: 6872 6973 7479 2d4c 796e 6e2c 2050 6574  hristy-Lynn, Pet
-00006590: 6572 736f 6e2c 204b 7972 796c 6f20 4265  erson, Kyrylo Be
-000065a0: 7373 6f6e 6f76 2c20 5265 696d 6572 2c20  ssonov, Reimer, 
-000065b0: 416c 6569 7368 612c 2053 6368 6f6e 6665  Aleisha, Schonfe
-000065c0: 6c64 2c20 4a75 7374 696e 2e20 4c4f 4349  ld, Justin. LOCI
-000065d0: 4445 583a 2044 6973 7472 6962 7574 6564  DEX: Distributed
-000065e0: 2061 6c6c 656c 6520 6361 6c6c 696e 6720   allele calling 
-000065f0: 656e 6769 6e65 2e20 3230 3234 2e20 6874  engine. 2024. ht
-00006600: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00006610: 2f70 6861 632d 6e6d 6c2f 6c6f 6369 6465  /phac-nml/locide
-00006620: 780a 0a23 2320 4c65 6761 6c0a 0a43 6f70  x..## Legal..Cop
-00006630: 7972 6967 6874 2047 6f76 6572 6e6d 656e  yright Governmen
-00006640: 7420 6f66 2043 616e 6164 6120 3230 3233  t of Canada 2023
-00006650: 0a0a 5772 6974 7465 6e20 6279 3a20 4e61  ..Written by: Na
-00006660: 7469 6f6e 616c 204d 6963 726f 6269 6f6c  tional Microbiol
-00006670: 6f67 7920 4c61 626f 7261 746f 7279 2c20  ogy Laboratory, 
-00006680: 5075 626c 6963 2048 6561 6c74 6820 4167  Public Health Ag
-00006690: 656e 6379 206f 6620 4361 6e61 6461 0a0a  ency of Canada..
-000066a0: 4c69 6365 6e73 6564 2075 6e64 6572 2074  Licensed under t
-000066b0: 6865 2041 7061 6368 6520 4c69 6365 6e73  he Apache Licens
-000066c0: 652c 2056 6572 7369 6f6e 2032 2e30 2028  e, Version 2.0 (
-000066d0: 7468 6520 224c 6963 656e 7365 2229 3b20  the "License"); 
-000066e0: 796f 7520 6d61 7920 6e6f 7420 7573 650a  you may not use.
-000066f0: 7468 6973 2077 6f72 6b20 6578 6365 7074  this work except
-00006700: 2069 6e20 636f 6d70 6c69 616e 6365 2077   in compliance w
-00006710: 6974 6820 7468 6520 4c69 6365 6e73 652e  ith the License.
-00006720: 2059 6f75 206d 6179 206f 6274 6169 6e20   You may obtain 
-00006730: 6120 636f 7079 206f 6620 7468 650a 4c69  a copy of the.Li
-00006740: 6365 6e73 6520 6174 3a0a 0a68 7474 703a  cense at:..http:
-00006750: 2f2f 7777 772e 6170 6163 6865 2e6f 7267  //www.apache.org
-00006760: 2f6c 6963 656e 7365 732f 4c49 4345 4e53  /licenses/LICENS
-00006770: 452d 322e 300a 0a55 6e6c 6573 7320 7265  E-2.0..Unless re
-00006780: 7175 6972 6564 2062 7920 6170 706c 6963  quired by applic
-00006790: 6162 6c65 206c 6177 206f 7220 6167 7265  able law or agre
-000067a0: 6564 2074 6f20 696e 2077 7269 7469 6e67  ed to in writing
-000067b0: 2c20 736f 6674 7761 7265 2064 6973 7472  , software distr
-000067c0: 6962 7574 6564 0a75 6e64 6572 2074 6865  ibuted.under the
-000067d0: 204c 6963 656e 7365 2069 7320 6469 7374   License is dist
-000067e0: 7269 6275 7465 6420 6f6e 2061 6e20 2241  ributed on an "A
-000067f0: 5320 4953 2220 4241 5349 532c 2057 4954  S IS" BASIS, WIT
-00006800: 484f 5554 2057 4152 5241 4e54 4945 5320  HOUT WARRANTIES 
-00006810: 4f52 0a43 4f4e 4449 5449 4f4e 5320 4f46  OR.CONDITIONS OF
-00006820: 2041 4e59 204b 494e 442c 2065 6974 6865   ANY KIND, eithe
-00006830: 7220 6578 7072 6573 7320 6f72 2069 6d70  r express or imp
-00006840: 6c69 6564 2e20 5365 6520 7468 6520 4c69  lied. See the Li
-00006850: 6365 6e73 6520 666f 7220 7468 650a 7370  cense for the.sp
-00006860: 6563 6966 6963 206c 616e 6775 6167 6520  ecific language 
-00006870: 676f 7665 726e 696e 6720 7065 726d 6973  governing permis
-00006880: 7369 6f6e 7320 616e 6420 6c69 6d69 7461  sions and limita
-00006890: 7469 6f6e 7320 756e 6465 7220 7468 6520  tions under the 
-000068a0: 4c69 6365 6e73 652e 0a0a 0a23 2320 436f  License....## Co
-000068b0: 6e74 6163 740a 0a2a 2a4a 616d 6573 2052  ntact..**James R
-000068c0: 6f62 6572 7473 6f6e 2a2a 3a20 6a61 6d65  obertson**: jame
-000068d0: 732e 726f 6265 7274 736f 6e40 7068 6163  s.robertson@phac
-000068e0: 2d61 7370 632e 6763 2e63 610a            -aspc.gc.ca.
+00000060: 782f 2364 6573 6372 6970 7469 6f6e 290d  x/#description).
+00000070: 0a5b 215b 4269 6f63 6f6e 6461 5d28 6874  .[![Bioconda](ht
+00000080: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000090: 732e 696f 2f62 6164 6765 2f49 6e73 7461  s.io/badge/Insta
+000000a0: 6c6c 2532 3077 6974 682d 6269 6f63 6f6e  ll%20with-biocon
+000000b0: 6461 2d67 7265 656e 295d 2868 7474 7073  da-green)](https
+000000c0: 3a2f 2f61 6e61 636f 6e64 612e 6f72 672f  ://anaconda.org/
+000000d0: 6269 6f63 6f6e 6461 2f6c 6f63 6964 6578  bioconda/locidex
+000000e0: 290d 0a5b 215b 436f 6e64 615d 2868 7474  )..[![Conda](htt
+000000f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000100: 2e69 6f2f 636f 6e64 612f 646e 2f62 696f  .io/conda/dn/bio
+00000110: 636f 6e64 612f 6c6f 6369 6465 783f 636f  conda/locidex?co
+00000120: 6c6f 723d 6772 6565 6e29 5d28 6874 7470  lor=green)](http
+00000130: 733a 2f2f 616e 6163 6f6e 6461 2e6f 7267  s://anaconda.org
+00000140: 2f62 696f 636f 6e64 612f 6c6f 6369 6465  /bioconda/locide
+00000150: 7829 0d0a 5b21 5b4c 6963 656e 7365 3a20  x)..[![License: 
+00000160: 4170 6163 6865 2d32 2e30 5d28 6874 7470  Apache-2.0](http
+00000170: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000180: 696f 2f67 6974 6875 622f 6c69 6365 6e73  io/github/licens
+00000190: 652f 7068 6163 2d6e 6d6c 2f6c 6f63 6964  e/phac-nml/locid
+000001a0: 6578 295d 2868 7474 7073 3a2f 2f77 7777  ex)](https://www
+000001b0: 2e61 7061 6368 652e 6f72 672f 6c69 6365  .apache.org/lice
+000001c0: 6e73 6573 2f4c 4943 454e 5345 2d32 2e30  nses/LICENSE-2.0
+000001d0: 290d 0a0d 0a3c 696d 6720 7372 633d 2268  )....<img src="h
+000001e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001f0: 6d2f 7068 6163 2d6e 6d6c 2f6c 6f63 6964  m/phac-nml/locid
+00000200: 6578 2f62 6c6f 622f 6465 762f 6173 7365  ex/blob/dev/asse
+00000210: 7473 2f6c 6f67 6f2e 706e 6722 2077 6964  ts/logo.png" wid
+00000220: 7468 203d 2022 3138 3022 2068 6569 6768  th = "180" heigh
+00000230: 743d 2231 3430 223e 0d0a 0d0a 2320 4c6f  t="140">....# Lo
+00000240: 6369 6465 780d 0a0d 0a2d 205b 496e 7472  cidex....- [Intr
+00000250: 6f64 7563 7469 6f6e 5d28 2369 6e74 726f  oduction](#intro
+00000260: 6475 6374 696f 6e29 0d0a 2020 2a20 5b43  duction)..  * [C
+00000270: 6974 6174 696f 6e5d 2823 6369 7461 7469  itation](#citati
+00000280: 6f6e 290d 0a20 202a 205b 436f 6e74 6163  on)..  * [Contac
+00000290: 745d 2823 636f 6e74 6163 7429 0d0a 2d20  t](#contact)..- 
+000002a0: 5b49 6e73 7461 6c6c 5d28 2369 6e73 7461  [Install](#insta
+000002b0: 6c6c 290d 0a20 2020 202b 205b 436f 6d70  ll)..    + [Comp
+000002c0: 6174 6962 696c 6974 795d 2823 636f 6d70  atibility](#comp
+000002d0: 6174 6962 696c 6974 7929 0d0a 2d20 5b47  atibility)..- [G
+000002e0: 6574 7469 6e67 2053 7461 7274 6564 5d28  etting Started](
+000002f0: 2367 6574 7469 6e67 2d73 7461 7274 6564  #getting-started
+00000300: 290d 0a20 202a 205b 5573 6167 655d 2823  )..  * [Usage](#
+00000310: 7573 6167 6529 0d0a 2020 2a20 5b43 6f6e  usage)..  * [Con
+00000320: 6669 6775 7261 7469 6f6e 2061 6e64 2053  figuration and S
+00000330: 6574 7469 6e67 735d 2823 636f 6e66 6967  ettings](#config
+00000340: 7572 6174 696f 6e2d 616e 642d 7365 7474  uration-and-sett
+00000350: 696e 6773 290d 0a20 2020 202b 205b 5365  ings)..    + [Se
+00000360: 6172 6368 5d28 2373 6561 7263 6829 0d0a  arch](#search)..
+00000370: 2020 2020 2b20 5b45 7874 7261 6374 5d28      + [Extract](
+00000380: 2365 7874 7261 6374 290d 0a20 2020 202b  #extract)..    +
+00000390: 205b 5265 706f 7274 5d28 2372 6570 6f72   [Report](#repor
+000003a0: 7429 0d0a 2020 2020 2b20 5b4d 6572 6765  t)..    + [Merge
+000003b0: 5d28 236d 6572 6765 290d 0a20 2020 202b  ](#merge)..    +
+000003c0: 205b 466f 726d 6174 5d28 2366 6f72 6d61   [Format](#forma
+000003d0: 7429 0d0a 2020 2020 2b20 5b42 7569 6c64  t)..    + [Build
+000003e0: 5d28 2362 7569 6c64 290d 0a20 202a 205b  ](#build)..  * [
+000003f0: 4578 616d 706c 6520 776f 726b 666c 6f77  Example workflow
+00000400: 5d28 2365 7861 6d70 6c65 2d77 6f72 6b66  ](#example-workf
+00000410: 6c6f 7729 0d0a 2020 2a20 5b44 6174 6162  low)..  * [Datab
+00000420: 6173 6520 7374 7275 6374 7572 655d 2823  ase structure](#
+00000430: 6461 7461 6261 7365 2d73 7472 7563 7475  database-structu
+00000440: 7265 290d 0a20 2020 202b 205b 636f 6e66  re)..    + [conf
+00000450: 6967 2e6a 736f 6e5d 2823 636f 6e66 6967  ig.json](#config
+00000460: 6a73 6f6e 290d 0a20 2020 202b 205b 6d65  json)..    + [me
+00000470: 7461 2e6a 736f 6e5d 2823 6d65 7461 6a73  ta.json](#metajs
+00000480: 6f6e 290d 0a20 2020 202b 205b 626c 6173  on)..    + [blas
+00000490: 7420 6461 7462 6173 6573 5d28 2362 6c61  t datbases](#bla
+000004a0: 7374 2d64 6174 6261 7365 7329 0d0a 2d20  st-datbases)..- 
+000004b0: 5b54 726f 7562 6c65 7368 6f6f 7469 6e67  [Troubleshooting
+000004c0: 2061 6e64 2046 4151 735d 2823 7472 6f75   and FAQs](#trou
+000004d0: 626c 6573 686f 6f74 696e 672d 616e 642d  bleshooting-and-
+000004e0: 6661 7173 290d 0a2d 205b 4265 6e63 686d  faqs)..- [Benchm
+000004f0: 6172 6b69 6e67 5d28 2362 656e 6368 6d61  arking](#benchma
+00000500: 726b 696e 6729 0d0a 2d20 5b4c 6567 616c  rking)..- [Legal
+00000510: 2061 6e64 2043 6f6d 706c 6961 6e63 6520   and Compliance 
+00000520: 496e 666f 726d 6174 696f 6e5d 2823 6c65  Information](#le
+00000530: 6761 6c2d 616e 642d 636f 6d70 6c69 616e  gal-and-complian
+00000540: 6365 2d69 6e66 6f72 6d61 7469 6f6e 290d  ce-information).
+00000550: 0a2d 205b 5570 6461 7465 7320 616e 6420  .- [Updates and 
+00000560: 5265 6c65 6173 6520 4e6f 7465 735d 2823  Release Notes](#
+00000570: 7570 6461 7465 732d 616e 642d 7265 6c65  updates-and-rele
+00000580: 6173 652d 6e6f 7465 7329 0d0a 0d0a 3c73  ase-notes)....<s
+00000590: 6d61 6c6c 3e3c 693e 3c61 2068 7265 663d  mall><i><a href=
+000005a0: 2768 7474 703a 2f2f 6563 6f74 7275 7374  'http://ecotrust
+000005b0: 2d63 616e 6164 612e 6769 7468 7562 2e69  -canada.github.i
+000005c0: 6f2f 6d61 726b 646f 776e 2d74 6f63 2f27  o/markdown-toc/'
+000005d0: 3e54 6162 6c65 206f 6620 636f 6e74 656e  >Table of conten
+000005e0: 7473 2067 656e 6572 6174 6564 2077 6974  ts generated wit
+000005f0: 6820 6d61 726b 646f 776e 2d74 6f63 3c2f  h markdown-toc</
+00000600: 613e 3c2f 693e 3c2f 736d 616c 6c3e 0d0a  a></i></small>..
+00000610: 0d0a 2320 496e 7472 6f64 7563 7469 6f6e  ..# Introduction
+00000620: 0d0a 4120 636f 6d6d 6f6e 2066 756e 6374  ..A common funct
+00000630: 696f 6e20 666f 7220 6d61 6e79 2074 6f6f  ion for many too
+00000640: 6c73 2069 6e20 6261 6374 6572 6961 6c20  ls in bacterial 
+00000650: 7479 7069 6e67 2069 7320 7065 7266 6f72  typing is perfor
+00000660: 6d69 6e67 2073 696d 696c 6172 6974 7920  ming similarity 
+00000670: 7365 6172 6368 696e 6720 7573 696e 6720  searching using 
+00000680: 4e43 4249 205b 626c 6173 745d 2868 7474  NCBI [blast](htt
+00000690: 7073 3a2f 2f62 6c61 7374 2e6e 6362 692e  ps://blast.ncbi.
+000006a0: 6e6c 6d2e 6e69 682e 676f 762f 426c 6173  nlm.nih.gov/Blas
+000006b0: 742e 6367 6929 2e20 426c 6173 7420 7072  t.cgi). Blast pr
+000006c0: 6f76 6964 6573 2061 2072 6f62 7573 7420  ovides a robust 
+000006d0: 636f 6d6d 616e 6420 6c69 6e65 2069 6e74  command line int
+000006e0: 6572 6661 6365 2066 6f72 2063 6f6e 7374  erface for const
+000006f0: 7275 6374 696e 6720 616e 6420 7573 696e  ructing and usin
+00000700: 6720 6461 7461 6261 7365 7320 666f 7220  g databases for 
+00000710: 7369 6d69 6c61 7269 7479 2073 6561 7263  similarity searc
+00000720: 6869 6e67 2061 6e64 2069 7320 7562 6971  hing and is ubiq
+00000730: 7569 746f 7573 2e20 5468 6572 6520 6172  uitous. There ar
+00000740: 6520 6d61 6e79 2074 7970 696e 6720 6170  e many typing ap
+00000750: 706c 6963 6174 696f 6e73 2077 6865 7265  plications where
+00000760: 2063 7573 746f 6d20 636f 6465 2069 7320   custom code is 
+00000770: 7772 6974 7465 6e20 6172 6f75 6e64 2074  written around t
+00000780: 6865 2062 6c61 7374 2063 6f6d 6d61 6e64  he blast command
+00000790: 206c 696e 6520 696e 7465 7266 6163 6520   line interface 
+000007a0: 746f 2070 6572 666f 726d 2073 6561 7263  to perform searc
+000007b0: 6865 7320 666f 7220 7661 7269 6f75 7320  hes for various 
+000007c0: 646f 776e 7374 7265 616d 2061 7070 6c69  downstream appli
+000007d0: 6361 7469 6f6e 732e 2046 6f72 2069 6e73  cations. For ins
+000007e0: 7461 6e63 652c 2074 6865 2069 6465 6e74  tance, the ident
+000007f0: 6966 6963 6174 696f 6e20 6f66 2073 7065  ification of spe
+00000800: 6369 6669 6320 7461 7267 6574 2073 6571  cific target seq
+00000810: 7565 6e63 6573 2077 6974 6869 6e20 616e  uences within an
+00000820: 2061 7373 656d 626c 7920 746f 2070 6572   assembly to per
+00000830: 666f 726d 2067 656e 652d 6279 2d67 656e  form gene-by-gen
+00000840: 6520 7068 796c 6f67 656e 6574 6963 2061  e phylogenetic a
+00000850: 6e61 6c79 7369 7320 284d 4c53 542c 2063  nalysis (MLST, c
+00000860: 674d 4c53 542c 2077 674d 4c53 5429 2c20  gMLST, wgMLST), 
+00000870: 616e 7469 6d69 6372 6f62 6961 6c20 7265  antimicrobial re
+00000880: 7369 7374 616e 6365 2067 656e 6520 6465  sistance gene de
+00000890: 7465 6374 696f 6e2c 2076 6972 756c 656e  tection, virulen
+000008a0: 6365 2067 656e 6520 6465 7465 6374 696f  ce gene detectio
+000008b0: 6e2c 2061 6e64 2069 6e20 7369 6c69 636f  n, and in silico
+000008c0: 2070 7265 6469 6374 696f 6e73 206f 6620   predictions of 
+000008d0: 7068 656e 6f74 7970 6573 2073 7563 6820  phenotypes such 
+000008e0: 6173 2073 6572 6f74 7970 6520 6973 2061  as serotype is a
+000008f0: 6e20 696d 706f 7274 616e 7420 6170 706c  n important appl
+00000900: 6963 6174 696f 6e20 7769 7468 696e 2070  ication within p
+00000910: 7562 6c69 6320 6865 616c 7468 2e20 5468  ublic health. Th
+00000920: 6520 7479 7069 6361 6c20 6170 7072 6f61  e typical approa
+00000930: 6368 2069 7320 6275 6e64 6c69 6e67 2074  ch is bundling t
+00000940: 6865 2073 6561 7263 682d 6261 7365 6420  he search-based 
+00000950: 6c6f 6769 6320 7769 7468 2061 6464 6974  logic with addit
+00000960: 696f 6e61 6c20 7370 6563 6961 6c69 7a65  ional specialize
+00000970: 6420 6c6f 6769 6320 746f 2070 6572 666f  d logic to perfo
+00000980: 726d 2074 6865 2064 6573 6972 6564 2061  rm the desired a
+00000990: 6e61 6c79 7369 732e 0d0a 0d0a 4465 6365  nalysis.....Dece
+000009a0: 6e74 7261 6c69 7a65 6420 616c 6c65 6c65  ntralized allele
+000009b0: 2063 616c 6c69 6e67 2068 6173 2062 6563   calling has bec
+000009c0: 6f6d 6520 6120 7072 6573 7369 6e67 2063  ome a pressing c
+000009d0: 6f6e 6365 726e 2066 6f72 2070 7562 6c69  oncern for publi
+000009e0: 6320 6865 616c 7468 206c 6162 6f72 6174  c health laborat
+000009f0: 6f72 6965 7320 6475 6520 746f 2074 6865  ories due to the
+00000a00: 2069 6e63 7265 6173 6564 2075 7365 206f   increased use o
+00000a10: 6620 7768 6f6c 6520 6765 6e6f 6d65 2073  f whole genome s
+00000a20: 6571 7565 6e63 696e 6720 2857 4753 2920  equencing (WGS) 
+00000a30: 666f 7220 6f75 7462 7265 616b 2064 6574  for outbreak det
+00000a40: 6563 7469 6f6e 2061 6e64 2073 7572 7665  ection and surve
+00000a50: 696c 6c61 6e63 6520 6f66 2076 6172 696f  illance of vario
+00000a60: 7573 2070 6174 686f 6765 6e73 2e20 4765  us pathogens. Ge
+00000a70: 6e65 2d62 792d 6765 6e65 2061 7070 726f  ne-by-gene appro
+00000a80: 6163 6865 7320 6861 7665 2061 2076 6172  aches have a var
+00000a90: 6965 7479 206f 6620 6265 6e65 6669 7473  iety of benefits
+00000aa0: 2066 6f72 2073 7065 6369 6573 2074 7970   for species typ
+00000ab0: 696e 672c 2069 6e63 6c75 6469 6e67 2061  ing, including a
+00000ac0: 2073 7461 6e64 6172 6469 7a65 6420 7365   standardized se
+00000ad0: 7420 6f66 206c 6f63 6920 666f 7220 6573  t of loci for es
+00000ae0: 7469 6d61 7469 6e67 2067 656e 6574 6963  timating genetic
+00000af0: 2073 696d 696c 6172 6974 7920 6265 7477   similarity betw
+00000b00: 6565 6e20 7361 6d70 6c65 732e 2054 6869  een samples. Thi
+00000b10: 7320 7374 616e 6461 7264 697a 6174 696f  s standardizatio
+00000b20: 6e20 616c 6c6f 7773 2066 6f72 2069 6e74  n allows for int
+00000b30: 6572 6f70 6572 6162 696c 6974 7920 6265  eroperability be
+00000b40: 7477 6565 6e20 6469 6666 6572 656e 7420  tween different 
+00000b50: 6772 6f75 7073 2e20 416c 736f 2c20 6974  groups. Also, it
+00000b60: 2068 6173 2074 6865 2062 656e 6566 6974   has the benefit
+00000b70: 206f 6620 636f 6d70 7265 7373 696f 6e2c   of compression,
+00000b80: 2073 696d 706c 6966 7969 6e67 2067 656e   simplifying gen
+00000b90: 6574 6963 2063 6f6d 7061 7269 736f 6e73  etic comparisons
+00000ba0: 2062 7920 7573 696e 6720 6120 7369 6d70   by using a simp
+00000bb0: 6c65 2068 616d 6d69 6e67 2064 6973 7461  le hamming dista
+00000bc0: 6e63 6520 6261 7365 6420 6f6e 2061 6c6c  nce based on all
+00000bd0: 656c 6520 6964 656e 7469 6669 6572 7320  ele identifiers 
+00000be0: 696e 7374 6561 6420 6f66 2061 2077 686f  instead of a who
+00000bf0: 6c65 2073 6571 7565 6e63 652e 2048 6f77  le sequence. How
+00000c00: 6576 6572 2c20 6120 6c69 6d69 7461 7469  ever, a limitati
+00000c10: 6f6e 206f 6620 7468 6973 2061 7070 726f  on of this appro
+00000c20: 6163 6820 6973 2074 6865 2072 6571 7569  ach is the requi
+00000c30: 7265 6d65 6e74 206f 6620 6120 6365 6e74  rement of a cent
+00000c40: 7261 6c69 7a65 6420 6175 7468 6f72 6974  ralized authorit
+00000c50: 7920 746f 2069 7373 7565 2075 6e69 7175  y to issue uniqu
+00000c60: 6520 616c 6c65 6c65 2069 6465 6e74 6966  e allele identif
+00000c70: 6965 7273 2c20 7768 6963 6820 706f 7365  iers, which pose
+00000c80: 7320 6d75 6c74 6970 6c65 206f 7065 7261  s multiple opera
+00000c90: 7469 6f6e 616c 2070 726f 626c 656d 732c  tional problems,
+00000ca0: 2073 7563 6820 6173 2070 7269 7661 6379   such as privacy
+00000cb0: 2061 6e64 2063 6f6e 6e65 6374 6976 6974   and connectivit
+00000cc0: 792e 2044 6573 7069 7465 2074 6869 7320  y. Despite this 
+00000cd0: 6c69 6d69 7461 7469 6f6e 2c20 5075 6c73  limitation, Puls
+00000ce0: 654e 6574 2049 6e74 6572 6e61 7469 6f6e  eNet Internation
+00000cf0: 616c 2068 6173 2061 646f 7074 6564 2067  al has adopted g
+00000d00: 656e 652d 6279 2d67 656e 6520 616e 616c  ene-by-gene anal
+00000d10: 7973 6973 2061 7320 6974 7320 7072 6566  ysis as its pref
+00000d20: 6572 7265 6420 616e 616c 7974 6963 616c  erred analytical
+00000d30: 2061 7070 726f 6163 6820 666f 7220 6573   approach for es
+00000d40: 7469 6d61 7469 6e67 2067 656e 6574 6963  timating genetic
+00000d50: 2073 696d 696c 6172 6974 7920 6265 7477   similarity betw
+00000d60: 6565 6e20 7361 6d70 6c65 7320 666f 7220  een samples for 
+00000d70: 726f 7574 696e 6520 6f70 6572 6174 696f  routine operatio
+00000d80: 6e73 2c20 7769 7468 2074 6865 206c 696d  ns, with the lim
+00000d90: 6974 6174 696f 6e20 7468 6174 2063 6f6d  itation that com
+00000da0: 7061 7269 6e67 2062 6574 7765 656e 206a  paring between j
+00000db0: 7572 6973 6469 6374 696f 6e73 2072 6571  urisdictions req
+00000dc0: 7569 7265 7320 7468 6520 7368 6172 696e  uires the sharin
+00000dd0: 6720 6f66 2074 6865 2070 7269 6d61 7279  g of the primary
+00000de0: 2073 6571 7565 6e63 6520 6461 7461 2072   sequence data r
+00000df0: 6174 6865 7220 7468 616e 2074 6865 2061  ather than the a
+00000e00: 6c6c 656c 6520 6964 656e 7469 6669 6572  llele identifier
+00000e10: 732e 0d0a 0d0a 496e 2072 6563 656e 7420  s.....In recent 
+00000e20: 7965 6172 732c 2074 6865 2063 6f6e 6365  years, the conce
+00000e30: 7074 206f 6620 7573 696e 6720 6372 7970  pt of using cryp
+00000e40: 746f 6772 6170 6869 6320 6861 7368 6573  tographic hashes
+00000e50: 206f 6620 7468 6520 616c 6c65 6c65 2073   of the allele s
+00000e60: 6571 7565 6e63 6520 6974 7365 6c66 2068  equence itself h
+00000e70: 6173 2067 6169 6e65 6420 7472 6163 7469  as gained tracti
+00000e80: 6f6e 2069 6e20 7661 7269 6f75 7320 616c  on in various al
+00000e90: 6c65 6c65 2d63 616c 6c69 6e67 2073 6f66  lele-calling sof
+00000ea0: 7477 6172 652c 2073 7563 6820 6173 205b  tware, such as [
+00000eb0: 4368 6577 6262 6163 615d 2868 7474 7073  Chewbbaca](https
+00000ec0: 3a2f 2f67 6974 6875 622e 636f 6d2f 422d  ://github.com/B-
+00000ed0: 554d 4d49 2f63 6865 7742 4241 4341 292c  UMMI/chewBBACA),
+00000ee0: 2074 6f20 7072 6f76 6964 6520 6465 6365   to provide dece
+00000ef0: 6e74 7261 6c69 7a65 6420 616c 6c65 6c65  ntralized allele
+00000f00: 2069 6465 6e74 6966 6965 7273 2e20 4861   identifiers. Ha
+00000f10: 7368 696e 6720 7468 6520 7365 7175 656e  shing the sequen
+00000f20: 6365 2079 6965 6c64 7320 6120 6465 7465  ce yields a dete
+00000f30: 726d 696e 6973 7420 616e 6420 6669 7865  rminist and fixe
+00000f40: 642d 7369 7a65 2068 6173 6820 7661 6c75  d-size hash valu
+00000f50: 652c 2077 6869 6368 2063 616e 2062 6520  e, which can be 
+00000f60: 636f 6d70 6172 6564 2069 6e20 7468 6520  compared in the 
+00000f70: 7361 6d65 206d 616e 6e65 7220 6173 2069  same manner as i
+00000f80: 6e74 6567 6572 732e 2054 6865 7265 2061  ntegers. There a
+00000f90: 7265 206e 756d 6572 6f75 7320 6861 7368  re numerous hash
+00000fa0: 2066 756e 6374 696f 6e73 2077 6974 6820   functions with 
+00000fb0: 6469 6666 6572 656e 7420 7374 7265 6e67  different streng
+00000fc0: 7468 7320 616e 6420 7765 616b 6e65 7373  ths and weakness
+00000fd0: 6573 2c20 6275 7420 4d44 3520 6469 6765  es, but MD5 dige
+00000fe0: 7374 7320 6861 7665 2062 6565 6e20 6272  sts have been br
+00000ff0: 6f61 646c 7920 6164 6f70 7465 6420 696e  oadly adopted in
+00001000: 2074 6865 2073 6f66 7477 6172 6520 636f   the software co
+00001010: 6d6d 756e 6974 792e 2054 6865 7920 6172  mmunity. They ar
+00001020: 6520 726f 7574 696e 656c 7920 7573 6564  e routinely used
+00001030: 2074 6f20 6173 7375 7265 2074 6861 7420   to assure that 
+00001040: 6120 7472 616e 7366 6572 7265 6420 6669  a transferred fi
+00001050: 6c65 2068 6173 2061 7272 6976 6564 2069  le has arrived i
+00001060: 6e74 6163 742e 2054 6865 2063 686f 6963  ntact. The choic
+00001070: 6520 6f66 206d 6435 2068 6173 6820 7072  e of md5 hash pr
+00001080: 6f76 6964 6573 2031 365e 3332 2c20 706f  ovides 16^32, po
+00001090: 7373 6962 6c65 2068 6173 6865 732e 2054  ssible hashes. T
+000010a0: 6865 7265 2069 7320 6120 7468 656f 7265  here is a theore
+000010b0: 7469 6361 6c20 6368 616e 6365 206f 6620  tical chance of 
+000010c0: 6861 7368 2063 6f6c 6c69 7369 6f6e 732c  hash collisions,
+000010d0: 2069 2e65 2e2c 2064 6966 6665 7265 6e74   i.e., different
+000010e0: 2073 6571 7565 6e63 6573 2072 6573 756c   sequences resul
+000010f0: 7469 6e67 2069 6e20 7468 6520 7361 6d65  ting in the same
+00001100: 2068 6173 682e 2048 6f77 6576 6572 2c20   hash. However, 
+00001110: 6173 2074 6865 206e 756d 6265 7220 6f66  as the number of
+00001120: 2061 6c6c 656c 6520 7365 7175 656e 6365   allele sequence
+00001130: 7320 666f 7220 6561 6368 2067 656e 6520  s for each gene 
+00001140: 696e 2064 6174 6162 6173 6573 2069 7320  in databases is 
+00001150: 7265 6c61 7469 7665 6c79 206c 6f77 2c20  relatively low, 
+00001160: 7468 6973 2073 686f 756c 6420 6265 2075  this should be u
+00001170: 6e63 6f6d 6d6f 6e2e 2049 6e20 7468 6973  ncommon. In this
+00001180: 2063 6173 652c 2063 6f6c 6c69 7369 6f6e   case, collision
+00001190: 7320 776f 756c 6420 7265 7375 6c74 2069  s would result i
+000011a0: 6e20 7072 6f66 696c 6573 2061 7070 6561  n profiles appea
+000011b0: 7269 6e67 206d 6f72 6520 7369 6d69 6c61  ring more simila
+000011c0: 7220 7468 616e 2074 6865 7920 6172 6520  r than they are 
+000011d0: 6174 2074 6865 2073 6571 7565 6e63 6520  at the sequence 
+000011e0: 6c65 7665 6c2e 2049 6e20 6164 6469 7469  level. In additi
+000011f0: 6f6e 2c20 7468 6520 6368 616e 6365 7320  on, the chances 
+00001200: 6f66 206d 756c 7469 706c 6520 6f63 6375  of multiple occu
+00001210: 7272 656e 6365 7320 6f66 2063 6f6c 6c69  rrences of colli
+00001220: 7369 6f6e 7320 7769 7468 696e 2061 2070  sions within a p
+00001230: 726f 6669 6c65 2077 6f75 6c64 2062 6520  rofile would be 
+00001240: 696e 6669 6e69 7465 6c79 2073 6d61 6c6c  infinitely small
+00001250: 2e0d 0a0d 0a54 6865 206d 6f74 6976 6174  .....The motivat
+00001260: 696f 6e20 666f 7220 6465 7665 6c6f 7069  ion for developi
+00001270: 6e67 206c 6f63 6964 6578 2069 7320 7468  ng locidex is th
+00001280: 6520 6e65 6564 2066 6f72 2061 2063 6f6d  e need for a com
+00001290: 6d6f 6e20 7365 6172 6368 2065 6e67 696e  mon search engin
+000012a0: 6520 666f 7220 7661 7269 6f75 7320 6c6f  e for various lo
+000012b0: 6369 2d62 6173 6564 2074 7970 696e 6720  ci-based typing 
+000012c0: 6170 706c 6963 6174 696f 6e73 2073 7563  applications suc
+000012d0: 6820 6173 2067 656e 652d 6279 2d67 656e  h as gene-by-gen
+000012e0: 6520 284d 4c53 542c 2020 6367 4d4c 5354  e (MLST,  cgMLST
+000012f0: 2c20 7767 4d4c 5354 2c20 724d 4c53 5429  , wgMLST, rMLST)
+00001300: 2c20 696e 2073 696c 6963 6f20 7365 726f  , in silico sero
+00001310: 7479 7069 6e67 2c20 6765 6e65 2d62 6173  typing, gene-bas
+00001320: 6564 2070 6865 6e6f 7479 7065 2070 7265  ed phenotype pre
+00001330: 6469 6374 696f 6e73 2028 616d 722c 2076  dictions (amr, v
+00001340: 6972 756c 656e 6365 2c20 7061 7468 6f74  irulence, pathot
+00001350: 7970 652c 2074 6f78 696e 2074 7970 696e  ype, toxin typin
+00001360: 6729 2c20 6d61 726b 6572 2d62 6173 6564  g), marker-based
+00001370: 2074 7970 696e 6720 2831 3653 292e 2054   typing (16S). T
+00001380: 6865 2074 6f6f 6c20 6d75 7374 2070 726f  he tool must pro
+00001390: 7669 6465 2063 7573 746f 6d20 6372 6974  vide custom crit
+000013a0: 6572 6961 2066 696c 7465 7269 6e67 2062  eria filtering b
+000013b0: 7920 6c6f 6369 2061 6e64 2070 726f 6475  y loci and produ
+000013c0: 6365 206d 756c 7469 706c 6520 666f 726d  ce multiple form
+000013d0: 6174 7320 666f 7220 646f 776e 7374 7265  ats for downstre
+000013e0: 616d 2061 7070 6c69 6361 7469 6f6e 732e  am applications.
+000013f0: 2049 7420 6d75 7374 2062 6520 636f 6d70   It must be comp
+00001400: 6174 6962 6c65 2077 6974 6820 616e 2048  atible with an H
+00001410: 5043 2065 6e76 6972 6f6e 6d65 6e74 2061  PC environment a
+00001420: 6e64 206e 6f74 2065 6e63 6f75 6e74 6572  nd not encounter
+00001430: 206c 6f63 6b69 6e67 2069 7373 7565 7320   locking issues 
+00001440: 7768 6572 6520 6d75 6c74 6970 6c65 2070  where multiple p
+00001450: 726f 6365 7373 6573 206d 6179 2074 7279  rocesses may try
+00001460: 2074 6f20 6368 616e 6765 2074 6865 2064   to change the d
+00001470: 6174 6120 7369 6d75 6c74 616e 656f 7573  ata simultaneous
+00001480: 6c79 2e20 4974 2073 686f 756c 6420 7072  ly. It should pr
+00001490: 6f76 6964 6520 696e 7075 7420 7365 7175  ovide input sequ
+000014a0: 656e 6365 2064 6174 6120 666c 6578 6962  ence data flexib
+000014b0: 696c 6974 7920 746f 2075 7365 7220 7768  ility to user wh
+000014c0: 6963 6820 696e 636c 7564 6573 2073 7570  ich includes sup
+000014d0: 706f 7274 2066 6f72 2031 2920 6578 6973  port for 1) exis
+000014e0: 7469 6e67 2073 6571 7565 6e63 6520 616e  ting sequence an
+000014f0: 6e6f 7461 7469 6f6e 7320 3229 2064 6520  notations 2) de 
+00001500: 6e6f 766f 2061 6e6e 6f74 6174 696f 6e73  novo annotations
+00001510: 2062 6173 6564 206f 6e20 636f 6e74 6967   based on contig
+00001520: 2069 6e70 7574 2033 2920 6361 7061 626c   input 3) capabl
+00001530: 6520 6f66 2065 7874 7261 6374 696e 6720  e of extracting 
+00001540: 7365 7175 656e 6365 2072 6567 696f 6e73  sequence regions
+00001550: 206f 6620 696e 7465 7265 7374 2e20 5468   of interest. Th
+00001560: 6520 6c6f 6769 6320 666f 7220 616c 6c65  e logic for alle
+00001570: 6c65 2063 616c 6c69 6e67 2069 7320 6772  le calling is gr
+00001580: 6561 746c 7920 7369 6d70 6c69 6669 6564  eatly simplified
+00001590: 2062 7920 6c65 7665 7261 6769 6e67 2065   by leveraging e
+000015a0: 7869 7374 696e 6720 616e 6e6f 7461 7469  xisting annotati
+000015b0: 6f6e 7320 6672 6f6d 2074 6f6f 6c73 2073  ons from tools s
+000015c0: 7563 6820 6173 205b 7072 6f64 6967 616c  uch as [prodigal
+000015d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000015e0: 2e63 6f6d 2f68 7961 7474 7064 2f50 726f  .com/hyattpd/Pro
+000015f0: 6469 6761 6c29 2c20 5b70 726f 6b6b 615d  digal), [prokka]
+00001600: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001610: 636f 6d2f 7473 6565 6d61 6e6e 2f70 726f  com/tseemann/pro
+00001620: 6b6b 6129 2c20 5b62 616b 7461 5d28 6874  kka), [bakta](ht
+00001630: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001640: 2f6f 7363 6877 656e 6765 7273 2f62 616b  /oschwengers/bak
+00001650: 7461 2920 746f 2064 656c 696e 6561 7465  ta) to delineate
+00001660: 2074 6865 2062 6f75 6e64 6172 6965 7320   the boundaries 
+00001670: 6f66 2074 6865 2073 6571 7565 6e63 6573  of the sequences
+00001680: 2074 6f20 6265 2071 7565 7269 6564 2061   to be queried a
+00001690: 6e64 2068 6173 6865 6420 746f 2070 726f  nd hashed to pro
+000016a0: 6475 6365 2061 6c6c 656c 6520 6964 656e  duce allele iden
+000016b0: 7469 6669 6572 732e 2048 6f77 6576 6572  tifiers. However
+000016c0: 2c20 6e6f 7420 616c 6c20 6c6f 6369 2061  , not all loci a
+000016d0: 7265 2070 726f 7465 696e 2063 6f64 696e  re protein codin
+000016e0: 672c 2068 6176 6520 696e 636f 6e73 6973  g, have inconsis
+000016f0: 7465 6e74 2061 6e6e 6f74 6174 696f 6e73  tent annotations
+00001700: 2c20 6f72 2061 7265 206e 6f74 2061 2063  , or are not a c
+00001710: 6f6d 706c 6574 6520 4f46 522c 2061 6e64  omplete OFR, and
+00001720: 2073 6f20 4c6f 6369 6465 7820 6861 7320   so Locidex has 
+00001730: 6275 696c 7420 696e 2073 7570 706f 7274  built in support
+00001740: 2066 6f72 2065 7874 7261 6374 696e 6720   for extracting 
+00001750: 7265 6769 6f6e 7320 6f66 2069 6e74 6572  regions of inter
+00001760: 6573 7420 6672 6f6d 2061 2071 7565 7279  est from a query
+00001770: 2067 656e 6f6d 652e 2041 2063 6f6d 6d6f   genome. A commo
+00001780: 6e20 6973 7375 6520 696e 206d 6174 6368  n issue in match
+00001790: 696e 6720 6170 706c 6963 6174 696f 6e73  ing applications
+000017a0: 2069 7320 7468 6174 2072 616e 6765 7320   is that ranges 
+000017b0: 6f66 2069 6465 6e74 6974 7920 616e 6420  of identity and 
+000017c0: 636f 7665 7261 6765 2066 6f72 2061 206d  coverage for a m
+000017d0: 6174 6368 2077 696c 6c20 7661 7279 2062  atch will vary b
+000017e0: 7920 6c6f 6375 732e 2053 6f2c 206c 6f63  y locus. So, loc
+000017f0: 6964 6578 2062 7569 6c64 7320 636f 6e74  idex builds cont
+00001800: 726f 6c20 6f76 6572 2074 6865 7365 2061  rol over these a
+00001810: 7474 7269 6275 7465 7320 6174 2061 206c  ttributes at a l
+00001820: 6f63 7573 206c 6576 656c 2069 6e74 6f20  ocus level into 
+00001830: 6974 7320 6461 7461 6261 7365 2073 7472  its database str
+00001840: 7563 7475 7265 2c20 616c 6c6f 7769 6e67  ucture, allowing
+00001850: 2066 6f72 2068 6967 6820 7661 7269 6162   for high variab
+00001860: 696c 6974 7920 6461 7461 6261 7365 7320  ility databases 
+00001870: 746f 2062 6520 7573 6564 2077 6974 686f  to be used witho
+00001880: 7574 2063 7573 746f 6d20 6c6f 6769 6320  ut custom logic 
+00001890: 6265 696e 6720 6275 696c 7420 646f 776e  being built down
+000018a0: 7374 7265 616d 2e20 5468 6973 2069 7320  stream. This is 
+000018b0: 7061 7274 6963 756c 6172 6c79 2069 6d70  particularly imp
+000018c0: 6f72 7461 6e74 2077 6865 6e20 6c65 6e67  ortant when leng
+000018d0: 7468 7320 6f66 206c 6f63 6920 6361 6e20  ths of loci can 
+000018e0: 6578 6869 6269 7420 636f 6e73 6964 6572  exhibit consider
+000018f0: 6162 6c65 2076 6172 6961 6269 6c69 7479  able variability
+00001900: 2c20 6173 2069 7320 7468 6520 6361 7365  , as is the case
+00001910: 2066 6f72 2067 656e 6573 206f 6620 696e   for genes of in
+00001920: 7465 7265 7374 2069 6e20 7479 7069 6e67  terest in typing
+00001930: 2061 7070 6c69 6361 7469 6f6e 732e 2054   applications. T
+00001940: 6869 7320 7072 6f76 6964 6573 2067 7265  his provides gre
+00001950: 6174 6572 2066 6c65 7869 6269 6c69 7479  ater flexibility
+00001960: 2066 6f72 2074 6865 2064 6573 6967 6e61   for the designa
+00001970: 7469 6f6e 206f 6620 6964 6561 6c20 7468  tion of ideal th
+00001980: 7265 7368 6f6c 6473 2066 6f72 2061 2067  resholds for a g
+00001990: 6976 656e 2061 7070 6c69 6361 7469 6f6e  iven application
+000019a0: 2e20 486f 7765 7665 722c 2074 6865 7365  . However, these
+000019b0: 2076 616c 7565 7320 6361 6e20 6265 206f   values can be o
+000019c0: 7665 7272 6964 6465 6e20 7573 696e 6720  verridden using 
+000019d0: 7468 6520 7265 706f 7274 206d 6f64 756c  the report modul
+000019e0: 6520 6669 6c74 6572 696e 6720 7061 7261  e filtering para
+000019f0: 6d65 7465 7273 2061 6e64 2062 7920 6d6f  meters and by mo
+00001a00: 6469 6679 696e 6720 7468 6520 7661 6c75  difying the valu
+00001a10: 6573 2077 6974 6869 6e20 7468 6520 6461  es within the da
+00001a20: 7461 6261 7365 2e0d 0a0d 0a5b 4368 6577  tabase.....[Chew
+00001a30: 6262 6163 615d 2868 7474 7073 3a2f 2f67  bbaca](https://g
+00001a40: 6974 6875 622e 636f 6d2f 422d 554d 4d49  ithub.com/B-UMMI
+00001a50: 2f63 6865 7742 4241 4341 2920 6973 2061  /chewBBACA) is a
+00001a60: 6e20 6578 6365 6c6c 656e 7420 6368 6f69  n excellent choi
+00001a70: 6365 2066 6f72 2061 6e20 6f70 656e 2d73  ce for an open-s
+00001a80: 6f75 7263 6520 616c 6c65 6c65 2063 616c  ource allele cal
+00001a90: 6c65 7220 616e 6420 7072 6f76 6964 6573  ler and provides
+00001aa0: 206d 616e 7920 6164 7661 6e63 6564 2066   many advanced f
+00001ab0: 6561 7475 7265 7320 666f 7220 6465 7665  eatures for deve
+00001ac0: 6c6f 7069 6e67 2c20 6375 7261 7469 6e67  loping, curating
+00001ad0: 2061 6e64 2075 7369 6e67 2067 656e 652d   and using gene-
+00001ae0: 6279 2d67 656e 6520 7363 6865 6d65 732e  by-gene schemes.
+00001af0: 2049 7420 7072 6f76 6964 6573 2061 2067   It provides a g
+00001b00: 7265 6174 2064 6561 6c20 6f66 2061 6464  reat deal of add
+00001b10: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
+00001b20: 696f 6e20 7265 6761 7264 696e 6720 7061  ion regarding pa
+00001b30: 7274 6961 6c20 6765 6e65 2073 6571 7565  rtial gene seque
+00001b40: 6e63 6573 2e20 466f 7220 5226 4420 6170  nces. For R&D ap
+00001b50: 706c 6963 6174 696f 6e73 2c20 7468 6973  plications, this
+00001b60: 2066 756e 6374 696f 6e61 6c69 7479 2063   functionality c
+00001b70: 616e 2062 6520 6578 7472 656d 656c 7920  an be extremely 
+00001b80: 7573 6566 756c 2e20 486f 7765 7665 722c  useful. However,
+00001b90: 2066 6f72 2073 6f6d 6520 6f70 6572 6174   for some operat
+00001ba0: 696f 6e61 6c20 636f 6e74 6578 7473 2c20  ional contexts, 
+00001bb0: 7468 6520 6465 7369 676e 206f 6620 5b43  the design of [C
+00001bc0: 6865 7762 6261 6361 5d28 6874 7470 733a  hewbbaca](https:
+00001bd0: 2f2f 6769 7468 7562 2e63 6f6d 2f42 2d55  //github.com/B-U
+00001be0: 4d4d 492f 6368 6577 4242 4143 4129 2070  MMI/chewBBACA) p
+00001bf0: 726f 7669 6465 7320 756e 6465 7369 7261  rovides undesira
+00001c00: 626c 6520 696e 666f 726d 6174 696f 6e2c  ble information,
+00001c10: 2061 6e64 2061 7420 7072 6573 656e 742c   and at present,
+00001c20: 2069 7420 6861 7320 6973 7375 6573 2077   it has issues w
+00001c30: 6974 6820 6d75 6c74 6970 6c65 2069 6e73  ith multiple ins
+00001c40: 7461 6e63 6573 2075 7369 6e67 2074 6865  tances using the
+00001c50: 2073 616d 6520 6461 7461 6261 7365 2061   same database a
+00001c60: 7420 6f6e 6365 2077 6974 6820 6e6f 7665  t once with nove
+00001c70: 6c20 616c 6c65 6c65 2064 6574 6563 7469  l allele detecti
+00001c80: 6f6e 2065 6e61 626c 6564 2028 5b42 2d55  on enabled ([B-U
+00001c90: 4d4d 492f 6368 6577 4242 4143 4123 3136  MMI/chewBBACA#16
+00001ca0: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+00001cb0: 622e 636f 6d2f 422d 554d 4d49 2f63 6865  b.com/B-UMMI/che
+00001cc0: 7742 4241 4341 2f69 7373 7565 732f 3136  wBBACA/issues/16
+00001cd0: 3829 292e 204c 6f63 6964 6578 2069 7320  8)). Locidex is 
+00001ce0: 6d65 616e 7420 746f 2062 6520 6f70 7469  meant to be opti
+00001cf0: 6d69 7a65 6420 666f 7220 726f 7574 696e  mized for routin
+00001d00: 6520 6f70 6572 6174 696f 6e2d 6c65 7665  e operation-leve
+00001d10: 6c20 7365 6172 6368 696e 672e 2049 7420  l searching. It 
+00001d20: 6973 2068 656c 7066 756c 2074 6f20 7365  is helpful to se
+00001d30: 7420 6465 6661 756c 7420 7061 7261 6d65  t default parame
+00001d40: 7465 7273 2066 6f72 2074 6865 2075 7365  ters for the use
+00001d50: 7220 746f 2068 6176 6520 7265 7072 6f64  r to have reprod
+00001d60: 7563 6962 696c 6974 7920 616e 6420 666c  ucibility and fl
+00001d70: 6578 6962 696c 6974 7920 7768 656e 2061  exibility when a
+00001d80: 7070 6c79 696e 6720 6d75 6c74 6970 6c65  pplying multiple
+00001d90: 2066 696c 7465 7269 6e67 2070 6172 616d   filtering param
+00001da0: 6574 6572 7320 6f6e 2074 6865 2073 6571  eters on the seq
+00001db0: 7565 6e63 6520 7374 6f72 6520 6166 7465  uence store afte
+00001dc0: 7220 7468 6520 6661 6374 2e20 5468 6973  r the fact. This
+00001dd0: 2061 6c6c 6f77 7320 6578 706c 6f72 696e   allows explorin
+00001de0: 6720 6469 6666 6572 656e 7420 7468 7265  g different thre
+00001df0: 7368 6f6c 6473 2077 6974 686f 7574 2074  sholds without t
+00001e00: 6865 206e 6565 6420 746f 2072 6563 6f6d  he need to recom
+00001e10: 7075 7465 2062 6c61 7374 2073 6561 7263  pute blast searc
+00001e20: 6865 732e 2049 6e20 6164 6469 7469 6f6e  hes. In addition
+00001e30: 2c20 7468 6572 6520 6973 206f 6674 656e  , there is often
+00001e40: 2061 2064 6573 6972 6520 746f 2069 6e63   a desire to inc
+00001e50: 6c75 6465 2061 6464 6974 696f 6e61 6c20  lude additional 
+00001e60: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00001e70: 7420 6120 6769 7665 6e20 6c6f 6375 732c  t a given locus,
+00001e80: 2073 7563 6820 6173 2064 6966 6665 7265   such as differe
+00001e90: 6e74 2069 6465 6e74 6966 6965 7273 2c20  nt identifiers, 
+00001ea0: 6675 6e63 7469 6f6e 616c 2070 726f 7065  functional prope
+00001eb0: 7274 6965 732c 2061 6e64 2070 6865 6e6f  rties, and pheno
+00001ec0: 7479 7069 6320 6566 6665 6374 732e 2054  typic effects. T
+00001ed0: 6865 2064 6174 6162 6173 6520 666f 726d  he database form
+00001ee0: 6174 206f 6620 6c6f 6369 6465 7820 616c  at of locidex al
+00001ef0: 6c6f 7773 2074 6865 2069 6e63 6c75 7369  lows the inclusi
+00001f00: 6f6e 206f 6620 616e 7920 6e75 6d62 6572  on of any number
+00001f10: 206f 6620 6669 656c 6473 2062 756e 646c   of fields bundl
+00001f20: 6564 2069 6e74 6f20 6120 7365 6172 6368  ed into a search
+00001f30: 2072 6573 756c 7420 6f62 6a65 6374 2066   result object f
+00001f40: 6f72 2075 7365 7273 2074 6f20 6465 7363  or users to desc
+00001f50: 7269 6265 2074 6865 6972 2064 6174 6120  ribe their data 
+00001f60: 636f 6e76 656e 6965 6e74 6c79 2064 7572  conveniently dur
+00001f70: 696e 6720 646f 776e 7374 7265 616d 2061  ing downstream a
+00001f80: 6e61 6c79 7369 732e 2054 6869 7320 6675  nalysis. This fu
+00001f90: 6e63 7469 6f6e 616c 6974 7920 616c 6c6f  nctionality allo
+00001fa0: 7773 2066 6f72 2064 6966 6665 7265 6e74  ws for different
+00001fb0: 2064 6174 6120 7573 6520 6361 7365 7320   data use cases 
+00001fc0: 6672 6f6d 2061 2063 6f6d 6d6f 6e20 6461  from a common da
+00001fd0: 7461 2073 746f 7265 2e20 4c6f 6369 6465  ta store. Locide
+00001fe0: 7820 646f 6573 206e 6f74 2068 6176 6520  x does not have 
+00001ff0: 7468 6520 6675 6c6c 2066 6561 7475 7265  the full feature
+00002000: 7320 666f 7220 6120 6765 6e65 2d62 792d  s for a gene-by-
+00002010: 6765 6e65 2073 6f66 7477 6172 6520 7061  gene software pa
+00002020: 636b 6167 6520 6c69 6b65 205b 4368 6577  ckage like [Chew
+00002030: 6262 6163 615d 2868 7474 7073 3a2f 2f67  bbaca](https://g
+00002040: 6974 6875 622e 636f 6d2f 422d 554d 4d49  ithub.com/B-UMMI
+00002050: 2f63 6865 7742 4241 4341 2920 6275 7420  /chewBBACA) but 
+00002060: 6361 6e20 6265 2075 7365 6420 746f 2061  can be used to a
+00002070: 6368 6965 7665 2073 696d 696c 6172 2072  chieve similar r
+00002080: 6573 756c 7473 2077 6869 6c65 2062 6569  esults while bei
+00002090: 6e67 2061 206d 6f72 6520 6765 6e65 7269  ng a more generi
+000020a0: 6320 746f 6f6c 206b 6974 2066 6f72 2062  c tool kit for b
+000020b0: 6c61 7374 2073 6561 7263 6865 732c 2073  last searches, s
+000020c0: 696d 696c 6172 2074 6f20 5b61 6272 6963  imilar to [abric
+000020d0: 6174 655d 2868 7474 7073 3a2f 2f67 6974  ate](https://git
+000020e0: 6875 622e 636f 6d2f 7473 6565 6d61 6e6e  hub.com/tseemann
+000020f0: 2f61 6272 6963 6174 6529 2e0d 0a0d 0a23  /abricate).....#
+00002100: 2320 4369 7461 7469 6f6e 0d0a 0d0a 526f  # Citation....Ro
+00002110: 6265 7274 736f 6e2c 204a 616d 6573 2c20  bertson, James, 
+00002120: 5765 6c6c 732c 204d 6174 7468 6577 2c20  Wells, Matthew, 
+00002130: 4368 7269 7374 792d 4c79 6e6e 2c20 5065  Christy-Lynn, Pe
+00002140: 7465 7273 6f6e 2c20 4b79 7279 6c6f 2042  terson, Kyrylo B
+00002150: 6573 736f 6e6f 762c 2052 6569 6d65 722c  essonov, Reimer,
+00002160: 2041 6c65 6973 6861 2c20 5363 686f 6e66   Aleisha, Schonf
+00002170: 656c 642c 204a 7573 7469 6e2e 204c 4f43  eld, Justin. LOC
+00002180: 4944 4558 3a20 4469 7374 7269 6275 7465  IDEX: Distribute
+00002190: 6420 616c 6c65 6c65 2063 616c 6c69 6e67  d allele calling
+000021a0: 2065 6e67 696e 652e 2032 3032 342e 205b   engine. 2024. [
+000021b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000021c0: 6f6d 2f70 6861 632d 6e6d 6c2f 6c6f 6369  om/phac-nml/loci
+000021d0: 6465 785d 2868 7474 7073 3a2f 2f67 6974  dex](https://git
+000021e0: 6875 622e 636f 6d2f 7068 6163 2d6e 6d6c  hub.com/phac-nml
+000021f0: 2f6c 6f63 6964 6578 290d 0a23 2320 436f  /locidex)..## Co
+00002200: 6e74 6163 740d 0a0d 0a46 6f72 2061 6e79  ntact....For any
+00002210: 2071 7565 7374 696f 6e73 2c20 6973 7375   questions, issu
+00002220: 6573 206f 7220 636f 6d6d 656e 7473 2070  es or comments p
+00002230: 6c65 6173 6520 6d61 6b65 2061 2047 6974  lease make a Git
+00002240: 6875 6220 6973 7375 6520 6f72 2072 6561  hub issue or rea
+00002250: 6368 206f 7574 2074 6f20 5b2a 2a4a 616d  ch out to [**Jam
+00002260: 6573 2052 6f62 6572 7473 6f6e 2a2a 5d28  es Robertson**](
+00002270: 6a61 6d65 732e 726f 6265 7274 736f 6e40  james.robertson@
+00002280: 7068 6163 2d61 7370 632e 6763 2e63 6129  phac-aspc.gc.ca)
+00002290: 2e0d 0a0d 0a23 2049 6e73 7461 6c6c 0d0a  .....# Install..
+000022a0: 0d0a 496e 7374 616c 6c20 7468 6520 6c61  ..Install the la
+000022b0: 7465 7374 2072 656c 6561 7365 6420 7665  test released ve
+000022c0: 7273 696f 6e20 6672 6f6d 2063 6f6e 6461  rsion from conda
+000022d0: 3a0d 0a0d 0a20 2020 2020 2020 2063 6f6e  :....        con
+000022e0: 6461 2063 7265 6174 6520 2d63 2062 696f  da create -c bio
+000022f0: 636f 6e64 6120 2d63 2063 6f6e 6461 2d66  conda -c conda-f
+00002300: 6f72 6765 202d 6e20 6c6f 6369 6465 7820  orge -n locidex 
+00002310: 6c6f 6369 6465 780d 0a0d 0a49 6e73 7461  locidex....Insta
+00002320: 6c6c 2075 7369 6e67 2070 6970 3a0d 0a0d  ll using pip:...
+00002330: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
+00002340: 7461 6c6c 206c 6f63 6964 6578 0d0a 0d0a  tall locidex....
+00002350: 496e 7374 616c 6c20 7468 6520 6c61 7465  Install the late
+00002360: 7374 206d 6173 7465 7220 6272 616e 6368  st master branch
+00002370: 2076 6572 7369 6f6e 2064 6972 6563 746c   version directl
+00002380: 7920 6672 6f6d 2047 6974 6875 623a 0d0a  y from Github:..
+00002390: 0d0a 2020 2020 2020 2020 7069 7020 696e  ..        pip in
+000023a0: 7374 616c 6c20 6769 742b 6874 7470 733a  stall git+https:
+000023b0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6861  //github.com/pha
+000023c0: 632d 6e6d 6c2f 6c6f 6369 6465 782e 6769  c-nml/locidex.gi
+000023d0: 740d 0a0d 0a23 2323 2043 6f6d 7061 7469  t....### Compati
+000023e0: 6269 6c69 7479 0d0a 0d0a 5b4c 6973 7420  bility....[List 
+000023f0: 6f75 7420 4465 7065 6e64 656e 6369 6573  out Dependencies
+00002400: 2061 6e64 2f6f 7220 7061 636b 6167 6573   and/or packages
+00002410: 2061 7320 6170 7072 6f70 7269 6174 655d   as appropriate]
+00002420: 0d0a 0d0a 2320 4765 7474 696e 6720 5374  ....# Getting St
+00002430: 6172 7465 640d 0a0d 0a23 2320 5573 6167  arted....## Usag
+00002440: 650d 0a0d 0a09 096c 6f63 6964 6578 203c  e......locidex <
+00002450: 636f 6d6d 616e 643e 205b 6f70 7469 6f6e  command> [option
+00002460: 735d 203c 7265 7175 6972 6564 2061 7267  s] <required arg
+00002470: 756d 656e 7473 3e0d 0a0d 0a23 2323 2043  uments>....### C
+00002480: 6f6d 6d61 6e64 730d 0a0d 0a4c 6f63 6964  ommands....Locid
+00002490: 6578 2075 7365 7320 7468 6520 666f 6c6c  ex uses the foll
+000024a0: 6f77 696e 6720 636f 6d6d 616e 6473 3a0d  owing commands:.
+000024b0: 0a0d 0a31 2e20 2a2a 7365 6172 6368 2a2a  ...1. **search**
+000024c0: 202d 2071 7565 7279 2061 2073 6574 206f   - query a set o
+000024d0: 6620 4f52 4673 2c20 616e 6420 6765 6e65  f ORFs, and gene
+000024e0: 7320 6167 6169 6e73 7420 6120 6461 7461  s against a data
+000024f0: 6261 7365 2074 6f20 7072 6f64 7563 6520  base to produce 
+00002500: 6120 7365 7175 656e 6365 2073 746f 7265  a sequence store
+00002510: 2066 6f72 2064 6f77 6e73 7472 6561 6d20   for downstream 
+00002520: 7072 6f63 6573 7369 6e67 0d0a 322e 202a  processing..2. *
+00002530: 2a65 7874 7261 6374 2a2a 202d 2065 7874  *extract** - ext
+00002540: 7261 6374 206c 6f63 6920 6672 6f6d 2061  ract loci from a
+00002550: 2067 656e 6f6d 6520 6261 7365 6420 6f6e   genome based on
+00002560: 2061 206c 6f63 6964 6578 2064 6174 6162   a locidex datab
+00002570: 6173 650d 0a33 2e20 2a2a 7265 706f 7274  ase..3. **report
+00002580: 2a2a 202d 2066 696c 7465 7220 6120 7365  ** - filter a se
+00002590: 7175 656e 6365 2073 746f 7265 2061 6e64  quence store and
+000025a0: 2070 726f 6475 6365 2061 6e20 6578 7472   produce an extr
+000025b0: 6163 7420 6f66 2062 6c61 7374 2072 6573  act of blast res
+000025c0: 756c 7473 2061 6e64 2067 656e 6520 7072  ults and gene pr
+000025d0: 6f66 696c 6520 2861 6c6c 656c 6520 6361  ofile (allele ca
+000025e0: 6c6c 696e 6729 0d0a 342e 202a 2a6d 6572  lling)..4. **mer
+000025f0: 6765 2a2a 202d 206d 6572 6765 2061 2073  ge** - merge a s
+00002600: 6574 206f 6620 6765 6e65 2070 726f 6669  et of gene profi
+00002610: 6c65 7320 696e 746f 2061 2073 7461 6e64  les into a stand
+00002620: 6172 6420 2761 6c6c 656c 6527 2070 726f  ard 'allele' pro
+00002630: 6669 6c65 2066 6f72 6d61 740d 0a35 2e20  file format..5. 
+00002640: 2a2a 666f 726d 6174 2a2a 202d 2066 6f72  **format** - for
+00002650: 6d61 7420 6661 7374 6120 6669 6c65 7320  mat fasta files 
+00002660: 6672 6f6d 206f 7468 6572 204d 4c53 5420  from other MLST 
+00002670: 6461 7461 6261 7365 7320 666f 7220 7573  databases for us
+00002680: 6520 7769 7468 206c 6f63 6964 6578 2062  e with locidex b
+00002690: 7569 6c64 0d0a 362e 202a 2a62 7569 6c64  uild..6. **build
+000026a0: 2a2a 202d 2062 7569 6c64 7320 6120 6c6f  ** - builds a lo
+000026b0: 6369 6465 7820 6461 7461 6273 650d 0a0d  cidex databse...
+000026c0: 0a23 2320 436f 6e66 6967 7572 6174 696f  .## Configuratio
+000026d0: 6e20 616e 6420 5365 7474 696e 6773 0d0a  n and Settings..
+000026e0: 0d0a 4c6f 6369 6465 7820 6973 2064 6573  ..Locidex is des
+000026f0: 6967 6e65 6420 746f 2062 6520 7665 7279  igned to be very
+00002700: 206d 6f64 756c 6172 2073 6f20 7468 6174   modular so that
+00002710: 2064 6576 656c 6f70 6572 7320 616e 6420   developers and 
+00002720: 7573 6572 7320 6361 6e20 6d69 7820 616e  users can mix an
+00002730: 6420 6d61 7463 6820 6469 6666 6572 656e  d match differen
+00002740: 7420 636f 6d70 6f6e 656e 7473 2066 6f72  t components for
+00002750: 2074 6865 6972 2069 6e64 6976 6964 7561   their individua
+00002760: 6c20 676f 616c 732e 2045 6163 6820 746f  l goals. Each to
+00002770: 6f6c 2069 7320 6465 7369 676e 6564 2073  ol is designed s
+00002780: 6f20 7468 6174 2069 7420 6361 6e20 6265  o that it can be
+00002790: 2069 6d70 6f72 7465 6420 6173 2061 2070   imported as a p
+000027a0: 7974 686f 6e20 6c69 6272 6172 7920 746f  ython library to
+000027b0: 2065 7874 656e 6420 616e 6420 696d 706c   extend and impl
+000027c0: 656d 656e 7420 6375 7374 6f6d 2062 6568  ement custom beh
+000027d0: 6176 696f 7572 2e20 4120 6465 7363 7269  aviour. A descri
+000027e0: 7074 696f 6e20 6f66 2065 6163 6820 746f  ption of each to
+000027f0: 6f6c 2061 6e64 2069 7473 2069 6e70 7574  ol and its input
+00002800: 732f 6f75 7470 7574 7320 6973 2070 726f  s/outputs is pro
+00002810: 7669 6465 6420 6265 6c6f 772e 0d0a 0d0a  vided below.....
+00002820: 5468 6520 6265 6c6f 7720 6669 6775 7265  The below figure
+00002830: 2073 686f 7773 2061 2067 656e 6572 616c   shows a general
+00002840: 2077 6f72 6b66 6c6f 7720 666f 7220 6561   workflow for ea
+00002850: 6368 206f 6620 7468 6520 6c6f 6369 6465  ch of the locide
+00002860: 7820 636f 6d6d 616e 6473 3a0d 0a21 5b6c  x commands:..![l
+00002870: 6f63 6964 6578 2077 6f72 6b66 6c6f 7773  ocidex workflows
+00002880: 5d28 2f61 7373 6574 732f 6c6f 6369 6465  ](/assets/locide
+00002890: 785f 776f 726b 666c 6f77 5f6d 6572 6d61  x_workflow_merma
+000028a0: 6964 2d32 3032 3430 3331 382e 706e 6729  id-20240318.png)
+000028b0: 0d0a 0d0a 2323 2320 5365 6172 6368 0d0a  ....### Search..
+000028c0: 0d0a 5468 6520 7365 6172 6368 206d 6f64  ..The search mod
+000028d0: 756c 6520 6973 206d 6561 6e74 2074 6f20  ule is meant to 
+000028e0: 7573 6520 6c6f 6369 6465 7820 666f 726d  use locidex form
+000028f0: 6174 7465 6420 6461 7461 6261 7365 2064  atted database d
+00002900: 6972 6563 746f 7269 6573 2e20 0d0a 0d0a  irectories. ....
+00002910: 2d20 444e 4120 616e 6420 7072 6f74 6569  - DNA and protei
+00002920: 6e20 626c 6173 7420 7365 6172 6368 6573  n blast searches
+00002930: 0d0a 2d20 4d64 3520 6861 7368 696e 6720  ..- Md5 hashing 
+00002940: 6f66 2061 6c6c 656c 6573 0d0a 2d20 5374  of alleles..- St
+00002950: 6f72 6167 6520 6f66 2072 6573 756c 7473  orage of results
+00002960: 2066 6f72 2070 6f73 742d 7072 6f63 6573   for post-proces
+00002970: 7369 6e67 2069 6e20 6a73 6f6e 2066 6f72  sing in json for
+00002980: 6d61 740d 0a0d 0a47 656e 6520 616e 6e6f  mat....Gene anno
+00002990: 7461 7469 6f6e 2069 7320 6e6f 746f 7269  tation is notori
+000029a0: 6f75 736c 7920 696e 636f 6e73 6973 7465  ously inconsiste
+000029b0: 6e74 2062 6574 7765 656e 2064 6966 6665  nt between diffe
+000029c0: 7265 6e74 2073 6f66 7477 6172 6520 616e  rent software an
+000029d0: 6420 736f 2069 7420 6973 202a 2a53 5452  d so it is **STR
+000029e0: 4f4e 474c 592a 2a20 7265 636f 6d6d 656e  ONGLY** recommen
+000029f0: 6465 6420 746f 2075 7365 2074 6865 2073  ded to use the s
+00002a00: 616d 6520 6d65 7468 6f64 206f 6620 616e  ame method of an
+00002a10: 6e6f 7461 7469 6f6e 2066 6f72 2079 6f75  notation for you
+00002a20: 7220 6461 7461 6261 7365 2061 6e64 2077  r database and w
+00002a30: 6861 7420 796f 7520 7769 6c6c 2075 7365  hat you will use
+00002a40: 2074 6f20 7365 6172 6368 2e20 6965 2e20   to search. ie. 
+00002a50: 6966 2075 7369 6e67 2070 726f 6469 6761  if using prodiga
+00002a60: 6c20 666f 7220 7365 6172 6368 696e 672c  l for searching,
+00002a70: 2075 7365 2070 726f 6469 6761 6c20 666f   use prodigal fo
+00002a80: 7220 636f 6e73 7472 7563 7469 6e67 2074  r constructing t
+00002a90: 6865 2064 6174 6162 6173 652e 0d0a 0d0a  he database.....
+00002aa0: 4558 414d 504c 453a 2052 756e 2073 6561  EXAMPLE: Run sea
+00002ab0: 7263 6820 696e 2061 6e6e 6f74 6174 696f  rch in annotatio
+00002ac0: 6e20 6d6f 6465 2077 6974 6820 6120 6661  n mode with a fa
+00002ad0: 7374 6120 696e 7075 743a 0d0a 0d0a 0909  sta input:......
+00002ae0: 6c6f 6369 6465 7820 7365 6172 6368 202d  locidex search -
+00002af0: 7120 2e2f 6578 616d 706c 652f 7365 6172  q ./example/sear
+00002b00: 6368 2f4e 435f 3030 3331 3938 2e31 2e66  ch/NC_003198.1.f
+00002b10: 6173 7461 202d 6420 2e2f 6578 616d 706c  asta -d ./exampl
+00002b20: 652f 6275 696c 645f 6462 5f6d 6c73 745f  e/build_db_mlst_
+00002b30: 6f75 7420 2d6f 202e 2f65 7861 6d70 6c65  out -o ./example
+00002b40: 2f73 6561 7263 682f 4e43 5f30 3033 3139  /search/NC_00319
+00002b50: 385f 6661 7374 6120 2d6e 2038 202d 2d61  8_fasta -n 8 --a
+00002b60: 6e6e 6f74 6174 650d 0a0d 0a45 5841 4d50  nnotate....EXAMP
+00002b70: 4c45 3a20 5275 6e20 7365 6172 6368 2077  LE: Run search w
+00002b80: 6974 6820 6578 6973 7469 6e67 2061 6e6e  ith existing ann
+00002b90: 6f74 6174 696f 6e73 2069 6e20 4765 6e42  otations in GenB
+00002ba0: 616e 6b20 666f 726d 6174 3a0d 0a0d 0a09  ank format:.....
+00002bb0: 096c 6f63 6964 6578 2073 6561 7263 6820  .locidex search 
+00002bc0: 2d71 202e 2f65 7861 6d70 6c65 2f73 6561  -q ./example/sea
+00002bd0: 7263 682f 4e43 5f30 3033 3139 382e 312e  rch/NC_003198.1.
+00002be0: 6762 6b20 2d64 202e 2f65 7861 6d70 6c65  gbk -d ./example
+00002bf0: 2f62 7569 6c64 5f64 625f 6d6c 7374 5f6f  /build_db_mlst_o
+00002c00: 7574 202d 6f20 2e2f 6578 616d 706c 652f  ut -o ./example/
+00002c10: 7365 6172 6368 2f4e 435f 3030 3331 3938  search/NC_003198
+00002c20: 5f66 6173 7461 202d 6e20 380d 0a0d 0a23  _fasta -n 8....#
+00002c30: 2323 2320 496e 7075 740d 0a0d 0a41 6363  ### Input....Acc
+00002c40: 6570 7465 6420 696e 7075 7420 4461 7461  epted input Data
+00002c50: 2046 6f72 6d61 7473 3a20 4765 6e42 616e   Formats: GenBan
+00002c60: 6b2c 2046 6173 7461 2028 6f66 2069 6e64  k, Fasta (of ind
+00002c70: 6976 6964 7561 6c20 6c6f 6369 2073 6571  ividual loci seq
+00002c80: 7565 6e63 6573 290d 0a0d 0a23 2323 2320  uences)....#### 
+00002c90: 4f75 7470 7574 0d0a 0d0a 6060 600d 0a7b  Output....```..{
+00002ca0: 6f75 7420 666f 6c64 6572 206e 616d 657d  out folder name}
+00002cb0: 0d0a e294 9ce2 9480 e294 8020 626c 6173  ........... blas
+00002cc0: 740d 0a20 20e2 949c e294 80e2 9480 206e  t..  ......... n
+00002cd0: 7563 6c65 6f74 6964 650d 0a20 2020 20e2  ucleotide..    .
+00002ce0: 949c e294 80e2 9480 2068 7370 732e 7478  ........ hsps.tx
+00002cf0: 7420 2020 2020 2020 200d 0a20 2020 20e2  t        ..    .
+00002d00: 9494 e294 80e2 9480 2071 7565 7269 6573  ........ queries
+00002d10: 2e66 6173 7461 0d0a 2020 e294 9ce2 9480  .fasta..  ......
+00002d20: e294 8020 7072 6f74 6569 6e0d 0a20 2020  ... protein..   
+00002d30: 20e2 949c e294 80e2 9480 2068 7370 732e   ......... hsps.
+00002d40: 7478 7420 2020 2020 2020 200d 0a20 2020  txt        ..   
+00002d50: 20e2 9494 e294 80e2 9480 2071 7565 7269   ......... queri
+00002d60: 6573 2e66 6173 7461 2020 2020 2020 0d0a  es.fasta      ..
+00002d70: e294 9ce2 9480 e294 8020 7365 715f 7374  ......... seq_st
+00002d80: 6f72 652e 6a73 6f6e 0d0a e294 94e2 9480  ore.json........
+00002d90: e294 8020 7265 7375 6c74 732e 6a73 6f6e  ... results.json
+00002da0: 2020 0d0a 6060 600d 0a0d 0a53 6565 2022    ..```....See "
+00002db0: 5365 7175 656e 6365 2053 746f 7265 2220  Sequence Store" 
+00002dc0: 666f 7220 6465 7363 7269 7074 696f 6e20  for description 
+00002dd0: 6f66 2074 6865 2073 6571 5f73 746f 7265  of the seq_store
+00002de0: 2e6a 736f 6e20 6f75 7470 7574 2066 696c  .json output fil
+00002df0: 650d 0a0d 0a23 2323 2045 7874 7261 6374  e....### Extract
+00002e00: 0d0a 0d0a 5468 6520 6578 7472 6163 7420  ....The extract 
+00002e10: 6d6f 6475 6c65 2069 7320 6d65 616e 7420  module is meant 
+00002e20: 746f 2075 7365 206c 6f63 6964 6578 2066  to use locidex f
+00002e30: 6f72 6d61 7474 6564 2064 6174 6162 6173  ormatted databas
+00002e40: 6520 6469 7265 6374 6f72 6965 7320 746f  e directories to
+00002e50: 2067 6574 2073 6571 7565 6e63 6573 206f   get sequences o
+00002e60: 6620 696e 6469 7669 6475 616c 206c 6f63  f individual loc
+00002e70: 6920 6261 7365 6420 6f6e 2061 206c 6f63  i based on a loc
+00002e80: 6964 6578 2066 6f72 6d61 7474 6564 2064  idex formatted d
+00002e90: 6174 6162 6173 652e 2054 6865 2065 7874  atabase. The ext
+00002ea0: 7261 6374 206d 6f64 756c 6520 6f70 6572  ract module oper
+00002eb0: 6174 6573 2069 6e20 666f 7572 2064 6966  ates in four dif
+00002ec0: 6665 7265 6e74 206d 6f64 6573 3a0d 0a0d  ferent modes:...
+00002ed0: 0a31 2920 7261 773a 2073 6571 7565 6e63  .1) raw: sequenc
+00002ee0: 6573 2061 7265 2064 6972 6563 746c 7920  es are directly 
+00002ef0: 6578 7472 6163 7465 6420 6672 6f6d 2074  extracted from t
+00002f00: 6865 2061 7373 656d 626c 7920 7769 7468  he assembly with
+00002f10: 206e 6f20 6675 7274 6865 7220 7072 6f63   no further proc
+00002f20: 6573 7369 6e67 2e0d 0a32 2920 7472 696d  essing...2) trim
+00002f30: 3a20 616e 7920 6c65 6164 696e 6720 6f72  : any leading or
+00002f40: 2074 7261 696c 696e 6720 6261 7365 7320   trailing bases 
+00002f50: 7768 6963 6820 6172 6520 6e6f 7420 7072  which are not pr
+00002f60: 6573 656e 7420 696e 2074 6865 2064 6220  esent in the db 
+00002f70: 6d61 7463 6820 6172 6520 7472 696d 6d65  match are trimme
+00002f80: 6420 6672 6f6d 2074 6865 2073 6571 7565  d from the seque
+00002f90: 6e63 652e 200d 0a33 2920 736e 703a 2054  nce. ..3) snp: T
+00002fa0: 6869 7320 7769 6c6c 2061 7070 6c79 206f  his will apply o
+00002fb0: 6e6c 7920 6e75 636c 656f 7469 6465 2076  nly nucleotide v
+00002fc0: 6172 6961 6e74 7320 746f 2074 6865 2072  ariants to the r
+00002fd0: 6566 6572 656e 6365 2061 6c6c 656c 6520  eference allele 
+00002fe0: 7768 6963 6820 6361 6e20 6265 2076 6572  which can be ver
+00002ff0: 7920 7573 6566 756c 2066 6f72 206e 616e  y useful for nan
+00003000: 6f70 6f72 6520 6173 7365 6d62 6c69 6573  opore assemblies
+00003010: 2077 6865 7265 2069 6e64 656c 7320 6172   where indels ar
+00003020: 6520 636f 6d6d 6f6e 2061 6e64 2075 6e6c  e common and unl
+00003030: 696b 656c 7920 746f 2062 6520 7265 616c  ikely to be real
+00003040: 2e20 0d0a 3429 2065 7874 656e 6420 3a20  . ..4) extend : 
+00003050: 5468 6973 206d 6f64 6520 7769 6c6c 2066  This mode will f
+00003060: 696c 6c20 696e 2061 6e79 2074 6572 6d69  ill in any termi
+00003070: 6e61 6c20 7365 7175 656e 6365 206d 6973  nal sequence mis
+00003080: 7369 6e67 2066 726f 6d20 7468 6520 7365  sing from the se
+00003090: 7175 656e 6365 2062 6173 6564 206f 6e20  quence based on 
+000030a0: 7468 6520 6d61 7463 6865 6420 7265 6665  the matched refe
+000030b0: 7265 6e63 6520 616c 6c65 6c65 2e0d 0a0d  rence allele....
+000030c0: 0a3e 205b 214e 6f74 655d 0d0a 3e20 4d6f  .> [!Note]..> Mo
+000030d0: 6465 7320 696e 766f 6c76 696e 6720 7072  des involving pr
+000030e0: 6f63 6573 7369 6e67 2028 7472 696d 2c20  ocessing (trim, 
+000030f0: 736e 7020 616e 6420 6578 7465 6e64 2920  snp and extend) 
+00003100: 696e 766f 6c76 6520 7061 6972 7769 7365  involve pairwise
+00003110: 206d 6166 6674 2061 6c69 676e 6d65 6e74   mafft alignment
+00003120: 206f 6620 7468 6520 6578 7472 6163 7465   of the extracte
+00003130: 6420 7365 7175 656e 6365 2077 6974 6820  d sequence with 
+00003140: 6974 7320 6265 7374 2062 6c61 7374 2068  its best blast h
+00003150: 6974 2069 6e20 7468 6520 6461 7461 6261  it in the databa
+00003160: 7365 2e0d 0a0d 0a21 5b65 7874 7261 6374  se.....![extract
+00003170: 2063 6f6d 6d61 6e64 206f 7074 696f 6e73   command options
+00003180: 5d28 2f61 7373 6574 732f 4c6f 6369 6465  ](/assets/Locide
+00003190: 7845 7874 7261 6374 2e70 6e67 290d 0a0d  xExtract.png)...
+000031a0: 0a23 2323 2320 496e 7075 740d 0a0d 0a49  .#### Input....I
+000031b0: 6e70 7574 2044 6174 6120 466f 726d 6174  nput Data Format
+000031c0: 733a 2046 6173 7461 2028 636f 6e74 6967  s: Fasta (contig
+000031d0: 7329 0d0a 0d0a 4765 6e65 2061 6e6e 6f74  s)....Gene annot
+000031e0: 6174 696f 6e20 6973 206e 6f74 6f72 696f  ation is notorio
+000031f0: 7573 6c79 2069 6e63 6f6e 7369 7374 656e  usly inconsisten
+00003200: 7420 6265 7477 6565 6e20 6469 6666 6572  t between differ
+00003210: 656e 7420 736f 6674 7761 7265 2c20 616e  ent software, an
+00003220: 6420 736f 2077 6520 696d 706c 656d 656e  d so we implemen
+00003230: 7465 6420 7468 6520 6578 7472 6163 7420  ted the extract 
+00003240: 6d6f 6475 6c65 2074 6f20 656e 6162 6c65  module to enable
+00003250: 2063 6f6e 7369 7374 656e 7420 7365 6c65   consistent sele
+00003260: 6374 696f 6e20 6f66 206c 6f63 6920 7365  ction of loci se
+00003270: 7175 656e 6365 7320 6672 6f6d 2061 6e20  quences from an 
+00003280: 696e 7075 7420 6765 6e6f 6d65 2e0d 0a0d  input genome....
+00003290: 0a45 5841 4d50 4c45 3a20 746f 2065 7874  .EXAMPLE: to ext
+000032a0: 7261 6374 206c 6f63 6920 7365 7175 656e  ract loci sequen
+000032b0: 6365 7320 6672 6f6d 2061 6e20 696e 7075  ces from an inpu
+000032c0: 7420 6765 6e6f 6d65 2c20 7265 706f 7274  t genome, report
+000032d0: 696e 6720 6a75 7374 2065 7874 7261 6374  ing just extract
+000032e0: 6564 2073 6571 7565 6e63 6573 2061 6e64  ed sequences and
+000032f0: 2073 6b69 7070 696e 6720 616e 7920 706f   skipping any po
+00003300: 7374 2070 726f 6365 7373 696e 6720 286d  st processing (m
+00003310: 6f64 653d 6072 6177 6029 0d0a 0d0a 0909  ode=`raw`)......
+00003320: 6c6f 6369 6465 7820 6578 7472 6163 7420  locidex extract 
+00003330: 2d2d 6d6f 6465 2072 6177 202d 6920 2e2f  --mode raw -i ./
+00003340: 6578 616d 706c 652f 7365 6172 6368 2f4e  example/search/N
+00003350: 435f 3030 3331 3938 2e31 2e66 6173 7461  C_003198.1.fasta
+00003360: 202d 6420 2e65 7861 6d70 6c65 2f62 7569   -d .example/bui
+00003370: 6c64 5f64 625f 6d6c 7374 5f6f 7574 202d  ld_db_mlst_out -
+00003380: 6f20 2e2f 6578 616d 706c 652f 7365 6172  o ./example/sear
+00003390: 6368 2f4e 435f 3030 3331 3938 5f66 6173  ch/NC_003198_fas
+000033a0: 7461 202d 6e20 3820 0d0a 0d0a 2323 2323  ta -n 8 ....####
+000033b0: 204f 7574 7075 740d 0a0d 0a60 6060 0d0a   Output....```..
+000033c0: 7b6f 7574 2066 6f6c 6465 7220 6e61 6d65  {out folder name
+000033d0: 7d0d 0ae2 949c e294 80e2 9480 2062 6c61  }........... bla
+000033e0: 7374 0d0a 2020 2020 e294 9ce2 9480 e294  st..    ........
+000033f0: 8020 6873 7073 2e74 7874 2020 2020 2020  . hsps.txt      
+00003400: 2020 0d0a e294 9ce2 9480 e294 8020 626c    ........... bl
+00003410: 6173 745f 6462 0d0a 2020 2020 e294 9ce2  ast_db..    ....
+00003420: 9480 e294 8020 636f 6e74 6967 732e 6661  ..... contigs.fa
+00003430: 7374 612e 6e64 6220 200d 0a20 2020 20e2  sta.ndb  ..    .
+00003440: 949c e294 80e2 9480 2063 6f6e 7469 6773  ........ contigs
+00003450: 2e66 6173 7461 2e6e 6872 0d0a 2020 2020  .fasta.nhr..    
+00003460: e294 9ce2 9480 e294 8020 636f 6e74 6967  ......... contig
+00003470: 732e 6661 7374 612e 6e69 6e20 0d0a 2020  s.fasta.nin ..  
+00003480: 2020 e294 9ce2 9480 e294 8020 636f 6e74    ......... cont
+00003490: 6967 732e 6661 7374 612e 6e6a 730d 0a20  igs.fasta.njs.. 
+000034a0: 2020 20e2 949c e294 80e2 9480 2063 6f6e     ......... con
+000034b0: 7469 6773 2e66 6173 7461 2e6e 6f74 0d0a  tigs.fasta.not..
+000034c0: 2020 2020 e294 9ce2 9480 e294 8020 636f      ......... co
+000034d0: 6e74 6967 732e 6661 7374 612e 6e73 710d  ntigs.fasta.nsq.
+000034e0: 0a20 2020 20e2 949c e294 80e2 9480 2063  .    ......... c
+000034f0: 6f6e 7469 6773 2e66 6173 7461 2e6e 7466  ontigs.fasta.ntf
+00003500: 0d0a 2020 2020 e294 94e2 9480 e294 8063  ..    .........c
+00003510: 6f6e 7469 6773 2e66 6173 7461 2e6e 746f  ontigs.fasta.nto
+00003520: 0d0a e294 9ce2 9480 e294 8020 6669 6c74  ........... filt
+00003530: 6572 6564 2e68 7370 732e 7478 740d 0ae2  ered.hsps.txt...
+00003540: 949c e294 80e2 9480 2070 726f 6365 7373  ........ process
+00003550: 6564 2e65 7874 7261 6374 6564 2e73 6571  ed.extracted.seq
+00003560: 732e 6661 7374 6120 236f 7074 696f 6e61  s.fasta #optiona
+00003570: 6c20 7365 7175 656e 6365 7320 7769 7468  l sequences with
+00003580: 2074 7269 6d6d 696e 672c 2067 6170 7020   trimming, gapp 
+00003590: 6669 6c6c 696e 6720 616e 2073 6e70 206f  filling an snp o
+000035a0: 6e6c 7920 6261 7365 6420 6f6e 206f 7074  nly based on opt
+000035b0: 696f 6e73 2073 656c 6563 7465 640d 0ae2  ions selected...
+000035c0: 949c e294 80e2 9480 2072 6177 2e65 7874  ........ raw.ext
+000035d0: 7261 6374 6564 2e73 6571 732e 6661 7374  racted.seqs.fast
+000035e0: 6120 2365 7861 6374 2065 7874 7261 6374  a #exact extract
+000035f0: 6564 2073 6571 7565 6e63 6573 0d0a e294  ed sequences....
+00003600: 94e2 9480 e294 8020 7265 7375 6c74 732e  ....... results.
+00003610: 6a73 6f6e 2020 0d0a 6060 600d 0a0d 0a23  json  ..```....#
+00003620: 2323 2052 6570 6f72 740d 0a0d 0a50 726f  ## Report....Pro
+00003630: 6475 6365 206c 6f63 6920 6861 7368 2070  duce loci hash p
+00003640: 726f 6669 6c65 7320 696e 206d 756c 7469  rofiles in multi
+00003650: 706c 6520 666f 726d 6174 7320 286a 736f  ple formats (jso
+00003660: 6e2c 2074 7376 2c20 7061 7271 7565 7429  n, tsv, parquet)
+00003670: 0d0a 0d0a 2d20 4669 6c74 6572 2072 6573  ....- Filter res
+00003680: 756c 7473 2062 6173 6564 206f 6e20 7573  ults based on us
+00003690: 6572 2063 7269 7465 7269 610d 0a2d 204d  er criteria..- M
+000036a0: 756c 7469 2d63 6f70 7920 6c6f 6369 2068  ulti-copy loci h
+000036b0: 616e 646c 696e 670d 0a0d 0a2a 2a4f 7074  andling....**Opt
+000036c0: 696f 6e61 6c3a 2a2a 2028 4e6f 7420 7265  ional:** (Not re
+000036d0: 7175 6972 6564 2066 6f72 204d 5650 2920  quired for MVP) 
+000036e0: 5072 6f64 7563 6520 636f 6e63 6174 656e  Produce concaten
+000036f0: 6174 6564 2066 6173 7461 2073 6571 7565  ated fasta seque
+00003700: 6e63 6573 2062 6173 6564 206f 6e20 616c  nces based on al
+00003710: 6c65 6c65 2070 726f 6669 6c65 730d 0a23  lele profiles..#
+00003720: 2323 2320 496e 7075 740d 0a0d 0a41 2053  ### Input....A S
+00003730: 6571 7565 6e63 6520 7374 6f72 6520 2860  equence store (`
+00003740: 7365 715f 7374 6f72 652e 6a73 6f6e 6029  seq_store.json`)
+00003750: 206f 626a 6563 7420 7072 6f64 7563 6564   object produced
+00003760: 2062 7920 7468 6520 2773 6561 7263 6827   by the 'search'
+00003770: 2066 756e 6374 696f 6e2e 0d0a 0d0a 0920   function...... 
+00003780: 2020 206c 6f63 6964 6578 2072 6570 6f72     locidex repor
+00003790: 7420 2d69 202e 6578 616d 706c 652f 7365  t -i .example/se
+000037a0: 6172 6368 2f73 6571 5f73 746f 7265 2e6a  arch/seq_store.j
+000037b0: 736f 6e20 2d6f 202e 2f65 7861 6d70 6c65  son -o ./example
+000037c0: 2f72 6570 6f72 745f 6f75 7420 2d2d 6e61  /report_out --na
+000037d0: 6d65 204e 435f 3030 3331 3938 0d0a 0d0a  me NC_003198....
+000037e0: 2323 2323 204f 7574 7075 740d 0a0d 0a5b  #### Output....[
+000037f0: 494e 5345 5254 2052 4550 4f52 5420 4f55  INSERT REPORT OU
+00003800: 5450 5554 5d0d 0a0d 0a23 2323 204d 6572  TPUT]....### Mer
+00003810: 6765 0d0a 0d0a 5265 6164 7320 616e 6420  ge....Reads and 
+00003820: 636f 6e63 6174 656e 6174 6573 2072 6570  concatenates rep
+00003830: 6f72 7420 6669 6c65 7320 696e 746f 2061  ort files into a
+00003840: 6e20 616c 6c65 6c65 2070 726f 6669 6c65  n allele profile
+00003850: 2069 6e20 5453 5620 666f 726d 6174 2e0d   in TSV format..
+00003860: 0a0d 0a23 2323 2320 496e 7075 740d 0a0d  ...#### Input...
+00003870: 0a43 616e 206c 6973 7420 7265 706f 7274  .Can list report
+00003880: 2066 696c 6573 206f 6e20 636f 6d6d 616e   files on comman
+00003890: 6420 6c69 6e65 206f 7220 7072 6f76 6964  d line or provid
+000038a0: 6520 6120 2766 696c 6520 6f66 2066 696c  e a 'file of fil
+000038b0: 6573 2720 2846 4f46 292e 2028 2767 7a27  es' (FOF). ('gz'
+000038c0: 2063 6f6d 7072 6573 7365 6420 616e 6420   compressed and 
+000038d0: 756e 636f 6d70 7265 7373 6564 2066 696c  uncompressed fil
+000038e0: 6573 2061 7265 2065 7863 6570 7465 6429  es are excepted)
+000038f0: 0d0a 0d0a 4558 414d 504c 453a 206d 6572  ....EXAMPLE: mer
+00003900: 6769 6e67 206d 756c 7469 706c 6520 6669  ging multiple fi
+00003910: 6c65 7320 7072 6f76 6964 6564 206f 6e20  les provided on 
+00003920: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
+00003930: 2074 6f20 2d69 0d0a 0d0a 0909 6c6f 6369   to -i......loci
+00003940: 6465 7820 6d65 7267 6520 2d69 202e 2f65  dex merge -i ./e
+00003950: 7861 6d70 6c65 2f6d 6572 6765 5f69 6e2f  xample/merge_in/
+00003960: 7072 6f66 696c 655f 312e 6a73 6f6e 202e  profile_1.json .
+00003970: 2f65 7861 6d70 6c65 2f6d 6572 6765 5f69  /example/merge_i
+00003980: 6e2f 7072 6f66 696c 655f 322e 6a73 6f6e  n/profile_2.json
+00003990: 2020 2d6f 202e 2f65 7861 6d70 6c65 2f6d    -o ./example/m
+000039a0: 6572 6765 5f6f 7574 2f0d 0a0d 0a45 5841  erge_out/....EXA
+000039b0: 4d50 4c45 3a20 6d65 7267 696e 6720 6669  MPLE: merging fi
+000039c0: 6c65 7320 7072 6f76 6964 6564 2074 6872  les provided thr
+000039d0: 6f75 6768 2061 206c 6973 7420 6f66 2070  ough a list of p
+000039e0: 6174 6873 2074 6f20 7265 706f 7274 2066  aths to report f
+000039f0: 696c 6573 0d0a 0d0a 0909 2020 6c6f 6369  iles......  loci
+00003a00: 6465 7820 6d65 7267 6520 2d69 202e 2f65  dex merge -i ./e
+00003a10: 7861 6d70 6c65 2f6d 6572 6765 5f69 6e2f  xample/merge_in/
+00003a20: 6669 6c65 5f6c 6973 742e 7478 7420 2e2f  file_list.txt ./
+00003a30: 6578 616d 706c 652f 6d65 7267 655f 6f75  example/merge_ou
+00003a40: 742f 200d 0a0d 0a23 2323 2320 4f75 7470  t/ ....#### Outp
+00003a50: 7574 0d0a 0d0a 6060 600d 0a7b 6f75 7420  ut....```..{out 
+00003a60: 666f 6c64 6572 206e 616d 657d 0d0a e294  folder name}....
+00003a70: 9ce2 9480 e294 8020 7072 6f66 696c 652e  ....... profile.
+00003a80: 7473 7620 2020 0d0a e294 94e2 9480 e294  tsv   ..........
+00003a90: 8020 7265 7375 6c74 732e 6a73 6f6e 2020  . results.json  
+00003aa0: 0d0a 6060 600d 0a0d 0a23 2323 2046 6f72  ..```....### For
+00003ab0: 6d61 740d 0a0d 0a54 616b 6573 2063 6f6d  mat....Takes com
+00003ac0: 6d6f 6e20 666f 726d 6174 7320 6f66 2067  mon formats of g
+00003ad0: 656e 652d 6279 2d67 656e 6520 6461 7461  ene-by-gene data
+00003ae0: 6261 7365 7320 616e 6420 666f 726d 6174  bases and format
+00003af0: 7320 7468 656d 2066 6f72 2075 7365 2077  s them for use w
+00003b00: 6974 6820 6c6f 6369 6465 7820 6275 696c  ith locidex buil
+00003b10: 6420 6d6f 6475 6c65 2e0d 0a0d 0a23 2323  d module.....###
+00003b20: 2320 496e 7075 740d 0a0d 0a41 6363 6570  # Input....Accep
+00003b30: 7473 2074 776f 2066 6f72 6d61 7473 2063  ts two formats c
+00003b40: 6f6d 6d6f 6e20 7769 7468 206d 6f73 7420  ommon with most 
+00003b50: 6f66 2074 6865 206d 616a 6f72 204d 4c53  of the major MLS
+00003b60: 5420 6461 7461 6261 7365 733a 0d0a 0d0a  T databases:....
+00003b70: 312e 2061 2064 6972 6563 746f 7279 206f  1. a directory o
+00003b80: 6620 6661 7374 6120 6669 6c65 733a 205b  f fasta files: [
+00003b90: 2266 6173 7461 222c 2266 6173 222c 2266  "fasta","fas","f
+00003ba0: 6122 2c22 6666 6e22 2c22 666e 6122 2c22  a","ffn","fna","
+00003bb0: 6661 7374 612e 677a 222c 2266 6173 2e67  fasta.gz","fas.g
+00003bc0: 7a22 2c22 6661 2e67 7a22 2c22 6666 6e2e  z","fa.gz","ffn.
+00003bd0: 677a 222c 2266 6e61 2e67 7a22 5d20 7769  gz","fna.gz"] wi
+00003be0: 7468 2022 6c6f 6375 7320 6e61 6d65 2220  th "locus name" 
+00003bf0: 6173 2074 6865 2066 696c 6520 6e61 6d65  as the file name
+00003c00: 2061 6e64 2061 6c6c 656c 6520 6964 2773   and allele id's
+00003c10: 2061 7265 2070 7265 7365 6e74 2069 6e20   are present in 
+00003c20: 7468 6520 6661 7374 6120 6865 6164 6572  the fasta header
+00003c30: 2073 6570 6172 6174 6564 2062 7920 616e   separated by an
+00003c40: 2075 6e64 6572 7363 6f72 652e 2069 652e   underscore. ie.
+00003c50: 2061 726f 4320 776f 756c 6420 6861 7665   aroC would have
+00003c60: 2074 6865 2066 696c 6520 6e61 6d65 2061   the file name a
+00003c70: 726f 432e 6661 7320 616e 6420 7468 6520  roC.fas and the 
+00003c80: 6865 6164 6572 206c 696e 6520 776f 756c  header line woul
+00003c90: 6420 6265 203e 6172 6f43 5f31 2e20 0d0a  d be >aroC_1. ..
+00003ca0: 322e 2061 2063 6f6e 6361 746f 6e61 7465  2. a concatonate
+00003cb0: 6420 6669 6c65 206f 6620 616c 6c20 6c6f  d file of all lo
+00003cc0: 6369 2069 6e20 6120 7369 6e67 6c65 2066  ci in a single f
+00003cd0: 6173 7461 2066 696c 6520 7768 6963 6820  asta file which 
+00003ce0: 6861 7320 7468 6520 6661 7374 6120 6465  has the fasta de
+00003cf0: 6620 6c69 6e65 2061 7320 603e 7b6c 6f63  f line as `>{loc
+00003d00: 7573 206e 616d 657d 5f7b 616c 6c65 6c65  us name}_{allele
+00003d10: 2069 647d 602e 2054 6865 7365 2074 776f   id}`. These two
+00003d20: 2066 6f72 6d61 7473 2061 7265 2063 6f6d   formats are com
+00003d30: 6d6f 6e20 7769 7468 206d 6f73 7420 6f66  mon with most of
+00003d40: 2074 6865 206d 616a 6f72 204d 4c53 5420   the major MLST 
+00003d50: 6461 7461 6261 7365 732e 0d0a 0d0a 0920  databases...... 
+00003d60: 2020 206c 6f63 6964 6578 2066 6f72 6d61     locidex forma
+00003d70: 7420 2d69 202e 2f65 7861 6d70 6c65 2f66  t -i ./example/f
+00003d80: 6f72 6d61 745f 6462 5f6d 6c73 745f 696e  ormat_db_mlst_in
+00003d90: 2f20 2d6f 202e 2f65 7861 6d70 6c65 2f6d  / -o ./example/m
+00003da0: 6c73 745f 6f75 742f 200d 0a0d 0a23 2323  lst_out/ ....###
+00003db0: 2320 4f75 7470 7574 0d0a 0d0a 6060 600d  # Output....```.
+00003dc0: 0a7b 6f75 7420 666f 6c64 6572 206e 616d  .{out folder nam
+00003dd0: 657d 0d0a e294 9ce2 9480 e294 8020 7265  e}........... re
+00003de0: 7375 6c74 732e 6a73 6f6e 2020 2020 2020  sults.json      
+00003df0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00003e00: e294 94e2 9480 e294 8020 6c6f 6369 6465  ......... locide
+00003e10: 782e 7478 740d 0a60 6060 0d0a 0d0a 2323  x.txt..```....##
+00003e20: 2320 4275 696c 640d 0a0d 0a42 7569 6c64  # Build....Build
+00003e30: 7320 6c6f 6369 6465 7820 6462 2066 6f6c  s locidex db fol
+00003e40: 6465 7220 7374 7275 6374 7572 650d 0a0d  der structure...
+00003e50: 0a2d 2043 7265 6174 6573 2064 6174 6162  .- Creates datab
+00003e60: 6173 6520 636f 6e66 6967 7572 6174 696f  ase configuratio
+00003e70: 6e20 6669 6c65 0d0a 2d20 4372 6561 7465  n file..- Create
+00003e80: 7320 6c6f 6369 206d 6574 6164 6174 6120  s loci metadata 
+00003e90: 6669 6c65 0d0a 2d20 436f 6e73 7472 7563  file..- Construc
+00003ea0: 7420 626c 6173 7420 6461 7461 6261 7365  t blast database
+00003eb0: 7320 286e 7563 6c65 6f74 6964 6520 616e  s (nucleotide an
+00003ec0: 642f 6f72 2070 726f 7465 696e 290d 0a0d  d/or protein)...
+00003ed0: 0a23 2323 2320 496e 7075 740d 0a0d 0a54  .#### Input....T
+00003ee0: 616b 6573 2074 6865 206f 7574 7075 7420  akes the output 
+00003ef0: 6f66 202a 2a6c 6f63 6964 6578 2066 6f72  of **locidex for
+00003f00: 6d61 742a 2a20 286d 6179 206f 7220 6d61  mat** (may or ma
+00003f10: 7920 6e6f 7420 6861 7665 2061 6464 6974  y not have addit
+00003f20: 696f 6e61 6c20 636f 6c75 6d6e 7320 6164  ional columns ad
+00003f30: 6465 6429 2e20 5468 6572 6520 6172 6520  ded). There are 
+00003f40: 7370 6563 6966 6963 2066 6965 6c64 7320  specific fields 
+00003f50: 6265 696e 6720 6c6f 6f6b 6564 2066 6f72  being looked for
+00003f60: 2069 6e20 7468 6520 6669 6c65 2077 6869   in the file whi
+00003f70: 6368 2065 6974 6865 7220 6f72 2062 6f74  ch either or bot
+00003f80: 6820 6172 6520 7265 7175 6972 6564 2064  h are required d
+00003f90: 6570 656e 6469 6e67 206f 6e20 7468 6520  epending on the 
+00003fa0: 7479 7065 206f 6620 6462 2062 6569 6e67  type of db being
+00003fb0: 2062 7569 6c74 2022 646e 615f 7365 7122   built "dna_seq"
+00003fc0: 2c20 2261 615f 7365 7122 2e0d 0a5b 4920  , "aa_seq"...[I 
+00003fd0: 5448 494e 4b20 5448 4953 204e 4545 4453  THINK THIS NEEDS
+00003fe0: 204c 4f4f 4b49 4e47 2041 545d 0d0a 0d0a   LOOKING AT]....
+00003ff0: 0d0a 0909 6c6f 6369 6465 7820 6275 696c  ....locidex buil
+00004000: 6420 2d69 202e 2f65 7861 6d70 6c65 2f62  d -i ./example/b
+00004010: 7569 6c64 5f64 625f 6d6c 7374 5f69 6e2f  uild_db_mlst_in/
+00004020: 7365 6e74 6572 6963 612e 6d6c 7374 2e74  senterica.mlst.t
+00004030: 7874 202d 6f20 2e2f 6578 616d 706c 652f  xt -o ./example/
+00004040: 6d6c 7374 5f6f 7574 5f64 622f 200d 0a0d  mlst_out_db/ ...
+00004050: 0a23 2323 2320 4f75 7470 7574 0d0a 0d0a  .#### Output....
+00004060: 5468 6973 2063 6f6d 6d61 6e64 2065 7874  This command ext
+00004070: 7261 6374 7320 7468 6520 7365 7175 656e  racts the sequen
+00004080: 6365 2064 6174 6120 286e 7563 6c65 6f74  ce data (nucleot
+00004090: 6964 657c 7072 6f74 6569 6e29 2061 6e64  ide|protein) and
+000040a0: 2069 6e69 7469 616c 697a 6573 2074 6865   initializes the
+000040b0: 2063 6f6e 6669 672e 6a73 6f6e 2c20 6d65   config.json, me
+000040c0: 7461 2e6a 736f 6e20 616e 6420 626c 6173  ta.json and blas
+000040d0: 7420 6462 2073 7472 7563 7475 7265 2077  t db structure w
+000040e0: 6869 6368 206c 6f63 6964 6578 2073 6561  hich locidex sea
+000040f0: 7263 6820 7265 7175 6972 6573 2e0d 0a53  rch requires...S
+00004100: 6565 202d 205b 4461 7461 6261 7365 2073  ee - [Database s
+00004110: 7472 7563 7475 7265 5d28 2f52 4541 444d  tructure](/READM
+00004120: 452e 6d64 2344 6174 6162 6173 6529 2066  E.md#Database) f
+00004130: 6f72 2066 7572 7468 6572 2069 6e66 6f72  or further infor
+00004140: 6d61 7469 6f6e 2e0d 0a0d 0a23 2320 4578  mation.....## Ex
+00004150: 616d 706c 6520 776f 726b 666c 6f77 0d0a  ample workflow..
+00004160: 0d0a 4d4c 5354 2045 7861 6d70 6c65 3a20  ..MLST Example: 
+00004170: 5468 6520 372d 6765 6e65 204d 4c53 5420  The 7-gene MLST 
+00004180: 7363 6865 6d65 2074 6172 6765 7473 2066  scheme targets f
+00004190: 726f 6d20 5b68 7474 7073 3a2f 2f70 7562  rom [https://pub
+000041a0: 6d6c 7374 2e6f 7267 2f6f 7267 616e 6973  mlst.org/organis
+000041b0: 6d73 2f73 616c 6d6f 6e65 6c6c 612d 7370  ms/salmonella-sp
+000041c0: 705d 2868 7474 7073 3a2f 2f70 7562 6d6c  p](https://pubml
+000041d0: 7374 2e6f 7267 2f6f 7267 616e 6973 6d73  st.org/organisms
+000041e0: 2f73 616c 6d6f 6e65 6c6c 612d 7370 7029  /salmonella-spp)
+000041f0: 2077 6572 6520 7573 6564 2061 7320 7461   were used as ta
+00004200: 7267 6574 7320 746f 2065 7874 7261 6374  rgets to extract
+00004210: 2074 6865 2066 756c 6c20 6c65 6e67 7468   the full length
+00004220: 2043 4453 2061 6e6e 6f74 6174 696f 6e73   CDS annotations
+00004230: 2066 726f 6d20 4e43 5f30 3033 3139 382e   from NC_003198.
+00004240: 3120 2853 616c 6d6f 6e65 6c6c 6120 5479  1 (Salmonella Ty
+00004250: 7068 6920 4354 3138 292e 2053 6571 7565  phi CT18). Seque
+00004260: 6e63 6573 2077 6572 6520 7365 7061 7261  nces were separa
+00004270: 7465 6420 696e 746f 2069 6e64 6976 6964  ted into individ
+00004280: 7561 6c20 6661 7374 6120 6669 6c65 7320  ual fasta files 
+00004290: 666f 7220 6561 6368 2067 656e 652c 2074  for each gene, t
+000042a0: 686f 7567 6820 6120 636f 6e63 6174 6f6e  hough a concaton
+000042b0: 6174 6564 2076 6572 7369 6f6e 2077 6f75  ated version wou
+000042c0: 6c64 2061 6c73 6f20 776f 726b 2061 7320  ld also work as 
+000042d0: 6c6f 6e67 2061 7320 7468 6520 6661 7374  long as the fast
+000042e0: 6120 6865 6164 6572 2062 6567 616e 2077  a header began w
+000042f0: 6974 6820 7468 6520 6c6f 6375 7320 6964  ith the locus id
+00004300: 656e 7469 6669 6572 2e20 0d0a 0d0a 3e20  entifier. ....> 
+00004310: 5b21 4e6f 7465 5d0d 0a3e 2054 6865 2065  [!Note]..> The e
+00004320: 7874 7261 6374 6564 2020 4344 5320 616e  xtracted  CDS an
+00004330: 6e6f 7461 7469 6f6e 7320 6172 6520 6e6f  notations are no
+00004340: 7420 6a75 7374 2074 6865 204d 4c53 5420  t just the MLST 
+00004350: 7461 7267 6574 2073 6571 7565 6e63 6573  target sequences
+00004360: 2062 7574 2074 6865 2066 756c 6c20 6f72   but the full or
+00004370: 6620 616e 6420 736f 2074 6869 7320 7769  f and so this wi
+00004380: 6c6c 2064 6966 6665 7220 6672 6f6d 206e  ll differ from n
+00004390: 6f72 6d61 6c20 4d4c 5354 2072 6573 756c  ormal MLST resul
+000043a0: 7473 2e20 4966 2079 6f75 2077 616e 7420  ts. If you want 
+000043b0: 746f 2075 7365 2074 6865 2074 7261 6469  to use the tradi
+000043c0: 7469 6f6e 616c 2073 7562 7365 6374 696f  tional subsectio
+000043d0: 6e73 206f 6620 6561 6368 206c 6f63 692c  ns of each loci,
+000043e0: 2079 6f75 2077 696c 6c20 6e65 6564 2074   you will need t
+000043f0: 6f20 6578 7472 6163 7420 7468 6573 6520  o extract these 
+00004400: 7573 696e 6720 616e 6f74 6865 7220 6d65  using another me
+00004410: 7468 6f64 2e20 0d0a 0d0a 606c 6f63 6964  thod. ....`locid
+00004420: 6578 2066 6f72 6d61 7460 2069 7320 7573  ex format` is us
+00004430: 6564 2074 6f20 6372 6561 7465 2061 2054  ed to create a T
+00004440: 5356 2066 696c 6520 636f 6e74 6169 6e69  SV file containi
+00004450: 6e67 2074 6865 2073 6571 7565 6e63 6520  ng the sequence 
+00004460: 6f66 2065 6163 6820 6f66 2074 6865 2074  of each of the t
+00004470: 6172 6765 7473 2061 6e64 2069 6e64 6976  argets and indiv
+00004480: 6964 7561 6c20 6d61 7463 6820 7468 7265  idual match thre
+00004490: 7368 6f6c 6473 2066 6f72 2065 6163 6820  sholds for each 
+000044a0: 7175 6572 792e 2054 6865 7365 2063 616e  query. These can
+000044b0: 2062 6520 6d6f 6469 6669 6564 2062 7920   be modified by 
+000044c0: 7468 6520 7573 6572 2062 6566 6f72 6520  the user before 
+000044d0: 6275 696c 6469 6e67 2074 6865 2064 6174  building the dat
+000044e0: 6162 6173 652e 200d 0a0d 0a09 096c 6f63  abase. ......loc
+000044f0: 6964 6578 2066 6f72 6d61 7420 2d69 207e  idex format -i ~
+00004500: 2f65 7861 6d70 6c65 2f66 6f72 6d61 745f  /example/format_
+00004510: 6462 5f6d 6c73 745f 696e 2f20 2d6f 207e  db_mlst_in/ -o ~
+00004520: 2f65 7861 6d70 6c65 2f66 6f72 6d61 745f  /example/format_
+00004530: 6462 5f6d 6c73 745f 6f75 742f 202d 2d66  db_mlst_out/ --f
+00004540: 6f72 6365 0d0a 0d0a 5468 6520 606c 6f63  orce....The `loc
+00004550: 6964 6578 2062 7569 6c64 6020 636f 6e76  idex build` conv
+00004560: 6572 7473 2074 6861 7420 5453 5620 696e  erts that TSV in
+00004570: 746f 2061 2066 6f72 6d20 7468 6174 2060  to a form that `
+00004580: 6c6f 6369 6465 7820 7365 6172 6368 6020  locidex search` 
+00004590: 6361 6e20 7573 652e 0d0a 0d0a 0909 6c6f  can use.......lo
+000045a0: 6369 6465 7820 6275 696c 6420 2d69 207e  cidex build -i ~
+000045b0: 2f65 7861 6d70 6c65 2f66 6f72 6d61 745f  /example/format_
+000045c0: 6462 5f6d 6c73 745f 6f75 742f 6c6f 6369  db_mlst_out/loci
+000045d0: 6465 782e 7478 7420 2d6f 207e 2f65 7861  dex.txt -o ~/exa
+000045e0: 6d70 6c65 2f62 7569 6c64 5f64 625f 6d6c  mple/build_db_ml
+000045f0: 7374 5f6f 7574 2f20 2d2d 666f 7263 650d  st_out/ --force.
+00004600: 0a0d 0a60 6c6f 6369 6465 7820 7365 6172  ...`locidex sear
+00004610: 6368 6020 6973 2075 7365 6420 746f 2071  ch` is used to q
+00004620: 7565 7279 2061 6761 696e 7374 2074 6865  uery against the
+00004630: 2064 6174 6162 6173 6520 746f 2070 726f   database to pro
+00004640: 6475 6365 2061 2073 6571 7565 6e63 6520  duce a sequence 
+00004650: 7374 6f72 6520 2874 776f 2065 7861 6d70  store (two examp
+00004660: 6c65 7320 6172 6520 7072 6f76 6964 6564  les are provided
+00004670: 2068 6572 6520 746f 2073 686f 7720 7468   here to show th
+00004680: 6520 7573 6520 6f66 2067 656e 6261 6e6b  e use of genbank
+00004690: 2061 6e6e 6f74 6174 696f 6e73 206f 7220   annotations or 
+000046a0: 7072 6f64 6967 616c 2072 6573 756c 7473  prodigal results
+000046b0: 292e 0d0a 0d0a 0909 6c6f 6369 6465 7820  ).......locidex 
+000046c0: 7365 6172 6368 202d 7120 7e2f 6578 616d  search -q ~/exam
+000046d0: 706c 652f 7365 6172 6368 2f4e 435f 3030  ple/search/NC_00
+000046e0: 3331 3938 2e31 2e67 626b 202d 6420 7e2f  3198.1.gbk -d ~/
+000046f0: 6578 616d 706c 652f 6275 696c 645f 6462  example/build_db
+00004700: 5f6d 6c73 745f 6f75 742f 202d 6f20 2e2f  _mlst_out/ -o ./
+00004710: 6d6c 7374 5f6e 6362 695f 616e 6e6f 7461  mlst_ncbi_annota
+00004720: 7465 6420 2d2d 666f 7263 6520 0d0a 0d0a  ted --force ....
+00004730: 0909 6c6f 6369 6465 7820 7365 6172 6368  ..locidex search
+00004740: 202d 7120 7e2f 6578 616d 706c 652f 7365   -q ~/example/se
+00004750: 6172 6368 2f4e 435f 3030 3331 3938 2e31  arch/NC_003198.1
+00004760: 2e66 6173 7461 202d 6420 7e2f 6578 616d  .fasta -d ~/exam
+00004770: 706c 652f 6275 696c 645f 6462 5f6d 6c73  ple/build_db_mls
+00004780: 745f 6f75 742f 202d 6f20 2e2f 6d6c 7374  t_out/ -o ./mlst
+00004790: 5f70 726f 6469 6761 6c20 2d2d 666f 7263  _prodigal --forc
+000047a0: 6520 2d2d 616e 6e6f 7461 7465 0d0a 0d0a  e --annotate....
+000047b0: 546f 2063 616c 6c20 7468 6520 616c 6c65  To call the alle
+000047c0: 6c65 7320 6672 6f6d 2074 6865 2062 6c61  les from the bla
+000047d0: 7374 2072 6573 756c 7473 206f 6620 7468  st results of th
+000047e0: 6520 7365 6172 6368 206d 6f64 756c 652c  e search module,
+000047f0: 2074 6865 2060 6c6f 6369 6465 7820 7265   the `locidex re
+00004800: 706f 7274 6020 6973 2063 616c 6c65 6420  port` is called 
+00004810: 616e 6420 7468 6520 7361 6d70 6c65 7320  and the samples 
+00004820: 6172 6520 6e61 6d65 6420 6261 7365 6420  are named based 
+00004830: 6f6e 2074 6865 2075 7365 7220 696e 7075  on the user inpu
+00004840: 742e 2049 6620 6e6f 206e 616d 6520 6973  t. If no name is
+00004850: 2073 7065 6369 6669 6564 2074 6865 6e20   specified then 
+00004860: 7468 6520 6261 7365 206e 616d 6520 6f66  the base name of
+00004870: 2074 6865 2066 696c 6520 6973 2075 7365   the file is use
+00004880: 642e 2028 7477 6f20 6578 616d 706c 6573  d. (two examples
+00004890: 2061 7265 2070 726f 7669 6465 6420 746f   are provided to
+000048a0: 2073 686f 7720 7468 6520 6469 6666 6572   show the differ
+000048b0: 656e 6365 2077 6865 6e20 7573 696e 6720  ence when using 
+000048c0: 6765 6e62 616e 6b20 616e 6e6f 7461 7469  genbank annotati
+000048d0: 6f6e 7320 7673 2070 726f 6469 6761 6c20  ons vs prodigal 
+000048e0: 7265 7375 6c74 7329 0d0a 0d0a 0909 6c6f  results)......lo
+000048f0: 6369 6465 7820 7265 706f 7274 202d 6920  cidex report -i 
+00004900: 2e2f 6d6c 7374 5f6e 6362 695f 616e 6e6f  ./mlst_ncbi_anno
+00004910: 7461 7465 642f 7365 715f 7374 6f72 652e  tated/seq_store.
+00004920: 6a73 6f6e 202d 6f20 2e2f 6d6c 7374 5f6e  json -o ./mlst_n
+00004930: 6362 695f 616e 6e6f 7461 7465 642f 7265  cbi_annotated/re
+00004940: 706f 7274 202d 2d6e 616d 6520 6e63 6269  port --name ncbi
+00004950: 202d 2d66 6f72 6365 0d0a 0d0a 0909 6c6f   --force......lo
+00004960: 6369 6465 7820 7265 706f 7274 202d 6920  cidex report -i 
+00004970: 2e2f 6d6c 7374 5f70 726f 6469 6761 6c2f  ./mlst_prodigal/
+00004980: 7365 715f 7374 6f72 652e 6a73 6f6e 202d  seq_store.json -
+00004990: 6f20 2e2f 6d6c 7374 5f70 726f 6469 6761  o ./mlst_prodiga
+000049a0: 6c2f 7265 706f 7274 202d 2d6e 616d 6520  l/report --name 
+000049b0: 7072 6f64 6967 616c 202d 2d66 6f72 6365  prodigal --force
+000049c0: 0d0a 0d0a 4669 6e61 6c6c 792c 2074 6865  ....Finally, the
+000049d0: 2069 6e64 6976 6964 7561 6c20 7072 6f66   individual prof
+000049e0: 696c 6573 2061 7265 206d 6572 6765 6420  iles are merged 
+000049f0: 696e 746f 2061 2054 5356 2066 696c 6520  into a TSV file 
+00004a00: 7768 6963 6820 6973 2063 6f6d 7061 7469  which is compati
+00004a10: 626c 6520 7769 7468 2064 6f77 6e73 7472  ble with downstr
+00004a20: 6561 6d20 6765 6e65 2070 726f 6669 6c65  eam gene profile
+00004a30: 2069 6e70 7574 2076 6961 2060 6c6f 6369   input via `loci
+00004a40: 6465 7820 6d65 7267 6560 0d0a 0d0a 0909  dex merge`......
+00004a50: 6c6f 6369 6465 7820 6d65 7267 6520 2d69  locidex merge -i
+00004a60: 202e 2f6d 6c73 745f 6e63 6269 5f61 6e6e   ./mlst_ncbi_ann
+00004a70: 6f74 6174 6564 2f72 6570 6f72 742f 7072  otated/report/pr
+00004a80: 6f66 696c 652e 6a73 6f6e 202e 2f2f 6d6c  ofile.json .//ml
+00004a90: 7374 5f70 726f 6469 6761 6c2f 7265 706f  st_prodigal/repo
+00004aa0: 7274 2f70 726f 6669 6c65 2e6a 736f 6e20  rt/profile.json 
+00004ab0: 2d6f 202e 2f6d 6572 6765 6420 2d2d 666f  -o ./merged --fo
+00004ac0: 7263 650d 0a0d 0a23 2320 4461 7461 6261  rce....## Databa
+00004ad0: 7365 2073 7472 7563 7475 7265 0d0a 0d0a  se structure....
+00004ae0: 5369 6d69 6c61 7220 746f 205b 6162 7269  Similar to [abri
+00004af0: 6361 7465 5d28 6874 7470 733a 2f2f 6769  cate](https://gi
+00004b00: 7468 7562 2e63 6f6d 2f74 7365 656d 616e  thub.com/tseeman
+00004b10: 6e2f 6162 7269 6361 7465 292c 204c 6f63  n/abricate), Loc
+00004b20: 6964 6578 2075 7365 7320 6120 6669 7865  idex uses a fixe
+00004b30: 6420 6461 7461 6261 7365 2073 7472 7563  d database struc
+00004b40: 7475 7265 206c 6179 6f75 742e 204c 6f63  ture layout. Loc
+00004b50: 6964 6578 2073 7570 706f 7274 7320 6e75  idex supports nu
+00004b60: 636c 656f 7469 6465 2028 626c 6173 746e  cleotide (blastn
+00004b70: 2920 616e 6420 7072 6f74 6569 6e20 2862  ) and protein (b
+00004b80: 6c61 7374 7029 2062 6c61 7374 2073 6561  lastp) blast sea
+00004b90: 7263 6865 732e 2049 7420 7574 696c 697a  rches. It utiliz
+00004ba0: 6573 2061 2066 6577 2063 6f6e 7472 6f6c  es a few control
+00004bb0: 6c65 6420 6669 656c 6473 2069 6e20 636f  led fields in co
+00004bc0: 6e66 6967 2e6a 736f 6e20 616e 6420 6d65  nfig.json and me
+00004bd0: 7461 2e6a 736f 6e20 6275 7420 636f 6d70  ta.json but comp
+00004be0: 6c65 7465 6c79 2073 7570 706f 7274 7320  letely supports 
+00004bf0: 7468 6520 6164 6469 746f 6e20 6f66 2061  the additon of a
+00004c00: 6e79 206e 756d 6265 7220 6f66 2061 6464  ny number of add
+00004c10: 6974 696f 6e61 6c20 6669 656c 6473 2074  itional fields t
+00004c20: 6861 7420 6d61 7920 6265 2064 6573 6972  hat may be desir
+00004c30: 6564 2062 7920 7468 6520 6461 7461 6261  ed by the databa
+00004c40: 7365 2062 7569 6c64 6572 2e20 5468 6572  se builder. Ther
+00004c50: 6520 6973 2061 206e 6573 7465 6420 666f  e is a nested fo
+00004c60: 6c64 6572 2073 7472 7563 7475 7265 2066  lder structure f
+00004c70: 6f72 2074 6865 2062 6c61 7374 2064 6174  or the blast dat
+00004c80: 6162 6173 6573 2077 6869 6368 206d 7573  abases which mus
+00004c90: 7420 636f 6e66 6f72 6d20 746f 2074 6865  t conform to the
+00004ca0: 206c 6179 6f75 7420 6265 6c6f 772e 0d0a   layout below...
+00004cb0: 0d0a 6060 600d 0a7b 4442 2066 6f6c 6465  ..```..{DB folde
+00004cc0: 7220 6e61 6d65 7d0d 0ae2 949c e294 80e2  r name}.........
+00004cd0: 9480 2063 6f6e 6669 672e 6a73 6f6e 2020  .. config.json  
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 2023 7265 7175 6972 6564 0d0a e294     #required....
+00004d00: 9ce2 9480 e294 8020 6d65 7461 2e6a 736f  ....... meta.jso
+00004d10: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00004d20: 2020 2020 2020 2020 2372 6571 7569 7265          #require
+00004d30: 640d 0ae2 9494 e294 80e2 9480 2062 6c61  d........... bla
+00004d40: 7374 2020 2020 2020 2020 2020 2020 2020  st              
+00004d50: 2020 2020 2020 2020 2020 2020 2023 7265               #re
+00004d60: 7175 6972 6564 0d0a 2020 2020 e294 94e2  quired..    ....
+00004d70: 9480 e294 8020 6e75 636c 656f 7469 6465  ..... nucleotide
+00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d90: 2020 236f 7074 696f 6e61 6c20 6275 7420    #optional but 
+00004da0: 3e3d 2031 6d75 7374 2062 6520 7072 6573  >= 1must be pres
+00004db0: 656e 740d 0a20 2020 2020 2020 20e2 949c  ent..        ...
+00004dc0: e294 80e2 9480 6e75 636c 656f 7469 6465  ......nucleotide
+00004dd0: 2e66 6173 7461 0d0a 2020 2020 2020 2020  .fasta..        
+00004de0: e294 9ce2 9480 e294 806e 7563 6c65 6f74  .........nucleot
+00004df0: 6964 652e 6e64 620d 0a20 2020 2020 2020  ide.ndb..       
+00004e00: 20e2 949c e294 80e2 9480 6e75 636c 656f   .........nucleo
+00004e10: 7469 6465 2e6e 6872 0d0a 2020 2020 2020  tide.nhr..      
+00004e20: 2020 e294 9ce2 9480 e294 806e 7563 6c65    .........nucle
+00004e30: 6f74 6964 652e 6e69 6e0d 0a20 2020 2020  otide.nin..     
+00004e40: 2020 20e2 949c e294 80e2 9480 6e75 636c     .........nucl
+00004e50: 656f 7469 6465 2e6e 6a73 0d0a 2020 2020  eotide.njs..    
+00004e60: 2020 2020 e294 9ce2 9480 e294 806e 7563      .........nuc
+00004e70: 6c65 6f74 6964 652e 6e73 710d 0a20 2020  leotide.nsq..   
+00004e80: 2020 2020 20e2 949c e294 80e2 9480 6e75       .........nu
+00004e90: 636c 656f 7469 6465 2e6e 7466 0d0a 2020  cleotide.ntf..  
+00004ea0: 2020 2020 2020 e294 94e2 9480 e294 806e        .........n
+00004eb0: 7563 6c65 6f74 6964 652e 6e74 6f20 0d0a  ucleotide.nto ..
+00004ec0: 2020 2020 e294 94e2 9480 e294 8070 726f      .........pro
+00004ed0: 7465 696e 2020 2020 2020 2020 2020 2020  tein            
+00004ee0: 2020 2020 2020 2020 2020 236f 7074 696f            #optio
+00004ef0: 6e61 6c20 6275 7420 3e3d 2031 6d75 7374  nal but >= 1must
+00004f00: 2062 6520 7072 6573 656e 740d 0a20 2020   be present..   
+00004f10: 2020 2020 20e2 949c e294 80e2 9480 2070       ......... p
+00004f20: 726f 7465 696e 2e66 6173 7461 0d0a 2020  rotein.fasta..  
+00004f30: 2020 2020 2020 e294 9ce2 9480 e294 8020        ......... 
+00004f40: 7072 6f74 6569 6e2e 7064 620d 0a20 2020  protein.pdb..   
+00004f50: 2020 2020 20e2 949c e294 80e2 9480 2070       ......... p
+00004f60: 726f 7465 696e 2e70 6872 0d0a 2020 2020  rotein.phr..    
+00004f70: 2020 2020 e294 9ce2 9480 e294 8020 7072      ......... pr
+00004f80: 6f74 6569 6e2e 7069 6e0d 0a20 2020 2020  otein.pin..     
+00004f90: 2020 20e2 949c e294 80e2 9480 2070 726f     ......... pro
+00004fa0: 7465 696e 2e70 6a73 0d0a 2020 2020 2020  tein.pjs..      
+00004fb0: 2020 e294 9ce2 9480 e294 8020 7072 6f74    ......... prot
+00004fc0: 6569 6e2e 706f 740d 0a20 2020 2020 2020  ein.pot..       
+00004fd0: 20e2 949c e294 80e2 9480 2070 726f 7465   ......... prote
+00004fe0: 696e 2e70 7371 0d0a 2020 2020 2020 2020  in.psq..        
+00004ff0: e294 9ce2 9480 e294 8020 7072 6f74 6569  ......... protei
+00005000: 6e2e 7074 660d 0a20 2020 2020 2020 20e2  n.ptf..        .
+00005010: 9494 e294 80e2 9480 7072 6f74 6569 6e2e  ........protein.
+00005020: 7074 6f0d 0a60 6060 0d0a 0d0a 2323 2320  pto..```....### 
+00005030: 636f 6e66 6967 2e6a 736f 6e0d 0a0d 0a54  config.json....T
+00005040: 6869 7320 5b4a 534f 4e5d 2868 7474 7073  his [JSON](https
+00005050: 3a2f 2f77 7777 2e6a 736f 6e2e 6f72 672f  ://www.json.org/
+00005060: 6a73 6f6e 2d65 6e2e 6874 6d6c 2920 6669  json-en.html) fi
+00005070: 6c65 2069 7320 7265 7370 6f6e 7369 626c  le is responsibl
+00005080: 6520 666f 7220 656e 636f 6469 6e67 2074  e for encoding t
+00005090: 6865 206d 6574 6164 6174 6120 7265 6761  he metadata rega
+000050a0: 7264 696e 6720 7468 6520 6c6f 6369 6465  rding the locide
+000050b0: 7820 6461 7461 6261 7365 2077 6869 6368  x database which
+000050c0: 2077 696c 6c20 6265 2062 756e 646c 6564   will be bundled
+000050d0: 2069 6e74 6f20 7468 6520 7365 715f 7374   into the seq_st
+000050e0: 6f72 6520 6f75 7470 7574 206f 6620 7468  ore output of th
+000050f0: 6520 7365 6172 6368 206d 6f64 756c 652e  e search module.
+00005100: 2049 7420 616c 736f 2064 6574 6572 6d69   It also determi
+00005110: 6e65 7320 7768 6574 6865 7220 6120 6769  nes whether a gi
+00005120: 7665 6e20 6461 7461 6261 7365 2069 7320  ven database is 
+00005130: 7573 6564 2066 6f72 206e 7563 6c65 6f74  used for nucleot
+00005140: 6964 6520 616e 642f 6f72 2070 726f 7465  ide and/or prote
+00005150: 696e 2062 6c61 7374 2073 6561 7263 6865  in blast searche
+00005160: 732e 2054 6869 7320 6461 7461 2061 7373  s. This data ass
+00005170: 6973 7473 2077 6974 6820 7072 6f76 656e  ists with proven
+00005180: 616e 6365 2069 6e66 6f72 6d61 7469 6f6e  ance information
+00005190: 2072 6567 6172 6469 6e67 2073 6561 7263   regarding searc
+000051a0: 6820 7265 7375 6c74 732e 0d0a 0d0a 6060  h results.....``
+000051b0: 600d 0a20 2020 2020 2020 207b 0d0a 2020  `..        {..  
+000051c0: 2020 2020 2020 2020 2020 2264 625f 6e61            "db_na
+000051d0: 6d65 223a 2022 5361 6c6d 6f6e 656c 6c61  me": "Salmonella
+000051e0: 2043 6865 7762 6261 6361 2d4f 6e6c 696e   Chewbbaca-Onlin
+000051f0: 6520 6367 4d4c 5354 222c 0d0a 2020 2020  e cgMLST",..    
+00005200: 2020 2020 2020 2020 2264 625f 7665 7273          "db_vers
+00005210: 696f 6e22 3a20 2231 2e30 2e30 222c 0d0a  ion": "1.0.0",..
+00005220: 2020 2020 2020 2020 2020 2020 2264 625f              "db_
+00005230: 6461 7465 223a 2022 3230 3234 2d30 322d  date": "2024-02-
+00005240: 3031 222c 0d0a 2020 2020 2020 2020 2020  01",..          
+00005250: 2020 2264 625f 6175 7468 6f72 223a 2022    "db_author": "
+00005260: 4a61 6d65 7320 526f 6265 7274 736f 6e22  James Robertson"
+00005270: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00005280: 6462 5f64 6573 6322 3a20 2244 6174 6120  db_desc": "Data 
+00005290: 6f62 7461 696e 6564 2066 726f 6d3a 2068  obtained from: h
+000052a0: 7474 7073 3a2f 2f63 6865 7762 6261 6361  ttps://chewbbaca
+000052b0: 2e6f 6e6c 696e 652f 7370 6563 6965 732f  .online/species/
+000052c0: 3822 2c0d 0a20 2020 2020 2020 2020 2020  8",..           
+000052d0: 2022 6462 5f6e 756d 5f73 6571 7322 3a38   "db_num_seqs":8
+000052e0: 3535 382c 0d0a 2020 2020 2020 2020 2020  558,..          
+000052f0: 2020 2269 735f 6e75 636c 223a 2022 5472    "is_nucl": "Tr
+00005300: 7565 222c 0d0a 2020 2020 2020 2020 2020  ue",..          
+00005310: 2020 2269 735f 7072 6f74 223a 2022 5472    "is_prot": "Tr
+00005320: 7565 222c 0d0a 2020 2020 2020 2020 2020  ue",..          
+00005330: 2020 226e 7563 6c65 6f74 6964 655f 6462    "nucleotide_db
+00005340: 5f6e 616d 6522 3a20 226e 7563 656c 6f74  _name": "nucelot
+00005350: 6964 6522 2c0d 0a20 2020 2020 2020 2020  ide",..         
+00005360: 2020 2022 7072 6f74 6569 6e5f 6462 5f6e     "protein_db_n
+00005370: 616d 6522 3a20 2270 726f 7465 696e 220d  ame": "protein".
+00005380: 0a20 2020 2020 2020 207d 0d0a 6060 600d  .        }..```.
+00005390: 0a0d 0a23 2323 206d 6574 612e 6a73 6f6e  ...### meta.json
+000053a0: 0d0a 0d0a 4672 6571 7565 6e74 6c79 2c20  ....Frequently, 
+000053b0: 7468 6572 6520 6973 2061 2064 6573 6972  there is a desir
+000053c0: 6520 746f 2065 6e63 6f64 6520 636f 6e74  e to encode cont
+000053d0: 6578 7475 616c 206d 6574 6164 6174 6120  extual metadata 
+000053e0: 7769 7468 2073 6571 7565 6e63 6520 6461  with sequence da
+000053f0: 7461 2066 6f72 2064 6966 6665 7265 6e74  ta for different
+00005400: 2061 6e61 6c79 7469 6361 6c20 6f70 6572   analytical oper
+00005410: 6174 696f 6e73 2e20 5468 6573 6520 6361  ations. These ca
+00005420: 6e20 7261 6e67 6520 6672 6f6d 2065 6e63  n range from enc
+00005430: 6f64 696e 6720 6765 6e65 2061 6e64 2061  oding gene and a
+00005440: 6c6c 656c 6520 6964 656e 7469 6669 6572  llele identifier
+00005450: 7320 746f 2070 6865 6e6f 7479 7069 6320  s to phenotypic 
+00005460: 6566 6665 6374 7320 616e 6420 6265 796f  effects and beyo
+00005470: 6e64 2e20 5468 6520 6f70 7469 6f6e 7320  nd. The options 
+00005480: 666f 7220 6465 7665 6c6f 7065 7273 2068  for developers h
+00005490: 6173 2062 6565 6e20 746f 2065 6e63 6f64  as been to encod
+000054a0: 6520 7468 6973 2069 6e74 6f20 7468 6520  e this into the 
+000054b0: 6661 7374 6120 6865 6164 6572 2064 6972  fasta header dir
+000054c0: 6563 7479 2077 6974 6820 6469 6666 6572  ecty with differ
+000054d0: 656e 7420 6465 6c69 6d65 7465 7273 2062  ent delimeters b
+000054e0: 6574 7765 656e 2066 6965 6c64 7320 6f72  etween fields or
+000054f0: 2074 6f20 6861 7665 2061 6e20 6164 6469   to have an addi
+00005500: 7469 6f6e 616c 2066 696c 6520 7769 7468  tional file with
+00005510: 2074 6865 2064 6573 6972 6564 2063 6f6e   the desired con
+00005520: 7465 7874 7561 6c20 696e 666f 726d 6174  textual informat
+00005530: 696f 6e20 7365 7061 7261 7465 2066 726f  ion separate fro
+00005540: 6d20 7468 6520 7365 7175 656e 6365 2064  m the sequence d
+00005550: 6174 612e 204c 6f63 6964 6578 2075 7469  ata. Locidex uti
+00005560: 6c69 7a65 7320 7468 6520 6c61 7465 7220  lizes the later 
+00005570: 6170 7072 6f61 6368 2077 6974 6820 616c  approach with al
+00005580: 6c20 6f66 2074 6865 2064 6174 6120 656e  l of the data en
+00005590: 636f 6465 6420 696e 205b 4a53 4f4e 5d28  coded in [JSON](
+000055a0: 6874 7470 733a 2f2f 7777 772e 6a73 6f6e  https://www.json
+000055b0: 2e6f 7267 2f6a 736f 6e2d 656e 2e68 746d  .org/json-en.htm
+000055c0: 6c29 2066 6f72 2065 6173 7920 7061 7273  l) for easy pars
+000055d0: 696e 6720 6279 2064 6f77 6e73 7472 6561  ing by downstrea
+000055e0: 6d20 6170 706c 6963 6174 696f 6e73 2e20  m applications. 
+000055f0: 5468 6973 2066 696c 6520 6973 2075 7365  This file is use
+00005600: 6420 6279 2074 6865 2073 6561 7263 6820  d by the search 
+00005610: 6d6f 6475 6c65 2074 6f20 6275 6e64 6c65  module to bundle
+00005620: 2074 6869 7320 636f 6e74 6578 7475 616c   this contextual
+00005630: 2069 6e66 6f72 6d61 7469 6f6e 2072 6567   information reg
+00005640: 6172 6469 6e67 2074 6865 2064 6174 6162  arding the datab
+00005650: 6173 6520 7365 7175 656e 6365 7320 666f  ase sequences fo
+00005660: 7220 6c61 7465 7220 7573 6520 7769 7468  r later use with
+00005670: 6f75 7420 7468 6520 6e65 6564 2074 6f20  out the need to 
+00005680: 7061 7373 2074 6865 206f 7269 6769 6e61  pass the origina
+00005690: 6c20 6d65 7461 2e6a 736f 6e20 696e 666f  l meta.json info
+000056a0: 726d 6174 696f 6e20 6265 7477 6565 6e20  rmation between 
+000056b0: 7072 6f63 6573 7365 732e 2041 6e20 6578  processes. An ex
+000056c0: 616d 706c 6520 7374 7562 2069 7320 7368  ample stub is sh
+000056d0: 6f77 6e20 6265 6c6f 7720 666f 7220 6d65  own below for me
+000056e0: 7461 6461 7461 2e20 616e 6420 616e 7920  tadata. and any 
+000056f0: 6e75 6d62 6572 206f 6620 6164 6469 7469  number of additi
+00005700: 6f6e 616c 2066 6965 6c64 7320 6361 6e20  onal fields can 
+00005710: 6265 2061 6464 6564 2074 6f20 7265 636f  be added to reco
+00005720: 7264 732e 0d0a 0d0a 6060 600d 0a7b 0d0a  rds.....```..{..
+00005730: 2020 2020 2269 6e66 6f22 3a20 7b0d 0a20      "info": {.. 
+00005740: 2020 2020 2020 2022 6e75 6d5f 7365 7173         "num_seqs
+00005750: 223a 2038 3535 382c 0d0a 2020 2020 2020  ": 8558,..      
+00005760: 2020 2269 735f 6364 7322 3a20 2254 7275    "is_cds": "Tru
+00005770: 6522 2c0d 0a20 2020 2020 2020 2022 7472  e",..        "tr
+00005780: 616e 735f 7461 626c 6522 3a20 3131 2c0d  ans_table": 11,.
+00005790: 0a20 2020 2020 2020 2022 646e 615f 6d69  .        "dna_mi
+000057a0: 6e5f 6c65 6e22 3a20 3732 2c0d 0a20 2020  n_len": 72,..   
+000057b0: 2020 2020 2022 646e 615f 6d61 785f 6c65       "dna_max_le
+000057c0: 6e22 3a20 3130 3634 342c 0d0a 2020 2020  n": 10644,..    
+000057d0: 2020 2020 2264 6e61 5f6d 696e 5f69 6465      "dna_min_ide
+000057e0: 6e74 223a 2038 302c 0d0a 2020 2020 2020  nt": 80,..      
+000057f0: 2020 2261 615f 6d69 6e5f 6c65 6e22 3a20    "aa_min_len": 
+00005800: 3234 2c0d 0a20 2020 2020 2020 2022 6161  24,..        "aa
+00005810: 5f6d 6178 5f6c 656e 223a 2033 3534 382c  _max_len": 3548,
+00005820: 0d0a 2020 2020 2020 2020 2261 615f 6d69  ..        "aa_mi
+00005830: 6e5f 6964 656e 7422 3a20 3830 0d0a 2020  n_ident": 80..  
+00005840: 2020 7d2c 0d0a 2020 2020 226d 6574 6122    },..    "meta"
+00005850: 3a20 7b0d 0a20 2020 2020 2020 2022 3022  : {..        "0"
+00005860: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
+00005870: 2022 6c6f 6375 735f 6e61 6d65 223a 2022   "locus_name": "
+00005880: 5341 4c5f 4347 4d4c 5354 5f30 3030 3030  SAL_CGMLST_00000
+00005890: 3030 3031 222c 0d0a 2020 2020 2020 2020  0001",..        
+000058a0: 2020 2020 226c 6f63 7573 5f6e 616d 655f      "locus_name_
+000058b0: 616c 7422 3a20 2249 4e4e 5545 4e44 4f5f  alt": "INNUENDO_
+000058c0: 6367 4d4c 5354 2d30 3030 3338 3330 315f  cgMLST-00038301_
+000058d0: 3122 2c0d 0a20 2020 2020 2020 2020 2020  1",..           
+000058e0: 2022 6c6f 6375 735f 7072 6f64 7563 7422   "locus_product"
+000058f0: 3a20 4e61 4e2c 0d0a 2020 2020 2020 2020  : NaN,..        
+00005900: 2020 2020 226c 6f63 7573 5f64 6573 6372      "locus_descr
+00005910: 6970 7469 6f6e 223a 204e 614e 2c0d 0a20  iption": NaN,.. 
+00005920: 2020 2020 2020 2020 2020 2022 6c6f 6375             "locu
+00005930: 735f 7569 6422 3a20 4e61 4e2c 0d0a 2020  s_uid": NaN,..  
+00005940: 2020 2020 2020 2020 2020 2264 6e61 5f73            "dna_s
+00005950: 6571 5f6c 656e 223a 2031 3532 312c 0d0a  eq_len": 1521,..
+00005960: 2020 2020 2020 2020 2020 2020 2264 6e61              "dna
+00005970: 5f73 6571 5f68 6173 6822 3a20 2263 3137  _seq_hash": "c17
+00005980: 3234 3034 6563 3334 3934 3763 3764 3835  2404ec34947c7d85
+00005990: 6630 6433 6537 6661 3362 3830 3822 2c0d  f0d3e7fa3b808",.
+000059a0: 0a20 2020 2020 2020 2020 2020 2022 6161  .            "aa
+000059b0: 5f73 6571 5f6c 656e 223a 2035 3037 2c0d  _seq_len": 507,.
+000059c0: 0a20 2020 2020 2020 2020 2020 2022 6161  .            "aa
+000059d0: 5f73 6571 5f68 6173 6822 3a20 2238 6132  _seq_hash": "8a2
+000059e0: 3861 6361 3132 6263 6631 3630 3835 3634  8aca12bcf1608564
+000059f0: 3234 3461 3638 3865 3739 6462 3622 2c0d  244a688e79db6",.
+00005a00: 0a20 2020 2020 2020 2020 2020 2022 646e  .            "dn
+00005a10: 615f 6d69 6e5f 6c65 6e22 3a20 3132 3137  a_min_len": 1217
+00005a20: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00005a30: 646e 615f 6d61 785f 6c65 6e22 3a20 3138  dna_max_len": 18
+00005a40: 3235 2c0d 0a20 2020 2020 2020 2020 2020  25,..           
+00005a50: 2022 6161 5f6d 696e 5f6c 656e 223a 2034   "aa_min_len": 4
+00005a60: 3036 2c0d 0a20 2020 2020 2020 2020 2020  06,..           
+00005a70: 2022 6161 5f6d 6178 5f6c 656e 223a 2036   "aa_max_len": 6
+00005a80: 3038 2c0d 0a20 2020 2020 2020 2020 2020  08,..           
+00005a90: 2022 646e 615f 6d69 6e5f 6964 656e 7422   "dna_min_ident"
+00005aa0: 3a20 3830 2c0d 0a20 2020 2020 2020 2020  : 80,..         
+00005ab0: 2020 2022 6161 5f6d 696e 5f69 6465 6e74     "aa_min_ident
+00005ac0: 223a 2038 300d 0a20 2020 2020 2020 207d  ": 80..        }
+00005ad0: 0d0a 2020 2020 7d0d 0a7d 0d0a 6060 600d  ..    }..}..```.
+00005ae0: 0a0d 0a23 2323 2062 6c61 7374 2064 6174  ...### blast dat
+00005af0: 6261 7365 730d 0a0d 0a54 6865 2062 6c61  bases....The bla
+00005b00: 7374 2066 6f6c 6465 7220 6d75 7374 2062  st folder must b
+00005b10: 6520 7072 6573 656e 7420 666f 7220 6120  e present for a 
+00005b20: 6c6f 6369 6465 7820 6461 7461 6261 7365  locidex database
+00005b30: 2074 6f20 6265 2076 616c 6964 2077 6974   to be valid wit
+00005b40: 6820 6e75 636c 656f 7469 6465 2061 6e64  h nucleotide and
+00005b50: 2f6f 7220 7072 6f74 6569 6e20 7375 6266  /or protein subf
+00005b60: 6f6c 6465 7273 2070 7265 7365 6e74 2e20  olders present. 
+00005b70: 466f 7220 6561 6368 2066 6f6c 6465 7220  For each folder 
+00005b80: 7072 6573 656e 742c 2069 7420 6d75 7374  present, it must
+00005b90: 2063 6f6e 7461 696e 2074 6865 2066 6173   contain the fas
+00005ba0: 7461 2066 696c 6520 7573 6564 2074 6f20  ta file used to 
+00005bb0: 6765 6e65 7261 7465 2074 6865 2064 6174  generate the dat
+00005bc0: 6162 6173 6520 286e 7563 6c65 6f74 6964  abase (nucleotid
+00005bd0: 652e 6661 7374 617c 7072 6f74 6569 6e2e  e.fasta|protein.
+00005be0: 6661 7374 6129 2061 6e64 2061 2063 6f72  fasta) and a cor
+00005bf0: 7265 7370 6f6e 6469 6e67 2062 6c61 7374  responding blast
+00005c00: 2064 6174 6162 6173 6520 7769 7468 2074   database with t
+00005c10: 6865 2066 6f6c 6465 7220 6e61 6d65 2077  he folder name w
+00005c20: 6974 686f 7574 2022 2e66 6173 7461 2220  ithout ".fasta" 
+00005c30: 7072 6573 656e 742e 2054 6865 2073 7472  present. The str
+00005c40: 7563 7475 7265 2069 7320 6465 7369 676e  ucture is design
+00005c50: 6564 2074 6f20 616c 6c6f 7720 666f 7220  ed to allow for 
+00005c60: 7468 6520 696e 636c 7573 696f 6e20 6f66  the inclusion of
+00005c70: 206f 7468 6572 2073 6571 7565 6e63 6520   other sequence 
+00005c80: 7369 6d69 6c61 7269 7479 2073 6561 7263  similarity searc
+00005c90: 6820 746f 6f6c 7320 6174 2061 206c 6174  h tools at a lat
+00005ca0: 6572 2064 6174 6520 7769 7468 206d 696e  er date with min
+00005cb0: 696d 616c 206d 6f64 6966 6963 6174 696f  imal modificatio
+00005cc0: 6e73 2e20 5072 6f74 6569 6e20 7365 6172  ns. Protein sear
+00005cd0: 6368 696e 6720 7669 6120 484d 4d73 2061  ching via HMMs a
+00005ce0: 6e64 206f 7468 6572 2074 6f6f 6c73 2073  nd other tools s
+00005cf0: 7563 6820 6173 205b 6469 616d 6f6e 645d  uch as [diamond]
+00005d00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00005d10: 636f 6d2f 6262 7563 6866 696e 6b2f 6469  com/bbuchfink/di
+00005d20: 616d 6f6e 6429 206d 6179 2062 6520 696e  amond) may be in
+00005d30: 636c 7564 6564 2069 6e20 6c61 7465 7220  cluded in later 
+00005d40: 7265 6c65 6173 6573 2e0d 0a0d 0a23 2054  releases.....# T
+00005d50: 726f 7562 6c65 7368 6f6f 7469 6e67 2061  roubleshooting a
+00005d60: 6e64 2046 4151 730d 0a0d 0a23 2320 4641  nd FAQs....## FA
+00005d70: 510d 0a0d 0a2a 2a43 616e 2049 2075 7365  Q....**Can I use
+00005d80: 206e 6f6e 2d63 6f64 696e 6720 7365 7175   non-coding sequ
+00005d90: 656e 6365 7320 6173 2069 6e70 7574 2074  ences as input t
+00005da0: 6f20 6c6f 6369 6465 783f 2a2a 0d0a 0d0a  o locidex?**....
+00005db0: 5965 732c 2079 6f75 2063 616e 2074 6f67  Yes, you can tog
+00005dc0: 676c 6520 6f66 6620 7072 6f74 6569 6e20  gle off protein 
+00005dd0: 636f 6469 6e67 2077 6974 6869 6e20 7468  coding within th
+00005de0: 6520 6461 7461 6261 7365 2063 6f6e 6669  e database confi
+00005df0: 6720 746f 2061 766f 6964 2074 7261 6e73  g to avoid trans
+00005e00: 6c61 7469 6f6e 2061 6e64 2070 726f 7465  lation and prote
+00005e10: 696e 2062 6c61 7374 2073 6561 7263 6865  in blast searche
+00005e20: 732e 2048 6f77 6576 6572 2c20 6966 2079  s. However, if y
+00005e30: 6f75 2077 616e 7420 746f 2075 7365 2074  ou want to use t
+00005e40: 6865 2022 616c 6c65 6c65 2220 6964 656e  he "allele" iden
+00005e50: 7469 7479 206f 6620 796f 7572 206c 6f63  tity of your loc
+00005e60: 7573 2073 7563 6820 6173 2061 6e20 7252  us such as an rR
+00005e70: 4e41 2067 656e 652c 2074 6865 6e20 796f  NA gene, then yo
+00005e80: 7520 7769 6c6c 206e 6565 6420 746f 2065  u will need to e
+00005e90: 7874 7261 6374 206f 7574 2074 6865 2073  xtract out the s
+00005ea0: 6571 7565 6e63 6573 2079 6f75 2077 616e  equences you wan
+00005eb0: 7420 746f 206d 6174 6368 2e0d 0a0d 0a2a  t to match.....*
+00005ec0: 2a44 6f20 4920 6e65 6564 2074 6f20 6861  *Do I need to ha
+00005ed0: 7665 2061 2072 6570 7265 7365 6e74 6974  ve a representit
+00005ee0: 6976 6520 6f66 2065 7665 7279 2061 6c6c  ive of every all
+00005ef0: 656c 6520 4920 7761 6e74 2074 6f20 6d61  ele I want to ma
+00005f00: 7463 6820 696e 206d 7920 6461 7461 6261  tch in my databa
+00005f10: 7365 3f2a 2a0d 0a0d 0a4e 6f2c 2074 6865  se?**....No, the
+00005f20: 2062 656e 6566 6974 206f 6620 6861 7669   benefit of havi
+00005f30: 6e67 2064 7561 6c20 7365 6172 6368 696e  ng dual searchin
+00005f40: 6720 7769 7468 2070 726f 7465 696e 2061  g with protein a
+00005f50: 6e64 2064 6e61 2069 7320 7468 6174 2079  nd dna is that y
+00005f60: 6f75 2063 616e 2068 6176 6520 6120 7370  ou can have a sp
+00005f70: 6172 7365 6c79 2070 6f70 756c 6174 6564  arsely populated
+00005f80: 2064 6174 6162 6173 6520 6f66 2073 6571   database of seq
+00005f90: 7565 6e63 6573 2074 6861 7420 6d65 6574  uences that meet
+00005fa0: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
+00005fb0: 6e73 2073 7065 6369 6669 6320 6e65 6564  ns specific need
+00005fc0: 2e20 5468 6973 206d 6561 6e73 2079 6f75  . This means you
+00005fd0: 2063 616e 2064 6564 7570 6c69 6361 7465   can deduplicate
+00005fe0: 2075 7369 6e67 2061 2074 6f6f 6c20 7375   using a tool su
+00005ff0: 6368 2061 7320 5b63 642d 6869 745d 2868  ch as [cd-hit](h
+00006000: 7474 7073 3a2f 2f73 6974 6573 2e67 6f6f  ttps://sites.goo
+00006010: 676c 652e 636f 6d2f 7669 6577 2f63 642d  gle.com/view/cd-
+00006020: 6869 7429 2074 6f20 7265 6d6f 7665 2068  hit) to remove h
+00006030: 6967 686c 7920 7369 6d69 6c61 7220 7365  ighly similar se
+00006040: 7175 656e 6365 7320 6672 6f6d 2079 6f75  quences from you
+00006050: 7220 6461 7461 6261 7365 2074 6f20 7265  r database to re
+00006060: 6475 6365 2072 756e 7469 6d65 2061 6e64  duce runtime and
+00006070: 2063 6f6d 706c 6578 6974 792e 2059 6f75   complexity. You
+00006080: 2077 696c 6c20 6e65 6564 2074 6f20 656d   will need to em
+00006090: 7069 7261 636c 7920 6465 7465 726d 696e  piracly determin
+000060a0: 6520 7768 6174 206c 6576 656c 206f 6620  e what level of 
+000060b0: 6469 7665 7273 6974 7920 6973 2073 7566  diversity is suf
+000060c0: 6669 6369 656e 7420 666f 7220 796f 7572  ficient for your
+000060d0: 2073 7065 6369 6669 6320 6170 706c 6963   specific applic
+000060e0: 6174 696f 6e2e 0d0a 0d0a 2a2a 486f 7720  ation.....**How 
+000060f0: 646f 6573 204c 6f63 6964 6578 2068 616e  does Locidex han
+00006100: 6465 6c20 6d75 6c74 6963 6f70 7920 6c6f  del multicopy lo
+00006110: 6369 3f2a 2a0d 0a0d 0a49 6465 616c 6c79  ci?**....Ideally
+00006120: 2061 2067 656e 652d 6279 2d67 656e 6520   a gene-by-gene 
+00006130: 7363 6865 6d65 2063 6f6e 7369 7374 7320  scheme consists 
+00006140: 6f66 206f 6e6c 7920 7369 6e67 6c65 2063  of only single c
+00006150: 6f70 7920 6765 6e65 7320 6275 7420 6261  opy genes but ba
+00006160: 6374 6572 6961 6c20 6765 6e6f 6d65 7320  cterial genomes 
+00006170: 6172 6520 6479 6e61 6d69 6320 616e 6420  are dynamic and 
+00006180: 6765 6e75 696e 6520 6475 6c70 6c69 6361  genuine dulplica
+00006190: 7469 6f6e 7320 6361 6e20 6f63 6375 722c  tions can occur,
+000061a0: 2069 6e20 6164 6469 7469 6f6e 2074 6f20   in addition to 
+000061b0: 6173 7365 6d62 6c79 2061 7274 6966 6163  assembly artifac
+000061c0: 7473 2061 6e64 2063 6f6e 7461 6d69 6e61  ts and contamina
+000061d0: 7469 6f6e 2e20 5468 6572 6520 6172 6520  tion. There are 
+000061e0: 6120 7661 7269 6574 7920 6f66 2061 7070  a variety of app
+000061f0: 726f 6163 6865 7320 6176 6169 6c61 626c  roaches availabl
+00006200: 6520 746f 206d 616e 6167 6573 2074 6865  e to manages the
+00006210: 7365 2063 6173 6573 2e20 5769 7468 696e  se cases. Within
+00006220: 2074 6865 2037 2d67 656e 6520 5b6d 6c73   the 7-gene [mls
+00006230: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00006240: 622e 636f 6d2f 7473 6565 6d61 6e6e 2f6d  b.com/tseemann/m
+00006250: 6c73 7429 2074 6f6f 6c20 6d75 6c74 6970  lst) tool multip
+00006260: 6c65 2061 6c6c 656c 6573 2066 6f72 2061  le alleles for a
+00006270: 2067 6976 656e 206c 6f63 7573 2061 7265   given locus are
+00006280: 2072 6570 6f72 7465 6420 7769 7468 2061   reported with a
+00006290: 2063 6f6d 6d61 2064 656c 696d 6974 696e   comma delimitin
+000062a0: 6720 6561 6368 2061 6c6c 656c 652e 2048  g each allele. H
+000062b0: 6f77 6576 6572 2c20 7468 6973 2070 6f73  owever, this pos
+000062c0: 6573 2061 6e20 6973 7375 6520 666f 7220  es an issue for 
+000062d0: 6361 6c63 756c 6174 696e 6720 6765 6e65  calculating gene
+000062e0: 7469 6320 6469 7374 616e 6365 7320 7369  tic distances si
+000062f0: 6e63 6520 6974 2069 7320 756e 636c 6561  nce it is unclea
+00006300: 7220 686f 7720 746f 2074 7265 6174 2074  r how to treat t
+00006310: 6865 206d 756c 7469 706c 6520 616c 6c65  he multiple alle
+00006320: 6c65 732e 2054 6865 7265 2061 7265 2073  les. There are s
+00006330: 6576 6572 616c 2063 6f6d 6d6f 6e20 6d65  everal common me
+00006340: 7468 6f64 7320 666f 7220 686f 7720 746f  thods for how to
+00006350: 2074 7265 6174 206d 756c 7469 706c 6520   treat multiple 
+00006360: 616c 6c65 6c65 733a 0d0a 0d0a 3129 2074  alleles:....1) t
+00006370: 7265 6174 2074 6865 2063 6f6d 6269 6e61  reat the combina
+00006380: 7469 6f6e 2061 7320 6120 6e6f 7665 6c20  tion as a novel 
+00006390: 616c 6c65 6c65 200d 0a32 2920 626c 616e  allele ..2) blan
+000063a0: 6b20 7468 6520 636f 6c75 6d6e 200d 0a33  k the column ..3
+000063b0: 2920 7365 6c65 6374 2074 6865 2065 6172  ) select the ear
+000063c0: 6c69 6573 7420 616c 6c65 6c65 2069 6e20  liest allele in 
+000063d0: 7468 6520 6461 7461 6261 7365 200d 0a34  the database ..4
+000063e0: 2920 5573 6520 6120 7369 6d69 6c61 7269  ) Use a similari
+000063f0: 7479 2073 636f 7265 2074 6f20 7261 7465  ty score to rate
+00006400: 2077 6869 6368 2069 7320 7468 6520 6265   which is the be
+00006410: 7374 2061 6c6c 656c 6520 746f 2069 6e63  st allele to inc
+00006420: 6c75 6465 2e20 0d0a 0d0a 5468 6520 6d6f  lude. ....The mo
+00006430: 7374 2063 6f6e 7365 7276 6174 6976 6520  st conservative 
+00006440: 6170 7072 6f61 6368 2069 7320 746f 206e  approach is to n
+00006450: 6f74 2069 6e74 6572 7072 6574 2074 6861  ot interpret tha
+00006460: 7420 636f 6c75 6d6e 2062 7920 626c 616e  t column by blan
+00006470: 6b69 6e67 2069 7420 696e 2064 6973 7461  king it in dista
+00006480: 6e63 6520 6361 6c63 756c 6174 696f 6e73  nce calculations
+00006490: 2077 6869 6368 2072 6573 756c 7473 2069   which results i
+000064a0: 6e20 626c 756e 7469 6e67 2072 6573 6f6c  n blunting resol
+000064b0: 7574 696f 6e20 7768 6963 6820 6973 2069  ution which is i
+000064c0: 6d70 6c65 6d65 6e74 6564 2077 6974 6869  mplemented withi
+000064d0: 6e20 6c6f 6369 6465 7820 6173 2074 6865  n locidex as the
+000064e0: 2063 6f6e 7365 7276 6174 6976 6520 6d6f   conservative mo
+000064f0: 6465 2e20 416c 7465 726e 6174 6976 656c  de. Alternativel
+00006500: 792c 2062 7920 7573 696e 6720 616e 2061  y, by using an a
+00006510: 7070 726f 6163 6820 746f 2073 656c 6563  pproach to selec
+00006520: 7420 6f6e 6c79 206f 6e65 206f 6620 7468  t only one of th
+00006530: 6520 6c6f 6369 2074 6f20 6d61 7463 6820  e loci to match 
+00006540: 7769 6c6c 2068 6176 6520 6d69 7865 6420  will have mixed 
+00006550: 6566 6665 6374 7320 286f 7074 696f 6e73  effects (options
+00006560: 2033 2c20 3429 2074 6861 7420 6361 6e20   3, 4) that can 
+00006570: 7265 7375 6c74 2069 6e20 696e 636f 6e73  result in incons
+00006580: 6973 7465 6e63 6965 7320 7768 6572 6520  istencies where 
+00006590: 736f 6d65 2069 736f 6c61 7465 7320 6170  some isolates ap
+000065a0: 7065 6172 206d 6f72 6520 7369 6d69 6c61  pear more simila
+000065b0: 7220 6f72 2064 6973 7369 6d69 6c61 7220  r or dissimilar 
+000065c0: 7468 616e 2074 6865 7920 6172 652e 2054  than they are. T
+000065d0: 6865 2070 7265 6665 7272 6564 206d 6574  he preferred met
+000065e0: 686f 6420 7468 6174 206c 6f63 6964 6578  hod that locidex
+000065f0: 2068 6173 2069 6d70 6c65 6d65 6e74 6564   has implemented
+00006600: 2061 7320 6974 7320 5b44 4546 4155 4c54   as its [DEFAULT
+00006610: 5d20 286e 6f72 6d61 6c29 206d 6f64 6520  ] (normal) mode 
+00006620: 6973 2074 6f20 636f 6d62 696e 6520 7468  is to combine th
+00006630: 6520 7265 7375 6c74 2069 6e74 6f20 6120  e result into a 
+00006640: 6e65 7720 2261 6c6c 656c 6522 2068 6173  new "allele" has
+00006650: 6820 7468 6174 2069 7320 6465 7269 7665  h that is derive
+00006660: 6420 6672 6f6d 2063 616c 6375 6c61 7469  d from calculati
+00006670: 6e67 2074 6865 206d 6435 2068 6173 6820  ng the md5 hash 
+00006680: 6f66 2074 6865 2063 6f6e 6361 7465 6e61  of the concatena
+00006690: 7465 6420 616c 6c65 6c65 206d 6435 2068  ted allele md5 h
+000066a0: 6173 6865 732c 2073 6f72 7465 6420 616c  ashes, sorted al
+000066b0: 7068 6162 6574 6963 616c 6c79 2e20 5468  phabetically. Th
+000066c0: 6973 2068 6173 2074 6865 2062 656e 6566  is has the benef
+000066d0: 6974 206f 6620 7468 6520 7361 6d65 2063  it of the same c
+000066e0: 6f6d 6269 6e61 7469 6f6e 206f 6620 616c  ombination of al
+000066f0: 6c65 6c65 7320 2072 6573 756c 7469 6e67  leles  resulting
+00006700: 2069 6e20 7468 6520 7361 6d65 2068 6173   in the same has
+00006710: 6820 636f 6465 2061 6e64 2077 696c 6c20  h code and will 
+00006720: 6d61 7463 6820 7768 656e 2074 6869 7320  match when this 
+00006730: 6f63 6375 7273 2e20 436f 6e76 6572 7365  occurs. Converse
+00006740: 6c79 2c20 6974 2077 696c 6c20 636f 756e  ly, it will coun
+00006750: 7420 6120 6469 6666 6572 656e 6365 2065  t a difference e
+00006760: 7665 6e20 7768 656e 2069 6e64 6976 6964  ven when individ
+00006770: 7561 6c20 636f 6d70 6f6e 656e 7420 616c  ual component al
+00006780: 6c65 6c65 7320 6d61 7920 6d61 7463 6820  leles may match 
+00006790: 6265 7477 6565 6e20 7477 6f20 7361 6d70  between two samp
+000067a0: 6c65 732e 0d0a 0d0a 2320 4265 6e63 686d  les.....# Benchm
+000067b0: 6172 6b69 6e67 0d0a 0d0a 436f 6d69 6e67  arking....Coming
+000067c0: 2073 6f6f 6e2e 0d0a 0d0a 2320 4c65 6761   soon.....# Lega
+000067d0: 6c20 616e 6420 436f 6d70 6c69 616e 6365  l and Compliance
+000067e0: 2049 6e66 6f72 6d61 7469 6f6e 0d0a 0d0a   Information....
+000067f0: 436f 7079 7269 6768 7420 476f 7665 726e  Copyright Govern
+00006800: 6d65 6e74 206f 6620 4361 6e61 6461 2032  ment of Canada 2
+00006810: 3032 330d 0a0d 0a57 7269 7474 656e 2062  023....Written b
+00006820: 793a 204e 6174 696f 6e61 6c20 4d69 6372  y: National Micr
+00006830: 6f62 696f 6c6f 6779 204c 6162 6f72 6174  obiology Laborat
+00006840: 6f72 792c 2050 7562 6c69 6320 4865 616c  ory, Public Heal
+00006850: 7468 2041 6765 6e63 7920 6f66 2043 616e  th Agency of Can
+00006860: 6164 610d 0a0d 0a4c 6963 656e 7365 6420  ada....Licensed 
+00006870: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
+00006880: 204c 6963 656e 7365 2c20 5665 7273 696f   License, Versio
+00006890: 6e20 322e 3020 2874 6865 2022 4c69 6365  n 2.0 (the "Lice
+000068a0: 6e73 6522 293b 2079 6f75 206d 6179 206e  nse"); you may n
+000068b0: 6f74 2075 7365 2074 6869 7320 776f 726b  ot use this work
+000068c0: 2065 7863 6570 7420 696e 2063 6f6d 706c   except in compl
+000068d0: 6961 6e63 6520 7769 7468 2074 6865 204c  iance with the L
+000068e0: 6963 656e 7365 2e20 596f 7520 6d61 7920  icense. You may 
+000068f0: 6f62 7461 696e 2061 2063 6f70 7920 6f66  obtain a copy of
+00006900: 2074 6865 204c 6963 656e 7365 2061 743a   the License at:
+00006910: 0d0a 0d0a 5b68 7474 703a 2f2f 7777 772e  ....[http://www.
+00006920: 6170 6163 6865 2e6f 7267 2f6c 6963 656e  apache.org/licen
+00006930: 7365 732f 4c49 4345 4e53 452d 322e 305d  ses/LICENSE-2.0]
+00006940: 2868 7474 703a 2f2f 7777 772e 6170 6163  (http://www.apac
+00006950: 6865 2e6f 7267 2f6c 6963 656e 7365 732f  he.org/licenses/
+00006960: 4c49 4345 4e53 452d 322e 3029 0d0a 0d0a  LICENSE-2.0)....
+00006970: 556e 6c65 7373 2072 6571 7569 7265 6420  Unless required 
+00006980: 6279 2061 7070 6c69 6361 626c 6520 6c61  by applicable la
+00006990: 7720 6f72 2061 6772 6565 6420 746f 2069  w or agreed to i
+000069a0: 6e20 7772 6974 696e 672c 2073 6f66 7477  n writing, softw
+000069b0: 6172 6520 6469 7374 7269 6275 7465 6420  are distributed 
+000069c0: 756e 6465 7220 7468 6520 4c69 6365 6e73  under the Licens
+000069d0: 6520 6973 2064 6973 7472 6962 7574 6564  e is distributed
+000069e0: 206f 6e20 616e 2022 4153 2049 5322 2042   on an "AS IS" B
+000069f0: 4153 4953 2c20 5749 5448 4f55 5420 5741  ASIS, WITHOUT WA
+00006a00: 5252 414e 5449 4553 204f 5220 434f 4e44  RRANTIES OR COND
+00006a10: 4954 494f 4e53 204f 4620 414e 5920 4b49  ITIONS OF ANY KI
+00006a20: 4e44 2c20 6569 7468 6572 2065 7870 7265  ND, either expre
+00006a30: 7373 206f 7220 696d 706c 6965 642e 2053  ss or implied. S
+00006a40: 6565 2074 6865 204c 6963 656e 7365 2066  ee the License f
+00006a50: 6f72 2074 6865 2073 7065 6369 6669 6320  or the specific 
+00006a60: 6c61 6e67 7561 6765 2067 6f76 6572 6e69  language governi
+00006a70: 6e67 2070 6572 6d69 7373 696f 6e73 2061  ng permissions a
+00006a80: 6e64 206c 696d 6974 6174 696f 6e73 2075  nd limitations u
+00006a90: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
+00006aa0: 2e0d 0a0d 0a23 2055 7064 6174 6573 2061  .....# Updates a
+00006ab0: 6e64 2052 656c 6561 7365 204e 6f74 6573  nd Release Notes
+00006ac0: 3a0d 0a52 656c 6561 7365 206e 6f74 6573  :..Release notes
+00006ad0: 2068 6967 686c 6967 6874 696e 6720 6e65   highlighting ne
+00006ae0: 7720 6665 6174 7572 6573 2061 6e64 2063  w features and c
+00006af0: 6861 6e67 6573 2e0d 0a                   hanges...
```

### Comparing `locidex-0.1.1/locidex/build.py` & `locidex-0.1.2/locidex/build.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/__init__.py` & `locidex-0.1.2/locidex/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/aligner.py` & `locidex-0.1.2/locidex/classes/aligner.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/blast.py` & `locidex-0.1.2/locidex/classes/blast.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/db.py` & `locidex-0.1.2/locidex/classes/db.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/extractor.py` & `locidex-0.1.2/locidex/classes/extractor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import pandas as pd
 import numpy as np
 from locidex.constants import NT_SUB, STOP_CODONS, START_CODONS
 class extractor:
     seqs = {}
     df = pd.DataFrame()
-    def __init__(self,df,seq_data,sseqid_col,queryid_col,qstart_col,qend_col,qlen_col,sstart_col,send_col,slen_col,sstrand_col,bitscore_col,overlap_thresh=1,extend_threshold_ratio = 0.2,filter_contig_breaks=True):
+    def __init__(self,df,seq_data,sseqid_col,queryid_col,qstart_col,qend_col,qlen_col,sstart_col,send_col,slen_col,sstrand_col,bitscore_col,overlap_thresh=100,extend_threshold_ratio = 0.2,filter_contig_breaks=True):
+        print('hi')
         self.filter_contig_breaks = filter_contig_breaks
         self.df = self.set_extraction_pos(df, sstart_col, send_col)
         self.is_complete(self.df,qstart_col,qend_col,qlen_col)
         self.is_contig_boundary(self.df,'ext_start','ext_end',slen_col)
         if filter_contig_breaks:
             self.df = df[ (df['is_5prime_boundary'] == False) & (df['is_3prime_boundary'] == False)]
             self.df = self.df.reset_index(drop=True)
         self.set_revcomp(self.df,sstart_col,send_col,sstrand_col)
         pcols = [qstart_col,qend_col,sstart_col,send_col]
         for c in pcols:
             self.df[c] = self.df[c].apply(lambda x: x - 1)
         #self.df = self.fix_postioning(self.df)
 
-        sort_cols = [sseqid_col, queryid_col, sstart_col, send_col, bitscore_col]
+        sort_cols = ['locus_name', sseqid_col, sstart_col, send_col, bitscore_col]
         ascending_cols = [True, True, True, True, False]
+        self.df = self.df.sort_values(sort_cols,ascending=ascending_cols).reset_index(drop=True)
+        self.df = self.recursive_filter_redundant_queries(self.df, 'locus_name', sseqid_col, bitscore_col, 
+                                                          sort_cols, ascending_cols, overlap_threshold=1)
+
         #self.df = self.recursive_filter_overlap_records(self.df, sseqid_col, bitscore_col, sort_cols, ascending_cols, overlap_threshold=overlap_thresh)
-        self.df = self.extend(self.df,sseqid_col, queryid_col, qstart_col, qend_col, sstart_col,send_col,slen_col, qlen_col, bitscore_col, overlap_threshold=1)
+        self.df = self.extend(self.df,sseqid_col, queryid_col, qstart_col, qend_col, sstart_col,send_col,slen_col, qlen_col, bitscore_col, overlap_threshold=overlap_thresh)
 
         #self.df = self.recursive_filter_overlap_records(self.df, sseqid_col, bitscore_col, sort_cols, ascending_cols,
         #                                                overlap_threshold=overlap_thresh)
         self.df = self.set_extraction_pos(self.df, sstart_col, send_col)
         loci_ranges = self.group_by_locus(self.df,sseqid_col, queryid_col,qlen_col,extend_threshold_ratio)
         self.seqs = self.extract_seq(loci_ranges, seq_data)
         pass
@@ -60,14 +65,80 @@
                 tmp = end
                 end = start
                 start = tmp
                 df.loc[idx, 'ext_start'] = start
                 df.loc[idx, 'ext_end'] = end
         return df
 
+    def recursive_filter_redundant_queries(self,df, locus_col, sseqid_col, bitscore_col, sort_cols, ascending_cols, overlap_threshold=1):
+        size = len(df)
+        prev_size = 0
+        while size != prev_size:
+            df = df.sort_values(sort_cols,
+                                ascending=ascending_cols).reset_index(drop=True)
+            df = self.remove_redundant_queries(df, locus_col, sseqid_col, bitscore_col, overlap_threshold=overlap_threshold)
+            prev_size = size
+            size = len(df)
+
+        return df.sort_values(sort_cols,ascending=ascending_cols).reset_index(drop=True)
+
+    def remove_redundant_queries(self,df,locus_col,sseqid_col, bitscore_col, overlap_threshold=1):
+        seq_id_list = list(df[sseqid_col].unique())
+        filter_df = []
+        for seqid in seq_id_list:
+            subset = df[df[sseqid_col] == seqid]
+            prev_locus_id = ''
+            prev_contig_id = ''
+            prev_index = -1
+            prev_contig_start = -1
+            prev_contig_end = -1
+            prev_score = 0
+            filter_rows = []
+            for idx, row in subset.iterrows():
+                contig_id = row[sseqid_col]
+                contig_start = row['ext_start']
+                contig_end = row['ext_end']
+                score = float(row[bitscore_col])
+                locus_id = row[locus_col]
+
+                if prev_contig_id == '':
+                    prev_index = idx
+                    prev_contig_id = contig_id
+                    prev_contig_start = contig_start
+                    prev_contig_end = contig_end
+                    prev_score = score
+                    prev_locus_id = locus_id
+                    continue
+
+                if locus_id == prev_locus_id:
+                    if (contig_start >= prev_contig_start and contig_start <= prev_contig_end) or (
+                            contig_end >= prev_contig_start and contig_end <= prev_contig_end):
+                        overlap = abs(contig_start - prev_contig_end)
+
+                        if overlap > overlap_threshold:
+                            if prev_score < score:
+                                filter_rows.append(prev_index)
+                            else:
+                                filter_rows.append(idx)
+
+                prev_index = idx
+                prev_contig_id = contig_id
+                prev_contig_start = contig_start
+                prev_contig_end = contig_end
+                prev_score = score
+                prev_locus_id = locus_id
+
+
+            valid_ids = list( set(subset.index) - set(filter_rows)  )
+
+            filter_df.append(subset.filter(valid_ids, axis=0))
+
+
+        return pd.concat(filter_df, ignore_index=True)
+
     def fix_postioning(self,df):
         for idx, row in df.iterrows():
             start = row['ext_start']
             end = row['ext_end']
             rev = row['reverse']
             complement = row['complement']
 
@@ -208,17 +279,18 @@
                                  'seq':seq,'start_codon':start_codon,'stop_codon':stop_codon,
                                  'is_stop_valid':is_stop_valid,'is_start_valid':is_start_valid,
                                  'is_cds_valid':cds_valid})
                     id+=1
         return seqs
 
     def extend(self,df,seqid_col, queryid_col, qstart_col, qend_col, sstart_col,send_col,slen_col, qlen_col, bitscore_col, overlap_threshold=1):
-        sort_cols = [seqid_col,'ext_start', 'ext_end', bitscore_col]
-        ascending_cols = [True, True, True, False]
-        df = self.recursive_filter_overlap_records(df, seqid_col, bitscore_col, sort_cols, ascending_cols, overlap_threshold)
+        sort_cols = ['locus_name',seqid_col,'ext_start', 'ext_end', bitscore_col]
+        ascending_cols = [True, True, True, True, False]
+
+        df = self.recursive_filter_overlap_records(df, 'locus_name', bitscore_col, sort_cols, ascending_cols, overlap_threshold)
         df = df.sort_values(sort_cols,
                             ascending=ascending_cols).reset_index(drop=True)
 
         queries = df[queryid_col].to_list()
 
         #Remove incomplete hits when complete ones are present
         filtered = []
@@ -304,14 +376,15 @@
 
         df['is_extended'] = is_extended
         df['is_5p_extended'] = five_p_ext
         df['is_3p_extended'] = three_p_ext
         return df
 
     def group_by_locus(self,df,seqid_col,query_col,qlen_col,extend_threshold_ratio = 0.2):
+        print(self.df.columns)
         sort_cols = ['locus_name',query_col,'ext_start', 'ext_end']
         ascending_cols = [True, True, True, True]
         df = df.sort_values(sort_cols,
                             ascending=ascending_cols).reset_index(drop=True)
 
         queries = df['qseqid'].to_list()
```

### Comparing `locidex-0.1.1/locidex/classes/fasta.py` & `locidex-0.1.2/locidex/classes/fasta.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/gbk.py` & `locidex-0.1.2/locidex/classes/gbk.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/mafft.py` & `locidex-0.1.2/locidex/classes/mafft.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/metadata.py` & `locidex-0.1.2/locidex/classes/metadata.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/prodigal.py` & `locidex-0.1.2/locidex/classes/prodigal.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/classes/seq_intake.py` & `locidex-0.1.2/locidex/classes/seq_intake.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/constants.py` & `locidex-0.1.2/locidex/constants.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/extract.py` & `locidex-0.1.2/locidex/extract.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/format.py` & `locidex-0.1.2/locidex/format.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/main.py` & `locidex-0.1.2/locidex/main.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/merge.py` & `locidex-0.1.2/locidex/merge.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/report.py` & `locidex-0.1.2/locidex/report.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,41 +18,43 @@
 
     parser = ArgumentParser(
         description="Locidex: Advanced searching and filtering of sequence databases using query sequences",
         formatter_class=CustomFormatter)
     parser.add_argument('-i','--input', type=str, required=True,help='Input file to report')
     parser.add_argument('-o', '--outdir', type=str, required=True, help='Output file to put results')
     parser.add_argument('-n', '--name', type=str, required=False, help='Sample name to include default=filename')
-    parser.add_argument('-m', '--mode', type=str, required=False, help='Allele profile assignment [normal,conservative]',default='normal')
+    parser.add_argument('-m', '--mode', type=str, required=False, help='Allele profile assignment [normal,conservative,fuzzy]',default='normal')
     parser.add_argument('-p', '--prop', type=str, required=False, help='Metadata label to use for aggregation',default='locus_name')
     parser.add_argument('-a', '--max_ambig', type=int, required=False, help='Maximum number of ambiguous characters allowed in a sequence',default=0)
     parser.add_argument('-s', '--max_stop', type=int, required=False, help='Maximum number of internal stop codons allowed in a sequence',default=0)
     parser.add_argument('--report_format', type=str, required=False,
                         help='Report format of parsed results [profile]',default='profile')
-
+    parser.add_argument('-r', '--match_ident', type=float, required=False, 
+                        help='Report match allele if percent difference is less than this value',default=100)
     parser.add_argument('-V', '--version', action='version', version="%(prog)s " + __version__)
     parser.add_argument('-f', '--force', required=False, help='Overwrite existing directory',
                         action='store_true')
 
     return parser.parse_args()
 
 
 class seq_reporter:
     data_dict = {}
     profile = {}
     loci = {}
     db_seq_info = {}
     failed_seqids = set()
 
-    def __init__(self,data_dict,method='nucleotide',mode='normal',label='locus_name',filters={},max_ambig=0,max_int_stop=0):
+    def __init__(self,data_dict,method='nucleotide',mode='normal',label='locus_name',filters={},max_ambig=0,max_int_stop=0,match_ident=0):
         self.max_ambig_count = max_ambig
         self.max_int_stop_count = max_int_stop
         self.label = label
         self.method = method
         self.mode = mode
+        self.match_ident = match_ident
         self.data_dict = data_dict
         self.db_seq_info = self.data_dict["db_seq_info"]
         self.query_seq_data = self.data_dict["query_data"]['query_seq_data']
         self.query_hits = self.data_dict["query_data"]["query_hits"]
         self.locus_profile = self.data_dict['query_data']["locus_profile"]
         self.blast_columns = self.data_dict["query_hit_columns"]
         self.build_profile()
@@ -138,28 +140,29 @@
                 self.query_hits[qid][dbtype] = filt
 
     def calc_query_best_hit(self):
         best_hits = {}
         for qid in self.query_hits:
             best_hits[qid] = {}
             for dbtype in self.query_hits[qid]:
-                best_hits[dbtype] = []
+                best_hits[qid][dbtype] = []
                 hit_ids = []
                 hit_bit = []
                 for hit in self.query_hits[qid][dbtype]:
                     hit_ids.append(str(hit['sseqid']))
                     hit_bit.append(hit['bitscore'])
                 if len(hit_bit) == 0:
                     continue
                 max_bit = max(hit_bit)
                 top_ids = []
                 for idx, value in enumerate(hit_bit):
-                    if value == max_bit:
+                    if value >= max_bit:
                         top_ids.append(idx)
-                best_hits[dbtype] = top_ids
+                best_hits[qid][dbtype] = top_ids
+
         return best_hits
 
     def get_hit_locinames(self):
         hit_names = {}
         for qid in self.query_hits:
             hit_names[qid] = {}
             for dbtype in self.query_hits[qid]:
@@ -179,15 +182,16 @@
             for l in hit_names[qid][dbtype]:
                 if not l in loci_lookup:
                     loci_lookup[l] = []
                 loci_lookup[l].append(qid)
         return loci_lookup
 
     def allele_assignment(self,dbtype):
-        query_best_hits = self.calc_query_best_hit()
+        self.query_best_hits = self.calc_query_best_hit()
+
         hit_loci_names = self.get_hit_locinames()
         loci_lookup = self.get_loci_to_query_map(hit_loci_names,dbtype)
 
         for locus in loci_lookup:
             loci_lookup[locus] = list(set(loci_lookup[locus]) - self.failed_seqids)
 
 
@@ -213,51 +217,76 @@
             matches = loci_lookup[locus_name ]
             num_matches = len(matches)
             if num_matches <= 1:
                 assigned_loci.add(locus_name)
                 continue
 
             for qid in matches:
-                if not dbtype in query_best_hits[qid]:
+                if not dbtype in self.query_best_hits[qid]:
                     continue
-                best_hits = query_best_hits[qid][dbtype]
+                best_hits = self.query_best_hits[qid][dbtype]
                 best_hit_names = set()
                 for l in best_hits:
+                    l = str(l)
                     hinfo = self.db_seq_info[l]
                     best_hit_names.add(hinfo['locus_name'])
                 if len(best_hit_names) == 1:
                     continue
                 if locus_name not in best_hit_names:
                     if qid in profile[locus_name]:
                         del(profile[locus_name][qid])
 
         self.locus_profile = profile
         self.populate_profile()
 
+
+    def get_matching_ref_seq_info(self,qid, dbtype):
+        for hit in self.query_hits[qid][dbtype]:
+            hit_id = str(hit['sseqid'])
+            pident = hit['pident']
+            if pident < self.match_ident:
+                    continue
+            hinfo = self.db_seq_info[hit_id]
+            hit_name = hinfo['locus_name']
+            return hinfo
+        return {}
+    
     def populate_profile(self):
         for locus_name in self.profile:
             values = set()
             if locus_name in self.locus_profile:
                 values = set(self.locus_profile[locus_name][self.method])
             allele_hashes = []
             for seq_id in values:
                 if self.method == 'nucleotide':
                     key = "dna_hash"
                 elif self.method == 'protein':
                     key = "aa_hash"
-                allele_hashes.append(self.query_seq_data[seq_id][key])
+                hash_value = self.query_seq_data[seq_id][key]
+                if self.mode == 'fuzzy':
+                    ref_seq_hitinfo = self.get_matching_ref_seq_info(seq_id, self.method)
+                    if len(ref_seq_hitinfo) > 0:
+                        if self.method == 'nucleotide':
+                            hash_value = ref_seq_hitinfo['dna_seq_hash']  
+                        elif self.method == 'protein':
+                            hash_value = ref_seq_hitinfo['aa_seq_hash'] 
+                            
+                allele_hashes.append(hash_value)
 
             num_alleles = len(allele_hashes)
             if num_alleles > 1 and self.mode == 'conservative':
                 allele_hashes = ['-']
             elif num_alleles > 1 and self.mode == 'normal':
                 allele_hashes = calc_md5(["".join([str(x) for x in sorted(allele_hashes)])])
             elif num_alleles == 0:
                 allele_hashes = ['-']
+            elif self.mode == 'fuzzy':
+                allele_hashes = calc_md5(["".join([str(x) for x in sorted(allele_hashes)])])
             self.profile[locus_name] = ",".join(list(set([str(x) for x in allele_hashes])))
+        
 
 
     def extract_hit_data(self,dbtype):
         data = []
         for qid in self.query_hits:
             query_name = self.query_seq_data[qid][self.label]
             for hit in self.query_hits[qid][dbtype]:
@@ -283,14 +312,15 @@
     label = cmd_args.prop
     report_format = cmd_args.report_format
     sample_name = cmd_args.name
     force = cmd_args.force
     mode = cmd_args.mode
     max_ambig = cmd_args.max_ambig
     max_int_stop = cmd_args.max_stop
+    match_ident = cmd_args.match_ident
 
 
     if sample_name is None:
         sample_name = '.'.join(os.path.basename(input_file).split('.')[:-1])
 
     run_data = SEARCH_RUN_DATA
     run_data['analysis_start_time'] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
@@ -306,15 +336,15 @@
     seq_store_dict = {}
     with open(input_file ,'r') as fh:
         seq_store_dict = json.load(fh)
 
     if len(seq_store_dict) == 0:
         sys.exit()
 
-    allele_obj = seq_reporter(seq_store_dict, method='nucleotide', mode=mode, label=label, filters={},max_ambig=max_ambig,max_int_stop=max_int_stop)
+    allele_obj = seq_reporter(seq_store_dict, method='nucleotide', mode=mode, label=label, filters={},max_ambig=max_ambig,max_int_stop=max_int_stop,match_ident=match_ident)
 
 
     if report_format == 'profile':
         allele_obj.filter_queries()
         allele_obj.allele_assignment('nucleotide')
         profile = {sample_name: allele_obj.profile}
         with open(os.path.join(outdir,"profile.json"),"w") as out:
```

### Comparing `locidex-0.1.1/locidex/search.py` & `locidex-0.1.2/locidex/search.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex/utils.py` & `locidex-0.1.2/locidex/utils.py`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/locidex.egg-info/PKG-INFO` & `locidex-0.1.2/locidex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: locidex
-Version: 0.1.1
+Version: 0.1.2
 Summary: Genomic Address Service: De novo clustering and cluster address assignment
 Home-page: https://github.com/phac-nml/locidex
 Author: James Robertson
 Author-email: james.robertson@phac-aspc.gc.ca
 License: GPLv3
 Description: UNKNOWN
 Keywords: cgMLST,wgMLST,outbreak,surveillance,blast,antimicrobial resistance,amr,virulence
```

### Comparing `locidex-0.1.1/locidex.egg-info/SOURCES.txt` & `locidex-0.1.2/locidex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locidex-0.1.1/setup.py` & `locidex-0.1.2/setup.py`

 * *Files identical despite different names*

