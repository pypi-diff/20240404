# Comparing `tmp/pySpade-0.1.0.tar.gz` & `tmp/pySpade-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pySpade-0.1.0.tar", last modified: Mon Mar 25 18:16:45 2024, max compression
+gzip compressed data, was "dist/pySpade-0.1.1.tar", last modified: Thu Apr  4 18:03:43 2024, max compression
```

## Comparing `pySpade-0.1.0.tar` & `pySpade-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-03-25 18:16:45.000000 pySpade-0.1.0/
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     1066 2022-09-29 20:16:43.000000 pySpade-0.1.0/LICENSE
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-09 16:49:13.000000 pySpade-0.1.0/MANIFEST.in
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-03-25 18:16:45.000000 pySpade-0.1.0/PKG-INFO
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15114 2024-03-25 18:14:48.000000 pySpade-0.1.0/README.md
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-03-25 18:16:45.000000 pySpade-0.1.0/pySpade/
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-03-21 19:46:56.000000 pySpade-0.1.0/pySpade/DEobs.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     5923 2023-10-30 17:50:45.000000 pySpade-0.1.0/pySpade/DEobsboot.py
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)    12308 2024-03-22 14:30:27.000000 pySpade-0.1.0/pySpade/DErand.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)       36 2024-02-21 21:06:53.000000 pySpade-0.1.0/pySpade/__init__.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     4342 2024-03-21 19:58:28.000000 pySpade-0.1.0/pySpade/__main__.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     2906 2024-01-12 23:46:21.000000 pySpade-0.1.0/pySpade/explevel.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     8198 2024-01-26 01:38:44.000000 pySpade-0.1.0/pySpade/fc.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9465 2024-02-21 19:40:48.000000 pySpade-0.1.0/pySpade/global.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    10147 2024-02-21 21:06:21.000000 pySpade-0.1.0/pySpade/local.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9344 2024-03-21 22:05:07.000000 pySpade-0.1.0/pySpade/manhattan.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    18929 2024-03-25 18:10:56.000000 pySpade-0.1.0/pySpade/parsers.py
--rwxr-----   0 s426305  (426305) Hon_lab   (7001)  2242597 2024-01-26 16:44:04.000000 pySpade-0.1.0/pySpade/plot_annotation.txt
--rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-01-12 23:45:43.000000 pySpade-0.1.0/pySpade/process.py
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    14874 2024-03-21 18:32:24.000000 pySpade-0.1.0/pySpade/utils.py
-drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-03-25 18:16:45.000000 pySpade-0.1.0/pySpade.egg-info/
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-03-25 18:16:43.000000 pySpade-0.1.0/pySpade.egg-info/PKG-INFO
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)      465 2024-03-25 18:16:44.000000 pySpade-0.1.0/pySpade.egg-info/SOURCES.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        1 2024-03-25 18:16:44.000000 pySpade-0.1.0/pySpade.egg-info/dependency_links.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       51 2024-03-25 18:16:44.000000 pySpade-0.1.0/pySpade.egg-info/entry_points.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        8 2024-03-25 18:16:44.000000 pySpade-0.1.0/pySpade.egg-info/top_level.txt
--rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       38 2024-03-25 18:16:45.000000 pySpade-0.1.0/setup.cfg
--rwxr--r--   0 s426305  (426305) Hon_lab   (7001)      987 2023-06-30 19:38:59.000000 pySpade-0.1.0/setup.py
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-04 18:03:43.000000 pySpade-0.1.1/
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)     1066 2022-09-29 20:16:43.000000 pySpade-0.1.1/LICENSE
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       36 2022-12-09 16:49:13.000000 pySpade-0.1.1/MANIFEST.in
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-04-04 18:03:43.000000 pySpade-0.1.1/PKG-INFO
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15114 2024-04-04 17:56:05.000000 pySpade-0.1.1/README.md
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-04 18:03:43.000000 pySpade-0.1.1/pySpade/
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-03-21 19:46:56.000000 pySpade-0.1.1/pySpade/DEobs.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     5923 2023-10-30 17:50:45.000000 pySpade-0.1.1/pySpade/DEobsboot.py
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)    12308 2024-03-22 14:30:27.000000 pySpade-0.1.1/pySpade/DErand.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)       36 2024-03-26 21:08:55.000000 pySpade-0.1.1/pySpade/__init__.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     4342 2024-03-21 19:58:28.000000 pySpade-0.1.1/pySpade/__main__.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     2906 2024-01-12 23:46:21.000000 pySpade-0.1.1/pySpade/explevel.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     8198 2024-01-26 01:38:44.000000 pySpade-0.1.1/pySpade/fc.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9465 2024-02-21 19:40:48.000000 pySpade-0.1.1/pySpade/global.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    10315 2024-04-02 16:51:22.000000 pySpade-0.1.1/pySpade/local.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)     9590 2024-03-26 21:54:47.000000 pySpade-0.1.1/pySpade/manhattan.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    18929 2024-03-25 18:10:56.000000 pySpade-0.1.1/pySpade/parsers.py
+-rwxr-----   0 s426305  (426305) Hon_lab   (7001)  2242597 2024-01-26 16:44:04.000000 pySpade-0.1.1/pySpade/plot_annotation.txt
+-rwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)     8375 2024-01-12 23:45:43.000000 pySpade-0.1.1/pySpade/process.py
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)    14874 2024-03-21 18:32:24.000000 pySpade-0.1.1/pySpade/utils.py
+drwxr-xr-x   0 s426305  (426305) Hon_lab   (7001)        0 2024-04-04 18:03:43.000000 pySpade-0.1.1/pySpade.egg-info/
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)    15621 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/PKG-INFO
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)      465 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/SOURCES.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        1 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/dependency_links.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       51 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/entry_points.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)        8 2024-04-04 18:03:42.000000 pySpade-0.1.1/pySpade.egg-info/top_level.txt
+-rw-r--r--   0 s426305  (426305) Hon_lab   (7001)       38 2024-04-04 18:03:43.000000 pySpade-0.1.1/setup.cfg
+-rwxr--r--   0 s426305  (426305) Hon_lab   (7001)      987 2023-06-30 19:38:59.000000 pySpade-0.1.1/setup.py
```

### Comparing `pySpade-0.1.0/LICENSE` & `pySpade-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/PKG-INFO` & `pySpade-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySpade
-Version: 0.1.0
+Version: 0.1.1
 Summary: Single cell Perturbations - Analysis of Differential gene Expression
 Home-page: https://github.com/Hon-lab/pySpade
 Author: Yihan Wang
 Author-email: Yihan.Wang@UTSouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ## Usage
 ________
 ```
 $pySpade
 usage: pySpade [-h]  ...
 
 pySpade 
-Version: 0.1.0
+Version: 0.1.1
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
     process   process mapping output and reformat for downstream analysis.
@@ -269,15 +269,15 @@
                         specify the csv file directory from the output of global function.
   -cx CUTOFF_EXPRESSION, --cutoff_expression CUTOFF_EXPRESSION
                         specify the cutoff of expressed genes. Default is 0.05 (genes expressed in more than 5 percent of
                         cells)
   -cf CUTOFF_FC, --cutoff_fc CUTOFF_FC
                         specify the cutoff of fold change. Default is 0.2 (fold change is more than 20 percent)
   -cs CUTOFF_SIGNIFICANCE, --cutoff_significance CUTOFF_SIGNIFICANCE
-                        specify the cutoff of Significance_scpre. Default is -5 (Significance score is smaller than -5)
+                        specify the cutoff of Significance_score. Default is -5 (Significance score is smaller than -5)
   -o OUTPUT_FOLDER, --output_folder OUTPUT_FOLDER
                         specify an output folder directory.
 ```
 
 ## Contacts
 _______
 * Yihan Wang `Yihan.Wang@UTSouthwestern.edu`
```

### Comparing `pySpade-0.1.0/README.md` & `pySpade-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ## Usage
 ________
 ```
 $pySpade
 usage: pySpade [-h]  ...
 
 pySpade 
-Version: 0.1.0
+Version: 0.1.1
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
     process   process mapping output and reformat for downstream analysis.
@@ -253,15 +253,15 @@
                         specify the csv file directory from the output of global function.
   -cx CUTOFF_EXPRESSION, --cutoff_expression CUTOFF_EXPRESSION
                         specify the cutoff of expressed genes. Default is 0.05 (genes expressed in more than 5 percent of
                         cells)
   -cf CUTOFF_FC, --cutoff_fc CUTOFF_FC
                         specify the cutoff of fold change. Default is 0.2 (fold change is more than 20 percent)
   -cs CUTOFF_SIGNIFICANCE, --cutoff_significance CUTOFF_SIGNIFICANCE
-                        specify the cutoff of Significance_scpre. Default is -5 (Significance score is smaller than -5)
+                        specify the cutoff of Significance_score. Default is -5 (Significance score is smaller than -5)
   -o OUTPUT_FOLDER, --output_folder OUTPUT_FOLDER
                         specify an output folder directory.
 ```
 
 ## Contacts
 _______
 * Yihan Wang `Yihan.Wang@UTSouthwestern.edu`
```

### Comparing `pySpade-0.1.0/pySpade/DEobs.py` & `pySpade-0.1.1/pySpade/DEobs.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/DEobsboot.py` & `pySpade-0.1.1/pySpade/DEobsboot.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/DErand.py` & `pySpade-0.1.1/pySpade/DErand.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/__main__.py` & `pySpade-0.1.1/pySpade/__main__.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/explevel.py` & `pySpade-0.1.1/pySpade/explevel.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/fc.py` & `pySpade-0.1.1/pySpade/fc.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/global.py` & `pySpade-0.1.1/pySpade/global.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/local.py` & `pySpade-0.1.1/pySpade/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,17 @@
         local_gene_series['fc'] = hits_fc
         local_gene_series['Significance_score'] = down_padj_list
         local_gene_series['fc_by_rand_dist_cpm'] = hits_fc_rand
         local_gene_series['pval-empirical'] = emp_pval
         local_gene_series['cpm_perturb'] = cpm[down_keep_genes_idx]
         local_gene_series['cpm_bg'] = cpm_mean[down_keep_genes_idx]
 
+        local_gene_df = pd.concat([local_gene_df, local_gene_series], ignore_index=True)
+        local_gene_df = local_gene_df.reindex(columns=df_column_list)
+        
         local_gene_series = annot_df[annot_df['gene_names'].isin(gene_seq[up_keep_genes_idx])].set_index('idx').sort_index()
         local_gene_series['region'] = region
         dist_list = []
         for i in local_gene_series['pos']:
             dist = get_distance(region, i)
             dist_list.append(dist)
         local_gene_series['distance'] = dist_list
```

### Comparing `pySpade-0.1.0/pySpade/manhattan.py` & `pySpade-0.1.1/pySpade/manhattan.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,21 @@
         even_idx= np.where(express_subset_df.color_idx == 1)
 
         fc = express_subset_df['fc_by_rand_dist_cpm'].values
 
 
         num_sgrna_cell = express_subset_df['num_cell'].values[0]
         if len(re.split(r'[:-]+', region)) == 3:
-            enh_chrom, left, right = re.split(r'[:-]+', region)
+            _, left, right = re.split(r'[:-]+', region)
+            if (_ in chr_order) == True: 
+                enh_chrom = _
+            else:
+                logger.info('Not valid chromosome coordinates, plot without perturbation region line.')
+                enh_chrom = 'chr1'
+                left = 0
         else:
             logger.info('No chromosome coordinates info, plot without perturbation region line.')
             enh_chrom = 'chr1'
             left = 0
             
         up_cutoff = 1
         down_cutoff = 1
```

### Comparing `pySpade-0.1.0/pySpade/parsers.py` & `pySpade-0.1.1/pySpade/parsers.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/plot_annotation.txt` & `pySpade-0.1.1/pySpade/plot_annotation.txt`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/process.py` & `pySpade-0.1.1/pySpade/process.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade/utils.py` & `pySpade-0.1.1/pySpade/utils.py`

 * *Files identical despite different names*

### Comparing `pySpade-0.1.0/pySpade.egg-info/PKG-INFO` & `pySpade-0.1.1/pySpade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySpade
-Version: 0.1.0
+Version: 0.1.1
 Summary: Single cell Perturbations - Analysis of Differential gene Expression
 Home-page: https://github.com/Hon-lab/pySpade
 Author: Yihan Wang
 Author-email: Yihan.Wang@UTSouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ## Usage
 ________
 ```
 $pySpade
 usage: pySpade [-h]  ...
 
 pySpade 
-Version: 0.1.0
+Version: 0.1.1
 
 optional arguments:
   -h, --help  show this help message and exit
 
 functions:
   
     process   process mapping output and reformat for downstream analysis.
@@ -269,15 +269,15 @@
                         specify the csv file directory from the output of global function.
   -cx CUTOFF_EXPRESSION, --cutoff_expression CUTOFF_EXPRESSION
                         specify the cutoff of expressed genes. Default is 0.05 (genes expressed in more than 5 percent of
                         cells)
   -cf CUTOFF_FC, --cutoff_fc CUTOFF_FC
                         specify the cutoff of fold change. Default is 0.2 (fold change is more than 20 percent)
   -cs CUTOFF_SIGNIFICANCE, --cutoff_significance CUTOFF_SIGNIFICANCE
-                        specify the cutoff of Significance_scpre. Default is -5 (Significance score is smaller than -5)
+                        specify the cutoff of Significance_score. Default is -5 (Significance score is smaller than -5)
   -o OUTPUT_FOLDER, --output_folder OUTPUT_FOLDER
                         specify an output folder directory.
 ```
 
 ## Contacts
 _______
 * Yihan Wang `Yihan.Wang@UTSouthwestern.edu`
```

### Comparing `pySpade-0.1.0/setup.py` & `pySpade-0.1.1/setup.py`

 * *Files identical despite different names*

