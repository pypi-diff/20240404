# Comparing `tmp/Giraffe_View-0.1.0.5.tar.gz` & `tmp/Giraffe_View-0.1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.1.0.5.tar", last modified: Thu Mar 28 00:50:06 2024, max compression
+gzip compressed data, was "Giraffe_View-0.1.0.6.tar", last modified: Thu Apr  4 03:30:55 2024, max compression
```

## Comparing `Giraffe_View-0.1.0.5.tar` & `Giraffe_View-0.1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-03-28 00:50:06.053653 Giraffe_View-0.1.0.5/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-03-28 00:50:06.053653 Giraffe_View-0.1.0.5/Giraffe_View/
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)       57 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/__init__.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3882 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/estimated_read_accuracy.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3698 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/function.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4924 2024-03-28 00:46:28.000000 Giraffe_View-0.1.0.5/Giraffe_View/gc_bias.py
--rwxr--r--   0 xudongliu  (1000) xudongliu  (1000)     6181 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/giraffe
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5674 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5315 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/observed_read_accuracy.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11011 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/plot.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2171 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-03-28 00:50:06.053653 Giraffe_View-0.1.0.5/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-03-28 00:50:05.000000 Giraffe_View-0.1.0.5/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2024-03-28 00:50:05.000000 Giraffe_View-0.1.0.5/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-03-28 00:50:05.000000 Giraffe_View-0.1.0.5/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       88 2024-03-28 00:50:05.000000 Giraffe_View-0.1.0.5/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2024-03-28 00:50:05.000000 Giraffe_View-0.1.0.5/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-03-28 00:50:06.053653 Giraffe_View-0.1.0.5/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11560 2024-03-28 00:43:50.000000 Giraffe_View-0.1.0.5/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2024-03-28 00:50:06.053653 Giraffe_View-0.1.0.5/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)      984 2024-03-28 00:44:25.000000 Giraffe_View-0.1.0.5/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 03:30:55.685450 Giraffe_View-0.1.0.6/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 03:30:55.685450 Giraffe_View-0.1.0.6/Giraffe_View/
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)       57 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/__init__.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3882 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/estimated_read_accuracy.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3698 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/function.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4924 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/gc_bias.py
+-rwxr--r--   0 xudongliu  (1000) xudongliu  (1000)     6181 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/giraffe
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5674 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5539 2024-04-04 03:28:23.000000 Giraffe_View-0.1.0.6/Giraffe_View/observed_read_accuracy.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11011 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/plot.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2171 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 03:30:55.685450 Giraffe_View-0.1.0.6/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-04-04 03:30:55.000000 Giraffe_View-0.1.0.6/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2024-04-04 03:30:55.000000 Giraffe_View-0.1.0.6/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-04-04 03:30:55.000000 Giraffe_View-0.1.0.6/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       98 2024-04-04 03:30:55.000000 Giraffe_View-0.1.0.6/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2024-04-04 03:30:55.000000 Giraffe_View-0.1.0.6/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-04-04 03:30:55.685450 Giraffe_View-0.1.0.6/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11560 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.6/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2024-04-04 03:30:55.685450 Giraffe_View-0.1.0.6/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1002 2024-04-04 03:26:17.000000 Giraffe_View-0.1.0.6/setup.py
```

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.1.0.6/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/function.py` & `Giraffe_View-0.1.0.6/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/gc_bias.py` & `Giraffe_View-0.1.0.6/Giraffe_View/gc_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/giraffe` & `Giraffe_View-0.1.0.6/Giraffe_View/giraffe`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/homopolymer.py` & `Giraffe_View-0.1.0.6/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.1.0.6/Giraffe_View/observed_read_accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
         cmd1 = ["minimap2", "-ax", "map-ont", "-o", "Giraffe_Results/2_Observed_quality/tmp.sam", "--MD", \
         "--secondary=no", "-L", "-t", str(threads), ref, data_path]
 
     elif data_type == "Pacbio":
         cmd1 = ["minimap2", "-ax", "map-pb", "-o", "Giraffe_Results/2_Observed_quality/tmp.sam", "--MD", \
         "--secondary=no", "-L", "-t", str(threads), ref, data_path]
 
+    elif data_type == "ONT_RNA":
+        cmd1 = ["minimap2", "-ax", "splice", "-uf", "-k14", "-o", "Giraffe_Results/2_Observed_quality/tmp.sam", "--MD", \
+        "--secondary=no", "-L", "-t", str(threads), ref, data_path]
+
     cmd2 = ["samtools", "view", "-bS", "-F4", "-@", str(threads), "-o", "Giraffe_Results/2_Observed_quality/tmp.bam", "Giraffe_Results/2_Observed_quality/tmp.sam"]
     cmd3 = ["samtools", "sort", "-@", str(threads), "-o", output, "Giraffe_Results/2_Observed_quality/tmp.bam"]
     cmd4 = ["samtools", "index", "-@", str(threads), output]
     cmd5 = ["rm", "-rf", "Giraffe_Results/2_Observed_quality/tmp.bam", "Giraffe_Results/2_Observed_quality/tmp.sam"]
 
     # Run each command and check the return code
     for i, cmd in enumerate([cmd1, cmd2, cmd3, cmd4, cmd5]):
```

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/plot.py` & `Giraffe_View-0.1.0.6/Giraffe_View/plot.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View/regional_modification.py` & `Giraffe_View-0.1.0.6/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.1.0.6/Giraffe_View.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe-View
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: Giraffe_View is specially designed to provide a comprehensive assessment of the accuracy of long-read sequencing datasets obtained from both the PacBio and Nanopore platforms.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.1.0.5/LICENSE` & `Giraffe_View-0.1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/PKG-INFO` & `Giraffe_View-0.1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe_View
-Version: 0.1.0.5
+Version: 0.1.0.6
 Summary: Giraffe_View is specially designed to provide a comprehensive assessment of the accuracy of long-read sequencing datasets obtained from both the PacBio and Nanopore platforms.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.1.0.5/README.md` & `Giraffe_View-0.1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.5/setup.py` & `Giraffe_View-0.1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.1.0.5",
+  version="0.1.0.6",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="Giraffe_View is specially designed to provide a comprehensive assessment of the accuracy of long-read sequencing datasets obtained from both the PacBio and Nanopore platforms.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
   packages=setuptools.find_packages(),
@@ -21,11 +21,12 @@
   python_requires = '>=3.8, <=3.11',
   install_requires=[
   'pysam >= 0.17.0',
   'plotnine >= 0.12.1',
   'numpy >= 1.7.0',
   'pandas >= 1.5.0',
   'tqdm == 4.64.0',
-  'termcolor >= 2.0.0'
+  'termcolor >= 2.0.0',
+  'Bio >= 1.75'
   ],
   scripts = ["Giraffe_View/giraffe"]
 )
```

