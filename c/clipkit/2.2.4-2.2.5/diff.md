# Comparing `tmp/clipkit-2.2.4.tar.gz` & `tmp/clipkit-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipkit-2.2.4.tar", last modified: Wed Mar  6 19:52:55 2024, max compression
+gzip compressed data, was "clipkit-2.2.5.tar", last modified: Thu Apr  4 03:23:04 2024, max compression
```

## Comparing `clipkit-2.2.4.tar` & `clipkit-2.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-03-06 19:52:55.611712 clipkit-2.2.4/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-2.2.4/LICENSE.md
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-03-06 19:52:55.611505 clipkit-2.2.4/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4564 2024-02-07 15:51:48.000000 clipkit-2.2.4/README.md
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-03-06 19:52:55.610331 clipkit-2.2.4/clipkit/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       25 2023-07-21 16:57:06.000000 clipkit-2.2.4/clipkit/__init__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-2.2.4/clipkit/__main__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2059 2024-03-06 19:22:29.000000 clipkit-2.2.4/clipkit/api.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1769 2024-03-06 19:22:29.000000 clipkit-2.2.4/clipkit/args_processing.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5094 2024-03-06 19:22:29.000000 clipkit-2.2.4/clipkit/clipkit.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      103 2023-07-21 16:57:06.000000 clipkit-2.2.4/clipkit/exceptions.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1548 2024-03-06 19:22:29.000000 clipkit-2.2.4/clipkit/files.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2330 2024-03-04 23:25:45.000000 clipkit-2.2.4/clipkit/helpers.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      193 2023-07-21 16:57:06.000000 clipkit-2.2.4/clipkit/logger.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      438 2024-03-06 19:22:29.000000 clipkit-2.2.4/clipkit/modes.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)    10424 2024-03-06 19:22:29.000000 clipkit-2.2.4/clipkit/msa.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     9264 2024-03-06 19:51:16.000000 clipkit-2.2.4/clipkit/parser.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      108 2024-03-06 19:44:41.000000 clipkit-2.2.4/clipkit/settings.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1538 2023-09-24 21:24:47.000000 clipkit-2.2.4/clipkit/site_classification.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2267 2024-02-18 20:23:57.000000 clipkit-2.2.4/clipkit/smart_gap_helper.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      912 2023-09-24 21:24:47.000000 clipkit-2.2.4/clipkit/stats.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2024-03-06 19:52:27.000000 clipkit-2.2.4/clipkit/version.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      648 2023-09-24 21:24:47.000000 clipkit-2.2.4/clipkit/warnings.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2388 2024-02-13 00:05:53.000000 clipkit-2.2.4/clipkit/write.py
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-03-06 19:52:55.611230 clipkit-2.2.4/clipkit.egg-info/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-03-06 19:52:55.000000 clipkit-2.2.4/clipkit.egg-info/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      596 2024-03-06 19:52:55.000000 clipkit-2.2.4/clipkit.egg-info/SOURCES.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2024-03-06 19:52:55.000000 clipkit-2.2.4/clipkit.egg-info/dependency_links.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       49 2024-03-06 19:52:55.000000 clipkit-2.2.4/clipkit.egg-info/entry_points.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       37 2024-03-06 19:52:55.000000 clipkit-2.2.4/clipkit.egg-info/requires.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2024-03-06 19:52:55.000000 clipkit-2.2.4/clipkit.egg-info/top_level.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2024-03-06 19:52:55.611755 clipkit-2.2.4/setup.cfg
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1211 2024-02-18 20:19:59.000000 clipkit-2.2.4/setup.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-04 03:23:04.954371 clipkit-2.2.5/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-2.2.5/LICENSE.md
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-04 03:23:04.954180 clipkit-2.2.5/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4564 2024-02-07 15:51:48.000000 clipkit-2.2.5/README.md
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-04 03:23:04.953203 clipkit-2.2.5/clipkit/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       25 2023-07-21 16:57:06.000000 clipkit-2.2.5/clipkit/__init__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-2.2.5/clipkit/__main__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2129 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/api.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1849 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/args_processing.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5499 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/clipkit.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      103 2023-07-21 16:57:06.000000 clipkit-2.2.5/clipkit/exceptions.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2198 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/files.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2330 2024-03-04 23:25:45.000000 clipkit-2.2.5/clipkit/helpers.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      193 2023-07-21 16:57:06.000000 clipkit-2.2.5/clipkit/logger.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      563 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/modes.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)    10486 2024-04-04 03:22:22.000000 clipkit-2.2.5/clipkit/msa.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     9703 2024-04-02 18:24:46.000000 clipkit-2.2.5/clipkit/parser.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      108 2024-03-18 22:22:33.000000 clipkit-2.2.5/clipkit/settings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1538 2023-09-24 21:24:47.000000 clipkit-2.2.5/clipkit/site_classification.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2267 2024-02-18 20:23:57.000000 clipkit-2.2.5/clipkit/smart_gap_helper.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      912 2023-09-24 21:24:47.000000 clipkit-2.2.5/clipkit/stats.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2024-04-04 03:22:40.000000 clipkit-2.2.5/clipkit/version.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      648 2023-09-24 21:24:47.000000 clipkit-2.2.5/clipkit/warnings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2388 2024-02-13 00:05:53.000000 clipkit-2.2.5/clipkit/write.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-04 03:23:04.953891 clipkit-2.2.5/clipkit.egg-info/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      596 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       49 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/entry_points.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       37 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/requires.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2024-04-04 03:23:04.000000 clipkit-2.2.5/clipkit.egg-info/top_level.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2024-04-04 03:23:04.954420 clipkit-2.2.5/setup.cfg
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1211 2024-02-18 20:19:59.000000 clipkit-2.2.5/setup.py
```

### Comparing `clipkit-2.2.4/LICENSE.md` & `clipkit-2.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/PKG-INFO` & `clipkit-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipkit Version: 2.2.4 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.2.5 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE.md Requires-Dist: biopython>=1.81 Requires-Dist:
```

### Comparing `clipkit-2.2.4/README.md` & `clipkit-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/clipkit/api.py` & `clipkit-2.2.5/clipkit/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,20 +38,22 @@
     if not output_file_path:
         output_temp_file = NamedTemporaryFile()
 
     # override some options not currently available through programmatic interface
     complement = False
     use_log = False
     quiet = True
+    auxiliary_file = None  # TODO: implement?
 
     trim_run, stats = run(
         input_temp_file.name if input_temp_file else input_file_path,
         input_file_format,
         output_temp_file.name if output_temp_file else output_file_path,
         output_file_format,
+        auxiliary_file,
         sequence_type,
         gaps,
         gap_characters,
         complement,
         codon,
         TrimmingMode(mode),
         use_log,
```

### Comparing `clipkit-2.2.4/clipkit/args_processing.py` & `clipkit-2.2.5/clipkit/args_processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     complement = args.complementary or False
     codon = args.codon or False
     mode = TrimmingMode(args.mode) if args.mode else TrimmingMode.smart_gap
     gaps = float(args.gaps) if args.gaps is not None else 0.9
     gap_characters = (
         [c for c in args.gap_characters] if args.gap_characters is not None else None
     )
+    auxiliary_file = args.auxiliary_file
     use_log = args.log or False
     quiet = args.quiet or False
     sequence_type = SeqType(args.sequence_type.lower()) if args.sequence_type else None
 
     if codon and mode == TrimmingMode.c3:
         logger.warning(
             "C3 and codon-based trimming are incompatible.\nCodon-based trimming removes whole codons while C3 removes every third codon position."
@@ -43,14 +44,15 @@
         sys.exit()
 
     return dict(
         input_file=input_file,
         output_file=output_file,
         input_file_format=args.input_file_format,
         output_file_format=args.output_file_format,
+        auxiliary_file=auxiliary_file,
         codon=codon,
         sequence_type=sequence_type,
         complement=complement,
         gaps=gaps,
         gap_characters=gap_characters,
         mode=mode,
         use_log=use_log,
```

### Comparing `clipkit-2.2.4/clipkit/clipkit.py` & `clipkit-2.2.5/clipkit/clipkit.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import sys
 import time
 from typing import Union
 
 from Bio.Align import MultipleSeqAlignment
 from .args_processing import process_args
 from .exceptions import InvalidInputFileFormat
-from .files import get_alignment_and_format, FileFormat, write_debug_log_file
+from .files import (
+    get_alignment_and_format,
+    FileFormat,
+    write_debug_log_file,
+    get_custom_sites_to_trim,
+)
 from .helpers import (
     create_msa,
     get_seq_type,
     get_gap_chars,
     write_msa,
     write_complement,
     SeqType,
@@ -59,14 +64,15 @@
 
 
 def run(
     input_file: str,
     input_file_format: FileFormat,
     output_file: str,
     output_file_format: FileFormat,
+    auxiliary_file: str,
     sequence_type: Union[SeqType, None],
     gaps: float,
     gap_characters: Union[list, None],
     complement: bool,
     codon: bool,
     mode: TrimmingMode,
     use_log: bool,
@@ -95,16 +101,28 @@
     if mode in {
         TrimmingMode.smart_gap,
         TrimmingMode.kpi_smart_gap,
         TrimmingMode.kpic_smart_gap,
     }:
         gaps = smart_gap_threshold_determination(alignment, gap_characters)
 
+    site_positions_to_trim = None
+    if mode == TrimmingMode.cst:
+        aln_length = len(alignment)
+        site_positions_to_trim = (
+            get_custom_sites_to_trim(auxiliary_file, aln_length) or []
+        )
+
     msa = create_msa(alignment, gap_characters)
-    msa.trim(mode, gap_threshold=gaps, site_positions_to_trim=None, codon=codon)
+    msa.trim(
+        mode,
+        gap_threshold=gaps,
+        site_positions_to_trim=site_positions_to_trim,
+        codon=codon,
+    )
 
     trim_run = TrimRun(
         alignment,
         msa,
         gap_characters,
         sequence_type,
         input_file_format,
@@ -125,14 +143,15 @@
     gaps: float,
     gap_characters: Union[list, None],
     complement: bool,
     codon: bool,
     mode: TrimmingMode,
     use_log: bool,
     quiet: bool,
+    auxiliary_file: str = None,
     **kwargs,
 ) -> None:
     if use_log:
         log_file_logger.setLevel(logging.DEBUG)
         log_file_logger.propagate = False
         fh = logging.FileHandler(f"{output_file}.log", mode="w")
         fh.setLevel(logging.DEBUG)
@@ -145,14 +164,15 @@
     start_time = time.time()
 
     trim_run, stats = run(
         input_file,
         input_file_format,
         output_file,
         output_file_format,
+        auxiliary_file,
         sequence_type,
         gaps,
         gap_characters,
         complement,
         codon,
         mode,
         use_log,
```

### Comparing `clipkit-2.2.4/clipkit/files.py` & `clipkit-2.2.5/clipkit/files.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from .logger import log_file_logger
 
 from Bio import AlignIO
 from Bio.Align import MultipleSeqAlignment
+import numpy as np
 
 from .exceptions import InvalidInputFileFormat
 
 
 class FileFormat(Enum):
     fasta = "fasta"
     clustal = "clustal"
@@ -42,10 +43,33 @@
                 continue
             except AssertionError:
                 continue
 
         raise InvalidInputFileFormat("File could not be read")
 
 
+def get_custom_sites_to_trim(file_path: str, aln_length: int) -> list:
+    with open(file_path) as f:
+        lines = f.read().splitlines()
+
+    sites_to_trim = []
+    sites_to_keep = []
+    for line in lines:
+        site = line.split("\t")
+        pos = int(site[0]) - 1
+        if site[1] == "trim":
+            sites_to_trim.append(pos)
+        else:
+            sites_to_keep.append(pos)
+
+    if len(sites_to_trim) == 0:
+        # we only had keeps so treat every other site as a trim
+        sites_to_trim = list(
+            np.setdiff1d(np.arange(aln_length), np.array(sites_to_keep))
+        )
+
+    return sites_to_trim
+
+
 def write_debug_log_file(msa):
     for info in msa.generate_debug_log_info():
         log_file_logger.debug(f"{str(info[0] + 1)} {info[1]} {info[2].value} {info[3]}")
```

### Comparing `clipkit-2.2.4/clipkit/helpers.py` & `clipkit-2.2.5/clipkit/helpers.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/clipkit/msa.py` & `clipkit-2.2.5/clipkit/msa.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,17 +122,18 @@
             )
         else:
             self._site_positions_to_trim = self.determine_site_positions_to_trim(
                 mode,
                 gap_threshold,
                 codon,
             )
-        self._site_positions_to_keep = np.delete(
-            np.arange(self._original_length), self._site_positions_to_trim
-        )
+        if len(self._site_positions_to_trim) > 0:
+            self._site_positions_to_keep = np.delete(
+                np.arange(self._original_length), self._site_positions_to_trim
+            )
 
     @property
     def column_character_frequencies(self):
         if self._column_character_frequencies is not None:
             return self._column_character_frequencies
 
         column_character_frequencies = []
```

### Comparing `clipkit-2.2.4/clipkit/parser.py` & `clipkit-2.2.5/clipkit/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
                     gappy,                          (default: smart-gap)
                     kpic,
                     kpic-smart-gap,           
                     kpic-gappy,                
                     kpi,
                     kpi-smart-gap,
                     kpi-gappy,
+                    cst,
                     c3>                      
                                                     
         -g, --gaps <threshold_of_gaps>              specifies gaps threshold
                                                     (default: 0.9)
 
         -gc, --gap_characters <string_of_gap_chars> specifies gap characters used in input file
                                                     (default for aa: Xx-?*
@@ -91,36 +92,41 @@
 
         -of, --output_file_format <file_format>     specifies output file format
                                                     (default: same as input file format)
 
         -l, --log                                   creates a log file
                                                     (input file named with '.log' suffix)
 
+        -a, --auxiliary_file                        auxiliary file with meta-information for various trimming
+                                                    modes (e.g., user-specified)
+
         -c, --complementary                         creates complementary alignment of trimmed sequences
                                                     (input file named with '.log' suffix)
 
         -co, --codon                                conduct trimming of codons
 
         -q, --quiet                                 disables all logging to stdout
 
         -h, --help                                  help message
         -v, --version                               print version
 
+
         -------------------------------------
         | Detailed explanation of arguments | 
         -------------------------------------
         Modes
             smart-gap: dynamic determination of gaps threshold
             gappy: trim sites that are greater than the gaps threshold
             kpic: keeps parismony informative and constant sites
             kpic-smart-gap: a combination of kpic- and smart-gap-based trimming
             kpic-gappy: a combination of kpic- and gappy-based trimming
             kpi: keep only parsimony informative sites
             kpi-smart-gap: a combination of kpi- and smart-gap-based trimming
             kpi-gappy: a combination of kpi- and gappy-based trimming
+            cst: custom site trimming specified using a tab-delimited text file
             c3: remove every third codon position
 
         Gaps
             Positions with gappyness greater than threshold will be trimmed. 
             Must be between 0 and 1. (Default: 0.9). This argument is ignored
             when using the kpi and kpic mdoes of trimming as well as an 
             iteration of trimming that uses smart-gap.
@@ -244,14 +250,22 @@
         required=False,
         choices=file_format_choices,
         help=SUPPRESS,
         metavar="",
     )
 
     optional.add_argument(
+        "-a",
+        "--auxiliary_file",
+        type=str,
+        required=False,
+        help=SUPPRESS,
+    )
+
+    optional.add_argument(
         "-l",
         "--log",
         action="store_true",
         required=False,
         help=SUPPRESS,
     )
```

### Comparing `clipkit-2.2.4/clipkit/site_classification.py` & `clipkit-2.2.5/clipkit/site_classification.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/clipkit/smart_gap_helper.py` & `clipkit-2.2.5/clipkit/smart_gap_helper.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/clipkit/stats.py` & `clipkit-2.2.5/clipkit/stats.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/clipkit/warnings.py` & `clipkit-2.2.5/clipkit/warnings.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/clipkit/write.py` & `clipkit-2.2.5/clipkit/write.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/clipkit.egg-info/PKG-INFO` & `clipkit-2.2.5/clipkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clipkit Version: 2.2.4 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.2.5 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
 markdown License-File: LICENSE.md Requires-Dist: biopython>=1.81 Requires-Dist:
```

### Comparing `clipkit-2.2.4/clipkit.egg-info/SOURCES.txt` & `clipkit-2.2.5/clipkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.4/setup.py` & `clipkit-2.2.5/setup.py`

 * *Files identical despite different names*

