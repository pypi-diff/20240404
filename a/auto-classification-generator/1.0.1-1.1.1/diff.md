# Comparing `tmp/auto_classification_generator-1.0.1.tar.gz` & `tmp/auto_classification_generator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_classification_generator-1.0.1.tar", last modified: Tue Feb 20 15:49:08 2024, max compression
+gzip compressed data, was "auto_classification_generator-1.1.1.tar", last modified: Thu Apr  4 10:25:47 2024, max compression
```

## Comparing `auto_classification_generator-1.0.1.tar` & `auto_classification_generator-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 15:49:08.122520 auto_classification_generator-1.0.1/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      642 2024-02-20 15:49:08.122520 auto_classification_generator-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5494 2024-02-20 15:40:54.000000 auto_classification_generator-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-20 15:49:08.062761 auto_classification_generator-1.0.1/auto_classification_generator/
--rw-rw-rw-   0        0        0      408 2024-02-20 15:29:18.000000 auto_classification_generator-1.0.1/auto_classification_generator/__init__.py
--rw-rw-rw-   0        0        0    14179 2024-02-19 00:07:14.000000 auto_classification_generator-1.0.1/auto_classification_generator/classification_generator.py
--rw-rw-rw-   0        0        0     2349 2024-02-20 15:31:22.000000 auto_classification_generator-1.0.1/auto_classification_generator/cli.py
--rw-rw-rw-   0        0        0     2018 2024-02-18 17:21:49.000000 auto_classification_generator-1.0.1/auto_classification_generator/common.py
--rw-rw-rw-   0        0        0       66 2024-02-20 15:33:26.000000 auto_classification_generator-1.0.1/auto_classification_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-02-20 15:29:02.000000 auto_classification_generator-1.0.1/auto_classification_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-02-20 15:49:08.122520 auto_classification_generator-1.0.1/auto_classification_generator.egg-info/
--rw-rw-rw-   0        0        0      642 2024-02-20 15:49:07.000000 auto_classification_generator-1.0.1/auto_classification_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-02-20 15:49:07.000000 auto_classification_generator-1.0.1/auto_classification_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 15:49:07.000000 auto_classification_generator-1.0.1/auto_classification_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-02-20 15:49:07.000000 auto_classification_generator-1.0.1/auto_classification_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-02-20 15:49:07.000000 auto_classification_generator-1.0.1/auto_classification_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-02-20 15:49:07.000000 auto_classification_generator-1.0.1/auto_classification_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      791 2024-02-20 15:35:07.000000 auto_classification_generator-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-20 15:49:08.122520 auto_classification_generator-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:47.965153 auto_classification_generator-1.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      642 2024-04-04 10:25:47.963152 auto_classification_generator-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5494 2024-02-20 15:40:54.000000 auto_classification_generator-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:47.924712 auto_classification_generator-1.1.1/auto_classification_generator/
+-rw-rw-rw-   0        0        0      408 2024-02-20 15:29:18.000000 auto_classification_generator-1.1.1/auto_classification_generator/__init__.py
+-rw-rw-rw-   0        0        0    14871 2024-04-04 09:56:06.000000 auto_classification_generator-1.1.1/auto_classification_generator/classification_generator.py
+-rw-rw-rw-   0        0        0     2608 2024-04-04 10:19:07.000000 auto_classification_generator-1.1.1/auto_classification_generator/cli.py
+-rw-rw-rw-   0        0        0     2224 2024-03-20 15:06:23.000000 auto_classification_generator-1.1.1/auto_classification_generator/common.py
+-rw-rw-rw-   0        0        0     1011 2024-03-24 00:10:19.000000 auto_classification_generator-1.1.1/auto_classification_generator/hash.py
+-rw-rw-rw-   0        0        0       64 2024-03-23 11:12:41.000000 auto_classification_generator-1.1.1/auto_classification_generator/test_cli.py
+-rw-rw-rw-   0        0        0       21 2024-04-04 10:19:40.000000 auto_classification_generator-1.1.1/auto_classification_generator/version.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:47.961151 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/
+-rw-rw-rw-   0        0        0      642 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-04-04 10:25:47.000000 auto_classification_generator-1.1.1/auto_classification_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      791 2024-04-04 10:25:00.000000 auto_classification_generator-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:25:47.965153 auto_classification_generator-1.1.1/setup.cfg
```

### Comparing `auto_classification_generator-1.0.1/LICENSE.md` & `auto_classification_generator-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.0.1/PKG-INFO` & `auto_classification_generator-1.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.0.1
-Summary: Auto Classificaiton Generator Tool for Archivists
+Version: 1.1.1
+Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Archiving
```

### Comparing `auto_classification_generator-1.0.1/README.md` & `auto_classification_generator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.0.1/auto_classification_generator/classification_generator.py` & `auto_classification_generator-1.1.1/auto_classification_generator/classification_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,42 +6,46 @@
 It is compatible with Windows, MacOS and Linux Operating Systems.
 
 author: Christopher Prince
 license: Apache License 2.0"
 """
 
 from auto_classification_generator.common import *
-import os
+from auto_classification_generator.hash import *
+import os, stat
 import pandas as pd
 from datetime import datetime
 import time
-import argparse
 
 class ClassificationGenerator():
     def __init__(self,
-                 root,
-                 output_path=os.getcwd(),
-                 prefix=None,
-                 accprefix=None,
-                 start_ref=1,
-                 empty_flag=False,
-                 skip_flag=False,
-                 accession_flag=None,
-                 meta_dir_flag=True,
-                 output_format="xlsx"):
+                 root: str,
+                 output_path: str = os.getcwd(),
+                 prefix: str = None,
+                 accprefix: str = None,
+                 start_ref: int = 1,
+                 fixity: str = None,
+                 empty_flag: bool = False,
+                 skip_flag: bool = False,
+                 accession_flag: bool = False,
+                 meta_dir_flag: bool = True,
+                 hidden_flag: bool = False,
+                 output_format: str ="xlsx"):
         
         self.root = os.path.abspath(root)
         self.root_level = self.root.count(os.sep)
         self.root_path = os.path.dirname(self.root)         
         self.output_path = output_path
         self.output_format = output_format
         self.empty_flag = empty_flag
         self.skip_flag = skip_flag
+        self.hidden_flag = hidden_flag
         self.prefix = prefix
-        self.start_ref = int(start_ref)
+        self.start_ref = start_ref
+        self.fixity = fixity
         self.reference_list = []
         self.record_list = []
         self.accession_flag = accession_flag
         self.accession_list = []
         self.accession_count = start_ref
         if accprefix: self.accession_prefix = accprefix
         else: self.accession_prefix = prefix
@@ -83,78 +87,86 @@
         2. '.opex' files
         3. Folders titled 'meta'
         4. Script file
         5. Output file
         
         Look to make dynamic and customisable...
         """ 
-        list_directories = sorted([f for f in os.listdir(directory) \
-            if not f.startswith('.') \
-            and not f.endswith('.opex') \
-            and f != 'meta'\
-            and f != os.path.basename(__file__) \
-            and not f.endswith(f'_AutoClass.{self.output_format}') and not f.endswith(f'_autoclass.{self.output_format}')\
-            and not f.endswith('_EmptyDirectoriesRemoved.txt')],key=str.casefold)
+        if not self.hidden_flag:
+            list_directories = sorted([f for f in os.listdir(directory) \
+                if not f.startswith('.') \
+                and not bool(os.stat(os.path.join(directory,f)).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN) \
+                and not f.endswith('.opex') \
+                and f != 'meta'\
+                and f != os.path.basename(__file__)],key=str.casefold)
+        else: list_directories = sorted([f for f in os.listdir(directory) \
+                if not f.endswith('.opex') \
+                and f != 'meta' \
+                and f != os.path.basename(__file__)],key=str.casefold)
         return list_directories
     
-    def parse_directory_dict(self,file_path,level,ref):
+    def parse_directory_dict(self,file_path: str, level: str, ref: int):
         """
-        Parse's directory / file data into a dict which is then appened to a list
+        Parse's directory / file data into a dict which is then appended to a list
         """
         full_path = os.path.abspath(file_path)
         file_stats = os.stat(file_path)                               
         if self.accession_flag:                                                   
             acc_ref = self.accession_running_number(file_path)
             self.accession_list.append(acc_ref)
         if os.path.isdir(file_path): file_type = "Dir"
         else: file_type = "File"
         class_dict = {'RelativeName': str(file_path).replace(self.root_path,""),
                         'FullName':str(full_path),
                         'Basename': os.path.splitext(os.path.basename(file_path))[0],
                         'Extension': os.path.splitext(file_path)[1],
-                        #'Parent':str(Path(full_path).parent),
-                        'Parent': os.path.abspath(os.path.join(full_path, os.pardir)), # Alt Parent 
+                        'Parent': os.path.abspath(os.path.join(full_path, os.pardir)),
                         'Attribute':file_type,
                         'Size':file_stats.st_size,
                         'CreateDate':datetime.fromtimestamp(file_stats.st_ctime),
                         'ModifiedDate': datetime.fromtimestamp(file_stats.st_mtime),
                         'AccessDate':datetime.fromtimestamp(file_stats.st_atime),
                         'Level':level,
                         'Ref_Section':ref}
+        if self.fixity and not os.path.isdir(file_path):
+            hash = HashGenerator(self.fixity).hash_generator(win_256_check(file_path))
+            class_dict.update({"Algorithm":self.fixity,"Hash":hash})
         self.record_list.append(class_dict)
         return class_dict
         
-    def list_directories(self,directory,ref=1):
+    def list_directories(self,directory: str, ref: int = 1):
         """
-        Generates a list of directories. Also calculate's level and a running reference number.
+        Generates a list of directories. Also calculate's level and the reference number utilised in lookups.
         """
         ref = int(ref)
         try:
             list_directory = self.filter_directories(directory)
-            level = directory.count(os.sep) - self.root_level + 1 # Counts the number of Seperators in the current file and subtracts from rootlevels (giving current level).
+            if directory.startswith(u'\\\\?\\'): level = directory.replace(u'\\\\?\\',"").count(os.sep) - self.root_level + 1
+            else: level = directory.count(os.sep) - self.root_level + 1
             for file in list_directory:
-                file_path = os.path.join(directory,file)        
-                # Processing and appending the metadata to lists.
+                file_path = os.path.join(directory,file)
+                file_path_256 = win_256_check(file_path)
                 self.parse_directory_dict(file_path,level,ref)
                 ref = int(ref) + int(1)
-                if os.path.isdir(file_path): self.list_directories(file_path,ref=1)
+                if os.path.isdir(file_path): self.list_directories(file_path_256,ref=1)
         except Exception as e:
             print(e)
-            print("Error Occured for directory/file: {}".format(list_directory))
+            print("Error occured for directory/file: {}".format(list_directory))
+            raise SystemExit()
             pass
         
     def init_dataframe(self):
         """
         The directories are listed which are listed and form dicts from above two functions.
         This looks up and pulls through the Parent row's data to the Child Row.
         The dataframe is merged on itself, Parent is merged 'left' on FullName to pull through the Parent's data (lookup is based on File Path's), and unnecessary data is dropped.
         Any errors are turned to 0 and the result are based to the reference loop init. 
         """
         self.parse_directory_dict(file_path=self.root,level=0,ref=0)
-        self.list_directories(self.root,self.start_ref) # Lists Directories..
+        self.list_directories(self.root,self.start_ref)
         df = pd.DataFrame(self.record_list)                                                                            
         df = df.merge(df[['FullName','Ref_Section']],how='left',left_on='Parent',right_on='FullName')              
         df = df.drop(['FullName_y'], axis=1)                                                                            
         df = df.rename(columns={'Ref_Section_x':'Ref_Section','Ref_Section_y':'Parent_Ref','FullName_x':'FullName'})    # Rename occurs to realign columns
         df['Parent_Ref'] = df['Parent_Ref'].fillna(0)                                                                   # Any Blank rows in Parent Ref set to 0                                                      
         df = df.astype({'Parent_Ref': int})                                                                             # Parent Ref is set as Type int
         df.index.name = "Index"
@@ -162,26 +174,24 @@
         self.df = df
         if self.skip_flag: pass
         else: self.init_reference_loop()
         return self.df
     
     def init_reference_loop(self):
         """
-        Intiation of the Reference loop. Sets some of the prevariables necessary for the loop.
+        Inits the Reference loop. Sets some of the pre-variables necessary for the loop.
         """
         c = 0                       
         tot = len(self.list_loop)
-        #print(tot)
         for REF,PARENT,LEVEL in self.list_loop:
-            #print(REF,PARENT,LEVEL)
             c += 1
-            print(f"Generating Auto Classification for: {c} / {tot}",end="\r") # For a simple progress bar....
+            print(f"Generating Auto Classification for: {c} / {tot}",end="\r")
             TRACK = 1  
-            self.reference_loop(REF,PARENT,TRACK,LEVEL)  #Start's Reference Loop - Recursive Function, so operates on it's own!
-        print()
+            self.reference_loop(REF,PARENT,TRACK,LEVEL)
+
         self.df['Archive_Reference'] = self.reference_list
         if self.accession_flag:
             self.df['Accession_Reference'] = self.accession_list
         return self.df
     
     def reference_loop(self, REF, PARENT, TRACK, LEVEL, NEWREF=None):
         """
@@ -204,15 +214,14 @@
         6) If the index does matches, then top level has not yet been reached. In this case we also account for the PARENT's Reference, to avoid an error at the 2nd to top layer.
         7) PARENTREF is looked up, by Indexing the Dataframe. Then if PARENTREF is 0, IE we're on the 2nd top layer. We check the TRACK.
         8) If TRACK is 1, IE the first iteration on the 2nd layer, NEWREF is just REF.
         9) If TRACK isn't 1, IE subsquent iteration's on the 2nd layer, NEWREF is just itself.
         10) If PARENTREF isn't 0, then we concatenate the PARENTREF with either REF or NEWREF.
         11) If TRACK is 1, NEWREF is PARENTREF + REF.
         12) If TRACK isn't 1, NEWREF is PARENTREF + NEWREF.
-
         13) At the end of the process the PARENT of the current folder is looked up and SUBPARENT replace's the PARENT variable. TRACK is also advanced.
         14) Then function is then called on recusrively. In this way the loop will work through until it reaches the top. 
         15) this is only called upon if the index does not fail. If it does fail, then the top-level is reached and the loop escaped.
         16) As this is acting within the Loop from the init stage, this will operate on all files within a list.
         """
         try:
             idx = self.df.index[self.df['FullName'] == PARENT]
@@ -240,23 +249,30 @@
 
         except Exception as e:
             print('Passed?')
             print(e)
             pass 
 
     def accession_running_number(self,file_path):
+        """
+        Generates a Running Number / Accession Code, can be set to 3 different "modes", counting Files, Directories or Both
+        """
+
         if self.accession_flag == "File":
             if os.path.isdir(file_path): accession_ref = self.accession_prefix + "-Dir"
             else: accession_ref = accession_ref = self.accession_prefix + "-" + str(self.accession_count); self.accession_count += 1
         elif self.accession_flag == "Dir":
             if os.path.isdir(file_path): accession_ref = self.accession_prefix + "-" + str(self.accession_count); self.accession_count += 1
             else: accession_ref = accession_ref = self.accession_prefix + "-File"
         elif self.accession_flag == "All":
             accession_ref = self.accession_prefix + "-" + str(self.accession_count); self.accession_count += 1
         return accession_ref
             
     def main(self):
+        """
+        Runs Program :)
+        """
         if self.empty_flag: self.remove_empty_directories()
         self.init_dataframe()
         output_file = define_output_file(self.output_path,self.root,meta_dir_flag=self.meta_dir_flag,output_format=self.output_format)
         if self.output_format == "xlsx": export_xl(df=self.df,output_filename=output_file)
         elif self.output_format == "csv": export_csv(df=self.df,output_filename=output_file)
```

### Comparing `auto_classification_generator-1.0.1/auto_classification_generator/cli.py` & `auto_classification_generator-1.1.1/auto_classification_generator/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,38 +8,39 @@
     parser.add_argument('root',nargs='?', default=os.getcwd())
     parser.add_argument("-p","--prefix",required=False, nargs='?')
     parser.add_argument("-accp", "--acc-prefix",required=False, nargs='?')
     parser.add_argument("-rm","--empty",required=False,action='store_true')
     parser.add_argument("-acc","--accession",required=False,choices=['None','Dir','File','All'],default=None)
     parser.add_argument("-o","--output",required=False,nargs='?')
     parser.add_argument("-s","--start-ref",required=False,nargs='?',default=1)
-    parser.add_argument("-m","--meta-dir",required=False,action='store_true',default=True)
+    parser.add_argument("--meta-dir",required=False,action='store_true',default=True)
     parser.add_argument("--skip",required=False,action='store_true',default=False)
+    parser.add_argument("--hidden",required=False,action='store_true',default=False)
     parser.add_argument("-fmt","--output-format",required=False,default="xlsx",choices=['xlsx','csv'])
+    parser.add_argument("-fx","--fixity",required=False,const="SHA-1",default=None,choices=['NONE','MD5','SHA-1','SHA-256','SHA-512'],type=str.upper)
     parser.add_argument("-v", "--version", action='version',version='%(prog)s {version}'.format(version=__version__))
     args = parser.parse_args()
     return args
 
 def run_cli():
     args = parse_args()
     if isinstance(args.root,str): args.root = args.root.strip("\"").rstrip("\\")
     if not args.output:
         args.output = os.path.abspath(args.root)
         print(f'No output path selected, defaulting to root Directory: {args.output}')
     else:
         args.output = os.path.abspath(args.output)
         print(f'Output path set to: {args.output}')
-    if args.version:
-        print(__version__)
-        raise SystemExit()
     
     ClassificationGenerator(args.root,
-                            output_path=args.output,
+                            output_path = args.output,
                             prefix=args.prefix,
                             accprefix=args.acc_prefix,
+                            fixity=args.fixity,
                             empty_flag=args.empty,
                             accession_flag=args.accession,
+                            hidden_flag=args.hidden,
                             start_ref=args.start_ref,
                             meta_dir_flag=args.meta_dir,
                             skip_flag=args.skip,
                             output_format=args.output_format).main()
     print('Complete!')
```

### Comparing `auto_classification_generator-1.0.1/auto_classification_generator/common.py` & `auto_classification_generator-1.1.1/auto_classification_generator/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 author: Christopher Prince
 license: Apache License 2.0"
 """
 
 import os
 import time
 import pandas as pd
+import sys
 
 def path_check(path):
     if os.path.exists(path):
         pass
     else: os.makedirs(path)
 
 def define_output_file(output_path,output_name,meta_dir_flag=True,output_suffix="_AutoClass",output_format="xlsx"):
@@ -54,7 +55,13 @@
     except Exception as e:
         print(e)
         print('Waiting 10 Seconds to try again...')
         time.sleep(10)
         export_xl(df,output_filename)
     finally:
         print(f"Saved to: {output_filename}")
+
+def win_256_check(path: str):
+    if len(path) > 255 and sys.platform == "win32":
+        if path.startswith(u'\\\\?\\'): path = path
+        else: path = u"\\\\?\\" + path
+    return path
```

### Comparing `auto_classification_generator-1.0.1/auto_classification_generator.egg-info/PKG-INFO` & `auto_classification_generator-1.1.1/auto_classification_generator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.0.1
-Summary: Auto Classificaiton Generator Tool for Archivists
+Version: 1.1.1
+Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Archiving
```

### Comparing `auto_classification_generator-1.0.1/auto_classification_generator.egg-info/SOURCES.txt` & `auto_classification_generator-1.1.1/auto_classification_generator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.md
 README.md
 pyproject.toml
 auto_classification_generator/__init__.py
 auto_classification_generator/classification_generator.py
 auto_classification_generator/cli.py
 auto_classification_generator/common.py
+auto_classification_generator/hash.py
 auto_classification_generator/test_cli.py
 auto_classification_generator/version.py
 auto_classification_generator.egg-info/PKG-INFO
 auto_classification_generator.egg-info/SOURCES.txt
 auto_classification_generator.egg-info/dependency_links.txt
 auto_classification_generator.egg-info/entry_points.txt
 auto_classification_generator.egg-info/requires.txt
```

### Comparing `auto_classification_generator-1.0.1/pyproject.toml` & `auto_classification_generator-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2261 7574 6f5f 636c  .name = "auto_cl
 00000070: 6173 7369 6669 6361 7469 6f6e 5f67 656e  assification_gen
 00000080: 6572 6174 6f72 220d 0a76 6572 7369 6f6e  erator"..version
-00000090: 203d 2022 312e 302e 3122 0d0a 6175 7468   = "1.0.1"..auth
+00000090: 203d 2022 312e 312e 3122 0d0a 6175 7468   = "1.1.1"..auth
 000000a0: 6f72 7320 3d20 5b0d 0a20 2020 207b 6e61  ors = [..    {na
 000000b0: 6d65 3d22 4368 7269 7374 6f70 6865 7220  me="Christopher 
 000000c0: 5072 696e 6365 222c 2065 6d61 696c 3d22  Prince", email="
 000000d0: 632e 706a 2e70 7269 6e63 6540 676d 6169  c.pj.prince@gmai
 000000e0: 6c2e 636f 6d22 7d0d 0a20 2020 205d 0d0a  l.com"}..    ]..
 000000f0: 6465 7363 7269 7074 696f 6e20 3d20 2241  description = "A
-00000100: 7574 6f20 436c 6173 7369 6669 6361 6974  uto Classificait
+00000100: 7574 6f20 436c 6173 7369 6669 6361 7469  uto Classificati
 00000110: 6f6e 2047 656e 6572 6174 6f72 2054 6f6f  on Generator Too
 00000120: 6c20 666f 7220 4172 6368 6976 6973 7473  l for Archivists
 00000130: 220d 0a63 6c61 7373 6966 6965 7273 203d  "..classifiers =
 00000140: 205b 0d0a 2020 2020 2250 726f 6772 616d   [..    "Program
 00000150: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 00000160: 2050 7974 686f 6e20 3a3a 2033 222c 0d0a   Python :: 3",..
 00000170: 2020 2020 224c 6963 656e 7365 203a 3a20      "License ::
```

