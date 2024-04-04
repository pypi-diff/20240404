# Comparing `tmp/PheTK-0.1.36.tar.gz` & `tmp/PheTK-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PheTK-0.1.36.tar", last modified: Sat Feb 24 23:53:30 2024, max compression
+gzip compressed data, was "PheTK-0.1.37.tar", last modified: Thu Apr  4 21:00:41 2024, max compression
```

## Comparing `PheTK-0.1.36.tar` & `PheTK-0.1.37.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-02-24 23:53:30.185534 PheTK-0.1.36/
--rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-02-24 21:29:54.000000 PheTK-0.1.36/LICENSE
--rw-r--r--   0 trantac  (1207383791) 1360859114    14996 2024-02-24 23:53:30.185291 PheTK-0.1.36/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114    14709 2024-02-24 23:51:24.000000 PheTK-0.1.36/README.md
--rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-02-24 23:53:30.185591 PheTK-0.1.36/setup.cfg
--rw-r--r--   0 trantac  (1207383791) 1360859114      889 2024-02-24 22:01:29.000000 PheTK-0.1.36/setup.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-02-24 23:53:30.145806 PheTK-0.1.36/src/
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-02-24 23:53:30.159391 PheTK-0.1.36/src/PheTK/
--rw-r--r--   0 trantac  (1207383791) 1360859114    16572 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/Cohort.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/Demo.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/PheWAS.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-02-24 23:52:58.000000 PheTK-0.1.36/src/PheTK/Phecode.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/Plot.py
--rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/__init__.py
--rw-r--r--   0 trantac  (1207383791) 1360859114      394 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/_paths.py
--rw-r--r--   0 trantac  (1207383791) 1360859114    10217 2024-02-24 23:26:57.000000 PheTK-0.1.36/src/PheTK/_queries.py
--rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/_utils.py
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-02-24 23:53:30.184002 PheTK-0.1.36/src/PheTK/phecode/
--rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/phecode/phecode12.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/phecode/phecodeX.csv
--rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-02-24 21:29:54.000000 PheTK-0.1.36/src/PheTK/phecode/phecodeX_WHO.csv
-drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-02-24 23:53:30.166118 PheTK-0.1.36/src/PheTK.egg-info/
--rw-r--r--   0 trantac  (1207383791) 1360859114    14996 2024-02-24 23:53:29.000000 PheTK-0.1.36/src/PheTK.egg-info/PKG-INFO
--rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-02-24 23:53:30.000000 PheTK-0.1.36/src/PheTK.egg-info/SOURCES.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-02-24 23:53:29.000000 PheTK-0.1.36/src/PheTK.egg-info/dependency_links.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114      108 2024-02-24 23:53:29.000000 PheTK-0.1.36/src/PheTK.egg-info/requires.txt
--rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-02-24 23:53:29.000000 PheTK-0.1.36/src/PheTK.egg-info/top_level.txt
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:41.016559 PheTK-0.1.37/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35149 2024-03-25 02:28:38.000000 PheTK-0.1.37/LICENSE
+-rw-r--r--   0 trantac  (1207383791) 1360859114      218 2024-04-04 21:00:41.016392 PheTK-0.1.37/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114    15638 2024-04-04 19:53:54.000000 PheTK-0.1.37/README.md
+-rw-r--r--   0 trantac  (1207383791) 1360859114       38 2024-04-04 21:00:41.016617 PheTK-0.1.37/setup.cfg
+-rw-r--r--   0 trantac  (1207383791) 1360859114      693 2024-04-04 21:00:34.000000 PheTK-0.1.37/setup.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:40.977319 PheTK-0.1.37/src/
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:40.982748 PheTK-0.1.37/src/PheTK/
+-rw-r--r--   0 trantac  (1207383791) 1360859114    16572 2024-03-25 02:28:39.000000 PheTK-0.1.37/src/PheTK/Cohort.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     8713 2024-03-25 02:28:39.000000 PheTK-0.1.37/src/PheTK/Demo.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    28199 2024-04-04 16:49:03.000000 PheTK-0.1.37/src/PheTK/PheWAS.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     5120 2024-04-04 16:49:03.000000 PheTK-0.1.37/src/PheTK/Phecode.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    35458 2024-04-04 16:49:03.000000 PheTK-0.1.37/src/PheTK/Plot.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114        0 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/__init__.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114      394 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/_paths.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114    10177 2024-04-04 19:02:44.000000 PheTK-0.1.37/src/PheTK/_queries.py
+-rw-r--r--   0 trantac  (1207383791) 1360859114     4208 2024-03-25 17:23:44.000000 PheTK-0.1.37/src/PheTK/_utils.py
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:41.010802 PheTK-0.1.37/src/PheTK/phecode/
+-rw-r--r--   0 trantac  (1207383791) 1360859114 17510731 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/phecode/phecode12.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114 11150857 2024-03-25 02:28:37.000000 PheTK-0.1.37/src/PheTK/phecode/phecodeX.csv
+-rw-r--r--   0 trantac  (1207383791) 1360859114  1393896 2024-03-25 02:28:39.000000 PheTK-0.1.37/src/PheTK/phecode/phecodeX_WHO.csv
+drwxr-xr-x   0 trantac  (1207383791) 1360859114        0 2024-04-04 21:00:40.984976 PheTK-0.1.37/src/PheTK.egg-info/
+-rw-r--r--   0 trantac  (1207383791) 1360859114      218 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/PKG-INFO
+-rw-r--r--   0 trantac  (1207383791) 1360859114      469 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/SOURCES.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        1 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/dependency_links.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114      115 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/requires.txt
+-rw-r--r--   0 trantac  (1207383791) 1360859114        6 2024-04-04 21:00:40.000000 PheTK-0.1.37/src/PheTK.egg-info/top_level.txt
```

### Comparing `PheTK-0.1.36/LICENSE` & `PheTK-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/PKG-INFO` & `PheTK-0.1.37/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1
-Name: PheTK
-Version: 0.1.36
-Summary: PheTK - Phenotype Toolkit
-Home-page: https://github.com/nhgritctran/PheTK
-Author: Tran, Tam
-Author-email: PheTK@mail.nih.gov
-License: GPL-3.0
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PheTK - The Phenotype Toolkit
 The official repository of PheTK.
 
-Current version: 0.1.36
+Current version: 0.1.37
+
+## Changelog:
+
+___version 0.1.37 (04 Apr 2024):___
+- Removed SNOMED codes from SQL query (_ehr_dx_code_query_) generating _ehr_length_, _dx_code_occurrence_count_, 
+_dx_condition_count_, and _age_at_last_event_ covariates in _.add_covariates()_ method in Cohort module.
+  - This was to make it consistent with ICD event query for phecode mapping, 
+    i.e., only ICD9CM and ICD10CM would be used as vocabulary_id for these queries.
+  - For _All of Us_ users, this change should affect less than 2% of covariate data previously generated 
+  by _.add_covariates()_ method from version 0.1.36 or earlier, and should not significantly change previous analysis results.
 
 ## 1. INSTALLATION
 PheTK can be installed using pip install command in a terminal (Python 3.7 or newer):
 
 ```
 pip install PheTK
 ```
@@ -34,24 +32,21 @@
 
 To check current installed version:
 ```
 pip show PheTK | grep Version
 ```
 
 ## 2. SYSTEM REQUIREMENTS
-As PheTK utilizes multithreading to speed up computational processes, the more CPUs/cores the system has, 
-the faster it would run.
-Memory requirement would vary based on computing platform, user actual workflow and how efficient it is.
-
-In our test, a PheWAS for a cohort of 400,000+ participants and 12 covariates successfully completed on a 
-MacBook Pro M2 Pro 12 CPU cores 32GB RAM in ~81 minutes; 
-PheWAS for the same cohort took ~12 minutes with a cloud instance of 96 CPUs 370GB RAM 
-(memory choice here is mainly for redundancy and for comparison with other tests that we did).
+PheTK was developed for efficient processing of large data while being resource friendly. 
+It was tested on different platforms from laptops to different cloud environments. 
+The lowest test configuration to date was a 4CPU 15GB RAM standard VM on the _All of Us_ researcher workbench 
+for PheWAS of a 200,000+ cohort and 18 covariates. 
 
-In short, the more CPUs the better and RAM should be adequate for user workflow.
+Since every platform and every study is different, users could try different available machine configurations
+to achieve optimal performance and cost-effectiveness.
 
 ## 3. 1-MINUTE PHEWAS DEMO
 
 User can run the quick 1-minute PheWAS demo with the following command in a terminal:
 
 ```
 python3 -m PheTK.Demo
@@ -70,15 +65,18 @@
 
 ### 4.1. PheWAS workflow and PheTK modules
 ![PheWAS workflow and PheTK modules](img/readme/PheTK_flowchart.png)
 Standard PheWAS workflow. Green texts are PheTK module names. 
 Black components are supported while gray ones are not supported by PheTK currently.
 
 ### 4.2. PheTK module descriptions
-This table will be updated as we update PheTK.
+This table will be updated as we update PheTK. 
+
+All modules can be used together or independently, 
+e.g., users who only need to run PheWAS analysis can provide their own cohort and phecode count data as input for PheWAS module. 
 
 | Module  | Class   | Method(s)     | Platform    | Requirements/Notes                                                           |
 |---------|---------|---------------|-------------|------------------------------------------------------------------------------|
 | Cohort  | Cohort  | by_genotype   | _All of Us_ | None                                                                         |
 |         |         |               | Other       | Variant data stored in Hail matrix table                                     |
 |         |         | add_covariate | _All of Us_ | None                                                                         |
 |         |         |               | Other       | Google BigQuery OMOP database                                                |
@@ -97,14 +95,16 @@
 ### 5.1. Cohort module
 Cohort module can be used for generating genetic cohort and add certain covariates to a cohort.
 
 #### 5.1.1. by_genotype
 
 This function takes genetic variant information as input, 
 and generates cohort with matching genotypes as an output csv file.
+As this function uses Hail to extract data from Hail matrix tables, it must be run in a compatible environment,
+e.g., a dataproc cluster on All of Us researcher workbench or UK Biobank RAP.
 
 For example, we generate cohort for _CFTR_ variant chr7-117559590-ATCT-A with 
 heterozygous (0/1 genotype) participants as cases and homozygous reference (0/0 genotype) participants as controls.
 
 #### Jupyter Notebook example for _All of Us_ Researcher Workbench:
 For _All of Us_ data version 7, the default Hail matrix table is the ACAF (common variant) table.
 User can use a different table by providing table location in the mt_path parameter.
@@ -161,15 +161,16 @@
 In this example, we are adding age at last diagnosis event, sex at birth and 10 genetic PCs (provided by _All of Us_).
 These options were set to True (or 10 in case of first_n_pcs).
 
 The covariates shown in this example are currently supported by PheTK. Users should only change parameter value to True 
 for covariates to be used in subsequent PheWAS. All parameters are set to False by default, i.e., user only need to 
 specify parameters of interest as shown in the "short version". 
 
-Users should decide which covariates to use for the study based on their data, and to add or use their own covariate data if necessary.
+It is highly recommended that users should decide which covariates to use for the study based on their data, 
+and it is perfectly fine to add or use their own covariate data if necessary. 
 
 #### Jupyter Notebook example for _All of Us_ Researcher Workbench:
 ```
 # user can skip the import and instantiation steps if running continuously 
 # from previous by_genotype example, i.e., skip directly to add covariates step.
 from PheTK.Cohort import Cohort
```

### Comparing `PheTK-0.1.36/src/PheTK/Cohort.py` & `PheTK-0.1.37/src/PheTK/Cohort.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/Demo.py` & `PheTK-0.1.37/src/PheTK/Demo.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/PheWAS.py` & `PheTK-0.1.37/src/PheTK/PheWAS.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/Phecode.py` & `PheTK-0.1.37/src/PheTK/Phecode.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/Plot.py` & `PheTK-0.1.37/src/PheTK/Plot.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/_queries.py` & `PheTK-0.1.37/src/PheTK/_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,20 +167,20 @@
 
     return query
 
 
 def ehr_dx_code_query(ds, participant_ids):
     """
     This method is exclusively for All of Us platform.
-    In condition occurrence table, diagnosis codes belongs to ICD9CM, ICD10CM and SNOMED, are counted.
+    In condition occurrence table, diagnosis codes belongs to ICD9CM, ICD10CM, are counted.
     In observation table, diagnosis codes belongs to ICD9CM and ICD10CM are counted.
     :param ds: Google BigQuery dataset ID containing OMOP data tables
     :param participant_ids: list of participant IDs to query
     :return: a SQL query that would generate a table contains participant IDs and
-            their ehr length (days), diagnosis code count(ICD & SNOMED), and age at last event
+            their ehr length (days), diagnosis code count(ICD), and age at last event
     """
     query: str = f"""
         SELECT DISTINCT
             df1.person_id,
             (DATETIME_DIFF(MAX(date), MIN(date), DAY) + 1)/365.2425 AS ehr_length,
             COUNT(code) AS dx_code_occurrence_count,
             COUNT(DISTINCT(code)) AS dx_condition_count,
@@ -195,15 +195,15 @@
                 FROM
                     {ds}.condition_occurrence AS co
                 INNER JOIN
                     {ds}.concept AS c
                 ON
                     co.condition_source_value = c.concept_code
                 WHERE
-                    c.vocabulary_id IN ("ICD9CM", "ICD10CM", "SNOMED")
+                    c.vocabulary_id IN ("ICD9CM", "ICD10CM")
                     AND
                     person_id IN {participant_ids}
                 )
             UNION DISTINCT
                 (
                 SELECT DISTINCT
                     co.person_id,
@@ -212,15 +212,15 @@
                 FROM
                     {ds}.condition_occurrence AS co
                 INNER JOIN
                     {ds}.concept AS c
                 ON
                     co.condition_source_concept_id = c.concept_id
                 WHERE
-                    c.vocabulary_id IN ("ICD9CM", "ICD10CM", "SNOMED")
+                    c.vocabulary_id IN ("ICD9CM", "ICD10CM")
                     AND
                     person_id IN {participant_ids}
                 )
             UNION DISTINCT
                 (
                 SELECT DISTINCT
                     o.person_id,
```

### Comparing `PheTK-0.1.36/src/PheTK/_utils.py` & `PheTK-0.1.37/src/PheTK/_utils.py`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/phecode/phecode12.csv` & `PheTK-0.1.37/src/PheTK/phecode/phecode12.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/phecode/phecodeX.csv` & `PheTK-0.1.37/src/PheTK/phecode/phecodeX.csv`

 * *Files identical despite different names*

### Comparing `PheTK-0.1.36/src/PheTK/phecode/phecodeX_WHO.csv` & `PheTK-0.1.37/src/PheTK/phecode/phecodeX_WHO.csv`

 * *Files identical despite different names*

