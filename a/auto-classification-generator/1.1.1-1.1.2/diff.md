# Comparing `tmp/auto_classification_generator-1.1.1.tar.gz` & `tmp/auto_classification_generator-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_classification_generator-1.1.1.tar", last modified: Thu Apr  4 10:25:47 2024, max compression
+gzip compressed data, was "auto_classification_generator-1.1.2.tar", last modified: Thu Apr  4 10:33:14 2024, max compression
```

## Comparing `auto_classification_generator-1.1.1.tar` & `auto_classification_generator-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:25:47.965153 auto_classification_generator-1.1.1/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0      642 2024-04-04 10:25:47.963152 auto_classification_generator-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5494 2024-02-20 15:40:54.000000 auto_classification_generator-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 10:25:47.924712 auto_classification_generator-1.1.1/auto_classification_generator/
--rw-rw-rw-   0        0        0      408 2024-02-20 15:29:18.000000 auto_classification_generator-1.1.1/auto_classification_generator/__init__.py
--rw-rw-rw-   0        0        0    14871 2024-04-04 09:56:06.000000 auto_classification_generator-1.1.1/auto_classification_generator/classification_generator.py
--rw-rw-rw-   0        0        0     2608 2024-04-04 10:19:07.000000 auto_classification_generator-1.1.1/auto_classification_generator/cli.py
--rw-rw-rw-   0        0        0     2224 2024-03-20 15:06:23.000000 auto_classification_generator-1.1.1/auto_classification_generator/common.py
--rw-rw-rw-   0        0        0     1011 2024-03-24 00:10:19.000000 auto_classification_generator-1.1.1/auto_classification_generator/hash.py
--rw-rw-rw-   0        0        0       64 2024-03-23 11:12:41.000000 auto_classification_generator-1.1.1/auto_classification_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-04-04 10:19:40.000000 auto_classification_generator-1.1.1/auto_classification_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:25:47.961151 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/
--rw-rw-rw-   0        0        0      642 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      791 2024-04-04 10:25:00.000000 auto_classification_generator-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 10:25:47.965153 auto_classification_generator-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0      642 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5494 2024-02-20 15:40:54.000000 auto_classification_generator-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:33:14.006857 auto_classification_generator-1.1.2/auto_classification_generator/
+-rw-rw-rw-   0        0        0      408 2024-02-20 15:29:18.000000 auto_classification_generator-1.1.2/auto_classification_generator/__init__.py
+-rw-rw-rw-   0        0        0    14871 2024-04-04 09:56:06.000000 auto_classification_generator-1.1.2/auto_classification_generator/classification_generator.py
+-rw-rw-rw-   0        0        0     2619 2024-04-04 10:31:14.000000 auto_classification_generator-1.1.2/auto_classification_generator/cli.py
+-rw-rw-rw-   0        0        0     2224 2024-03-20 15:06:23.000000 auto_classification_generator-1.1.2/auto_classification_generator/common.py
+-rw-rw-rw-   0        0        0     1011 2024-03-24 00:10:19.000000 auto_classification_generator-1.1.2/auto_classification_generator/hash.py
+-rw-rw-rw-   0        0        0       64 2024-03-23 11:12:41.000000 auto_classification_generator-1.1.2/auto_classification_generator/test_cli.py
+-rw-rw-rw-   0        0        0       21 2024-04-04 10:31:21.000000 auto_classification_generator-1.1.2/auto_classification_generator/version.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/
+-rw-rw-rw-   0        0        0      642 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      791 2024-04-04 10:31:27.000000 auto_classification_generator-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/setup.cfg
```

### Comparing `auto_classification_generator-1.1.1/LICENSE.md` & `auto_classification_generator-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.1/PKG-INFO` & `auto_classification_generator-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.1.1
+Version: 1.1.2
 Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `auto_classification_generator-1.1.1/README.md` & `auto_classification_generator-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.1/auto_classification_generator/classification_generator.py` & `auto_classification_generator-1.1.2/auto_classification_generator/classification_generator.py`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.1/auto_classification_generator/cli.py` & `auto_classification_generator-1.1.2/auto_classification_generator/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     parser.add_argument("-acc","--accession",required=False,choices=['None','Dir','File','All'],default=None)
     parser.add_argument("-o","--output",required=False,nargs='?')
     parser.add_argument("-s","--start-ref",required=False,nargs='?',default=1)
     parser.add_argument("--meta-dir",required=False,action='store_true',default=True)
     parser.add_argument("--skip",required=False,action='store_true',default=False)
     parser.add_argument("--hidden",required=False,action='store_true',default=False)
     parser.add_argument("-fmt","--output-format",required=False,default="xlsx",choices=['xlsx','csv'])
-    parser.add_argument("-fx","--fixity",required=False,const="SHA-1",default=None,choices=['NONE','MD5','SHA-1','SHA-256','SHA-512'],type=str.upper)
+    parser.add_argument("-fx","--fixity",required=False,nargs='?', const="SHA-1",default=None,choices=['NONE','MD5','SHA-1','SHA-256','SHA-512'],type=str.upper)
     parser.add_argument("-v", "--version", action='version',version='%(prog)s {version}'.format(version=__version__))
     args = parser.parse_args()
     return args
 
 def run_cli():
     args = parse_args()
     if isinstance(args.root,str): args.root = args.root.strip("\"").rstrip("\\")
```

### Comparing `auto_classification_generator-1.1.1/auto_classification_generator/common.py` & `auto_classification_generator-1.1.2/auto_classification_generator/common.py`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.1/auto_classification_generator/hash.py` & `auto_classification_generator-1.1.2/auto_classification_generator/hash.py`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.1/auto_classification_generator.egg-info/PKG-INFO` & `auto_classification_generator-1.1.2/auto_classification_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.1.1
+Version: 1.1.2
 Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `auto_classification_generator-1.1.1/auto_classification_generator.egg-info/SOURCES.txt` & `auto_classification_generator-1.1.2/auto_classification_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.1/pyproject.toml` & `auto_classification_generator-1.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2261 7574 6f5f 636c  .name = "auto_cl
 00000070: 6173 7369 6669 6361 7469 6f6e 5f67 656e  assification_gen
 00000080: 6572 6174 6f72 220d 0a76 6572 7369 6f6e  erator"..version
-00000090: 203d 2022 312e 312e 3122 0d0a 6175 7468   = "1.1.1"..auth
+00000090: 203d 2022 312e 312e 3222 0d0a 6175 7468   = "1.1.2"..auth
 000000a0: 6f72 7320 3d20 5b0d 0a20 2020 207b 6e61  ors = [..    {na
 000000b0: 6d65 3d22 4368 7269 7374 6f70 6865 7220  me="Christopher 
 000000c0: 5072 696e 6365 222c 2065 6d61 696c 3d22  Prince", email="
 000000d0: 632e 706a 2e70 7269 6e63 6540 676d 6169  c.pj.prince@gmai
 000000e0: 6c2e 636f 6d22 7d0d 0a20 2020 205d 0d0a  l.com"}..    ]..
 000000f0: 6465 7363 7269 7074 696f 6e20 3d20 2241  description = "A
 00000100: 7574 6f20 436c 6173 7369 6669 6361 7469  uto Classificati
```

