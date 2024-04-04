# Comparing `tmp/xnattagger-0.6.6-py2.py3-none-any.whl.zip` & `tmp/xnattagger-0.6.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6831 bytes, number of entries: 10
--rwxrwx---  2.0 unx    16630 b- defN 23-Dec-13 18:46 xnattagger/__init__.py
--rwxrwx---  2.0 unx      220 b- defN 24-Jan-16 16:24 xnattagger/__version__.py
--rwxrwx---  2.0 unx      160 b- defN 23-Dec-08 15:08 xnattagger/config/__init__.py
--rwxrwxr--  2.0 unx     1448 b- defN 23-Dec-08 15:08 xnattagger/config/tagger.yaml
--rwxrwxr-x  2.0 unx     2286 b- defN 24-Jan-16 16:30 xnattagger-0.6.6.data/scripts/xnat_tagger.py
--rwxrwxr--  2.0 unx     1541 b- defN 24-Jan-16 16:30 xnattagger-0.6.6.dist-info/LICENSE
--rwxrwx---  2.0 unx      266 b- defN 24-Jan-16 16:30 xnattagger-0.6.6.dist-info/METADATA
--rwxrwx---  2.0 unx      110 b- defN 24-Jan-16 16:30 xnattagger-0.6.6.dist-info/WHEEL
--rwxrwx---  2.0 unx       11 b- defN 24-Jan-16 16:30 xnattagger-0.6.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      834 b- defN 24-Jan-16 16:30 xnattagger-0.6.6.dist-info/RECORD
-10 files, 23506 bytes uncompressed, 5403 bytes compressed:  77.0%
+Zip file size: 6852 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    16622 b- defN 24-Apr-04 19:05 xnattagger/__init__.py
+-rw-r--r--  2.0 unx      220 b- defN 24-Apr-04 19:06 xnattagger/__version__.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Jun-23 16:36 xnattagger/config/__init__.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-Aug-25 17:45 xnattagger/config/tagger.yaml
+-rwxr-xr-x  2.0 unx     2297 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.data/scripts/xnat_tagger.py
+-rw-r--r--  2.0 unx     1541 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      834 b- defN 24-Apr-04 19:07 xnattagger-0.6.7.dist-info/RECORD
+10 files, 23553 bytes uncompressed, 5424 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: xnattagger/config/__init__.py
 Comment: 
 
 Filename: xnattagger/config/tagger.yaml
 Comment: 
 
-Filename: xnattagger-0.6.6.data/scripts/xnat_tagger.py
+Filename: xnattagger-0.6.7.data/scripts/xnat_tagger.py
 Comment: 
 
-Filename: xnattagger-0.6.6.dist-info/LICENSE
+Filename: xnattagger-0.6.7.dist-info/LICENSE
 Comment: 
 
-Filename: xnattagger-0.6.6.dist-info/METADATA
+Filename: xnattagger-0.6.7.dist-info/METADATA
 Comment: 
 
-Filename: xnattagger-0.6.6.dist-info/WHEEL
+Filename: xnattagger-0.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: xnattagger-0.6.6.dist-info/top_level.txt
+Filename: xnattagger-0.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: xnattagger-0.6.6.dist-info/RECORD
+Filename: xnattagger-0.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xnattagger/__init__.py

```diff
@@ -18,38 +18,38 @@
         self.cache = cache
         self.target = target 
         self.session = session
         self.updates = dict()
 
     def generate_updates(self):
         self.get_scan_listing()
-        if self.target == 'dwi':
+        if 'dwi' in self.target:
             self.updates.update({
                 'dwi': self.dwi(self.scans), # Generate updates for main DWI scan(s)
                 'dwi_PA': self.dwi_PA(self.scans), # Generate updates for PA fieldmap(s)
                 'dwi_AP': self.dwi_AP(self.scans), # Generate updates for AP fieldmap(s)
                 'revpol': self.revpol(self.scans) # Generate updates for revpol scans
             })
-        elif self.target == 't1':
+        if 't1' in self.target:
             self.updates.update({
                 't1w': self.t1w(self.scans),  # Generate updates for T1w scan(s)
                 't1w_move': self.t1w_move(self.scans)  # Generate updates for T1w_MOVE scan(s)
             })
-        elif self.target == 't2':
+        if 't2' in self.target:
             self.updates.update({
                 't2w': self.t2w(self.scans),  # Generate updates for T2w scan(s)
                 't2w_move': self.t2w_move(self.scans)  # Generate updates for T2w_MOVE scan(s)
             })
-        elif self.target == 'bold':
+        if 'bold' in self.target:
             self.updates.update({
                 'bold': self.bold(self.scans),
                 'bold_PA': self.bold_PA(self.scans),
                 'bold_AP': self.bold_AP(self.scans)
                 })
-        elif self.target == 'all':
+        if 'all' in self.target:
             self.updates.update({
                 't1w': self.t1w(self.scans),  # Generate updates for T1w scan(s)
                 't1w_move': self.t1w_move(self.scans),  # Generate updates for T1w_MOVE scan(s)
                 't2w': self.t2w(self.scans),  # Generate updates for T2w scan(s)
                 't2w_move': self.t2w_move(self.scans),  # Generate updates for T2w_MOVE scan(s)
                 'dwi': self.dwi(self.scans), # Generate updates for main DWI scan(s)
                 'dwi_PA': self.dwi_PA(self.scans), # Generate updates for PA fieldmap(s)
```

## xnattagger/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'xnattagger'
 __description__ = 'XNAT Tagger'
 __url__ = 'https://github.com/harvard-nrg/xnattagger'
-__version__ = '0.6.6'
+__version__ = '0.6.7'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## Comparing `xnattagger-0.6.6.data/scripts/xnat_tagger.py` & `xnattagger-0.6.7.data/scripts/xnat_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         help='Output summary of updates')  # Provide help text for output-file argument
     parser.add_argument('--dry-run', action='store_true',
         help='Do not execute updates')  # Provide help text for dry-run argument
     parser.add_argument('--confirm', action='store_true',
         help='Prompt user to confirm every update')  # Provide help text for confirm argument
     parser.add_argument('--config', required=True,
         help='Filters configuration file') 
-    parser.add_argument('--target-modality', choices=['t1', 't2', 'dwi', 'bold', 'all'], required=True, type=str.lower) # Require --target argument
+    parser.add_argument('--target-modality', choices=['t1', 't2', 'dwi', 'bold', 'all'], nargs='+', required=True, type=str.lower) # Require --target argument
     parser.add_argument('--label', required=True,
         help='Label of XNAT MR Session')  # Require label argument
     args = parser.parse_args()
 
     with open(args.config) as fo:
         configs = yaml.load(fo, Loader=yaml.SafeLoader)
```

## Comparing `xnattagger-0.6.6.dist-info/LICENSE` & `xnattagger-0.6.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xnattagger-0.6.6.dist-info/RECORD` & `xnattagger-0.6.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-xnattagger/__init__.py,sha256=o4n1A9qupOj-V-HK9XOqGHZewd3cvVGLqO1HQPOPHxo,16630
-xnattagger/__version__.py,sha256=5EVRdFW_QVH9qxTEB5AmHNiFXMsZ29bWPWmYncn_hno,220
+xnattagger/__init__.py,sha256=3vK4YO5t9dQArgcu6x_QyCmXTeFlwZlPUnq_reQnH7g,16622
+xnattagger/__version__.py,sha256=Al0FbwAwoyM-oGeRRc6d96MdwkD2zJQ4TYF4S9ibFeI,220
 xnattagger/config/__init__.py,sha256=9NvVYPkoanrrNVRCljmYCAjjJZGq5kvF_oatEgVQDQo,160
 xnattagger/config/tagger.yaml,sha256=sWK8PBkv1aLe1G22SvrwBylos0C5UXYg-W3ugGc5Wbg,1448
-xnattagger-0.6.6.data/scripts/xnat_tagger.py,sha256=gELQluptLlYWdvSf-I6L7XxnMs5yfgrZU9eYofdaESE,2286
-xnattagger-0.6.6.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-xnattagger-0.6.6.dist-info/METADATA,sha256=BFMBBKBYHaE3ObA43qHkCwxXOJVzHElrbgTsb_Eqis4,266
-xnattagger-0.6.6.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-xnattagger-0.6.6.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
-xnattagger-0.6.6.dist-info/RECORD,,
+xnattagger-0.6.7.data/scripts/xnat_tagger.py,sha256=D7Yu2D72X_p0IqdFywsmgttT5H0jsHHIYlb-YSwAIWA,2297
+xnattagger-0.6.7.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+xnattagger-0.6.7.dist-info/METADATA,sha256=7C4o1a3iBi-Ya7z8r2QlogXz6DNEbLQAaFvUG_2hoAY,310
+xnattagger-0.6.7.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
+xnattagger-0.6.7.dist-info/top_level.txt,sha256=LdHhj5smL9uEh9HAguIPB8FH7EgYimhI-AODf4fl6tE,11
+xnattagger-0.6.7.dist-info/RECORD,,
```

