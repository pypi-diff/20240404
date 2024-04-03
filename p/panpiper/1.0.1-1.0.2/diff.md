# Comparing `tmp/panpiper-1.0.1.tar.gz` & `tmp/panpiper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panpiper-1.0.1.tar", last modified: Wed Apr  3 01:45:45 2024, max compression
+gzip compressed data, was "panpiper-1.0.2.tar", last modified: Wed Apr  3 23:22:11 2024, max compression
```

## Comparing `panpiper-1.0.1.tar` & `panpiper-1.0.2.tar`

### file list

```diff
@@ -1,81 +1,56 @@
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.673124 panpiper-1.0.1/
--rw-r--r--   0 reneeoles   (501) staff       (20)     1509 2023-01-23 16:00:15.000000 panpiper-1.0.1/LICENSE
--rw-r--r--   0 reneeoles   (501) staff       (20)       37 2023-01-21 00:39:08.000000 panpiper-1.0.1/MANIFEST.in
--rw-r--r--   0 reneeoles   (501) staff       (20)     9698 2024-04-03 01:45:45.672949 panpiper-1.0.1/PKG-INFO
--rw-r--r--   0 reneeoles   (501) staff       (20)     8735 2024-04-03 00:21:18.000000 panpiper-1.0.1/README.md
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.636859 panpiper-1.0.1/panpiper/
--rw-r--r--   0 reneeoles   (501) staff       (20)      415 2023-01-23 16:01:59.000000 panpiper-1.0.1/panpiper/__init__.py
--rwxr-xr-x   0 reneeoles   (501) staff       (20)     7451 2024-04-03 01:12:25.000000 panpiper-1.0.1/panpiper/main.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     5638 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/test.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.639690 panpiper-1.0.1/panpiper/tests/
--rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/__init__.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.640218 panpiper-1.0.1/panpiper/tests/test_data/
--rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_data/__init__.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     3918 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/tests/test_main.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.641922 panpiper-1.0.1/panpiper/tests/test_scripts/
--rw-r--r--   0 reneeoles   (501) staff       (20)      361 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_scripts/__init__.py
--rw-r--r--   0 reneeoles   (501) staff       (20)    14686 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_scripts/filter_isolates.py
--rwxr-xr-x   0 reneeoles   (501) staff       (20)     1493 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_scripts/test_concat_amrfinder.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.644948 panpiper-1.0.1/panpiper/workflow/
--rw-r--r--   0 reneeoles   (501) staff       (20)     1706 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/workflow/assembly.smk
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.654017 panpiper-1.0.1/panpiper/workflow/envs/
--rw-r--r--   0 reneeoles   (501) staff       (20)      149 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/amrfinder.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       93 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/bakta.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       65 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/bbmap.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      106 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/bwa.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      102 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/checkm.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      330 2024-04-03 01:37:37.000000 panpiper-1.0.1/panpiper/workflow/envs/checkm2.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      110 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/eggnog.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      114 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/fastani.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      100 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/fasttree.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       97 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/iqtree.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       96 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/kraken.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       89 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/mash.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       97 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/panaroo.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       68 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/poppunk.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      172 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/prokka.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       95 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/pyseer.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      201 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/r.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)       68 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/raxml.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      112 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/shovill.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      102 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/unitig.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)      104 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/virsorter.yml
--rw-r--r--   0 reneeoles   (501) staff       (20)    13100 2024-04-03 01:09:15.000000 panpiper-1.0.1/panpiper/workflow/pangenome.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     7287 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/workflow/pyseer.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     5918 2024-04-03 01:19:50.000000 panpiper-1.0.1/panpiper/workflow/quality.smk
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.672102 panpiper-1.0.1/panpiper/workflow/scripts/
--rw-r--r--   0 reneeoles   (501) staff       (20)     1813 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/AMR_heatmap.R
--rw-r--r--   0 reneeoles   (501) staff       (20)     4329 2024-01-24 18:23:49.000000 panpiper-1.0.1/panpiper/workflow/scripts/checkm-log.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     1696 2024-01-24 00:59:58.000000 panpiper-1.0.1/panpiper/workflow/scripts/checkm_bin-stats.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     1559 2024-01-24 01:00:41.000000 panpiper-1.0.1/panpiper/workflow/scripts/checkm_cat.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     1711 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/concat_amrfinder.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     1603 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/count_patterns.py
--rwxr-xr-x   0 reneeoles   (501) staff       (20)      201 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/create_list.sh
--rw-r--r--   0 reneeoles   (501) staff       (20)      946 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_genes.R
--rw-r--r--   0 reneeoles   (501) staff       (20)     6219 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_isolates.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     1033 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_kmers.R
--rw-r--r--   0 reneeoles   (501) staff       (20)      962 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_kmers_enet.R
--rw-r--r--   0 reneeoles   (501) staff       (20)     1948 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/kraken_reformat.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     2039 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/long_to_wide.py
--rw-r--r--   0 reneeoles   (501) staff       (20)      749 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/mash.smk
--rwxr-xr-x   0 reneeoles   (501) staff       (20)      561 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/move_files.sh
--rw-r--r--   0 reneeoles   (501) staff       (20)     1098 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/nc_aa_translate.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     2513 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/phylogeny_distance.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     5633 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/phylogroup_cluster.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     4055 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/quality_report.Rmd
--rw-r--r--   0 reneeoles   (501) staff       (20)  8290584 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/quality_report.html
--rwxr-xr-x   0 reneeoles   (501) staff       (20)      190 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/setup.sh
--rw-r--r--   0 reneeoles   (501) staff       (20)     3628 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/summarise_annotations.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     3338 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/summarise_annotations_enet.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     4461 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/wrangle_output.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     3278 2024-04-03 01:11:13.000000 panpiper-1.0.1/panpiper/workflow.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.672453 panpiper-1.0.1/panpiper.egg-info/
--rw-r--r--   0 reneeoles   (501) staff       (20)     9698 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/PKG-INFO
--rw-r--r--   0 reneeoles   (501) staff       (20)     2467 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/SOURCES.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        1 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/dependency_links.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)       47 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/entry_points.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-03-30 16:55:22.000000 panpiper-1.0.1/panpiper.egg-info/not-zip-safe
--rw-r--r--   0 reneeoles   (501) staff       (20)      187 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/requires.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        9 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/top_level.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)       38 2024-04-03 01:45:45.673500 panpiper-1.0.1/setup.cfg
--rw-r--r--   0 reneeoles   (501) staff       (20)     2026 2024-04-03 01:41:52.000000 panpiper-1.0.1/setup.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.558195 panpiper-1.0.2/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1509 2024-01-24 00:50:52.000000 panpiper-1.0.2/LICENSE
+-rw-r--r--   0 reneeoles   (501) staff       (20)       37 2024-01-24 00:50:52.000000 panpiper-1.0.2/MANIFEST.in
+-rw-r--r--   0 reneeoles   (501) staff       (20)     9402 2024-04-03 23:22:11.557737 panpiper-1.0.2/PKG-INFO
+-rw-r--r--   0 reneeoles   (501) staff       (20)     8652 2024-01-24 00:50:52.000000 panpiper-1.0.2/README.md
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.513013 panpiper-1.0.2/panpiper/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      415 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/__init__.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     7555 2024-04-03 04:00:54.000000 panpiper-1.0.2/panpiper/main.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     5638 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/test.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.516247 panpiper-1.0.2/panpiper/tests/
+-rw-r--r--   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/tests/__init__.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.516727 panpiper-1.0.2/panpiper/tests/test_data/
+-rw-r--r--   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/tests/test_data/__init__.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3918 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/tests/test_main.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.517875 panpiper-1.0.2/panpiper/tests/test_scripts/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      361 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/tests/test_scripts/__init__.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)    14686 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/tests/test_scripts/filter_isolates.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1493 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/tests/test_scripts/test_concat_amrfinder.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.519577 panpiper-1.0.2/panpiper/workflow/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1706 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/assembly.smk
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.556843 panpiper-1.0.2/panpiper/workflow/envs/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      149 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/amrfinder.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       93 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/bakta.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       65 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/bbmap.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      106 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/bwa.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      102 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/checkm.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      312 2024-04-03 23:14:25.000000 panpiper-1.0.2/panpiper/workflow/envs/checkm2.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      110 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/eggnog.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      114 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/fastani.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      100 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/fasttree.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       97 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/iqtree.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       96 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/kraken.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       89 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/mash.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       97 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/panaroo.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       68 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/poppunk.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      172 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/prokka.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       95 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/pyseer.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      201 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/r.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       68 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/raxml.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      112 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/shovill.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      102 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/unitig.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      104 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/envs/virsorter.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)    13100 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/pangenome.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     7287 2024-04-03 01:42:00.000000 panpiper-1.0.2/panpiper/workflow/pyseer.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     5981 2024-04-03 03:56:42.000000 panpiper-1.0.2/panpiper/workflow/quality.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3278 2024-04-03 03:56:27.000000 panpiper-1.0.2/panpiper/workflow.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 23:22:11.557285 panpiper-1.0.2/panpiper.egg-info/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     9402 2024-04-03 23:22:11.000000 panpiper-1.0.2/panpiper.egg-info/PKG-INFO
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1407 2024-04-03 23:22:11.000000 panpiper-1.0.2/panpiper.egg-info/SOURCES.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        1 2024-04-03 23:22:11.000000 panpiper-1.0.2/panpiper.egg-info/dependency_links.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)       47 2024-04-03 23:22:11.000000 panpiper-1.0.2/panpiper.egg-info/entry_points.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        1 2024-01-24 18:18:25.000000 panpiper-1.0.2/panpiper.egg-info/not-zip-safe
+-rw-r--r--   0 reneeoles   (501) staff       (20)       64 2024-04-03 23:22:11.000000 panpiper-1.0.2/panpiper.egg-info/requires.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        9 2024-04-03 23:22:11.000000 panpiper-1.0.2/panpiper.egg-info/top_level.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)       38 2024-04-03 23:22:11.558250 panpiper-1.0.2/setup.cfg
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1910 2024-04-03 23:21:18.000000 panpiper-1.0.2/setup.py
```

### Comparing `panpiper-1.0.1/LICENSE` & `panpiper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/PKG-INFO` & `panpiper-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 Metadata-Version: 2.1
 Name: panpiper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Panpiper: snakemake workflow for bacterial isolate analysis
 Home-page: https://github.com/rolesucsd/Panpiper
 Author: Renee Oles
 Author-email: roles@health.ucsd.edu
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
-Requires-Dist: biopython>=1.78
-Requires-Dist: pandas>=1.0.0
-Requires-Dist: numpy>=1.19.2
-Requires-Dist: matplotlib>=3.1.0
-Requires-Dist: seaborn>=0.10.0
-Requires-Dist: scikit-learn>=0.22.0
-Requires-Dist: scipy>=1.4.0
-Requires-Dist: scikit-bio>=0.5.6
-Requires-Dist: umap-learn>=0.4.0
-Requires-Dist: dendropy>=4.5.0
-Requires-Dist: PyYAML>=5.3
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
+Requires-Dist: umap-learn
+Requires-Dist: biopython
 
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 # Panpiper
 
 This package conducts bacterial isolate analysis for one species.  
 
 * Assembly
     * Using [shovill](https://github.com/tseemann/shovill) the paired fastq files are assembled and sorted into ones which pass and fail assembly
 * Quality control
-    * The assemblies are analyzed with [CheckM](https://github.com/Ecogenomics/CheckM) and [FastANI](https://github.com/ParBLiSS/FastANI)
+    * The assemblies are analyzed with [CheckM2](https://github.com/chklovski/CheckM2) and [FastANI](https://github.com/ParBLiSS/FastANI)
     * Based on user-defined thresholds the samples are sorted into ones which pass or don't pass requirements
 * Pangenome analysis
-    * A pangenome is created with the assemblies using [Panaroo](https://github.com/gtonkinhill/panaroo) and annotated with [AMRFinderPlus](https://github.com/ncbi/amr), [Bakta](https://github.com/oschwengers/bakta), [EggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper), and [Kraken2](https://github.com/DerrickWood/kraken2)
+    * A pangenome is created with the assemblies using [Panaroo](https://github.com/gtonkinhill/panaroo) and annotated with [AMRFinderPlus](https://github.com/ncbi/amr), [Bakta](https://github.com/oschwengers/bakta), and [EggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper)
     * The core genome alignment is used to create a phylogenetic tree with [FastTree](http://www.microbesonline.org/fasttree/), [RAxML](https://github.com/stamatak/standard-RAxML), and [IQ-TREE](https://github.com/Cibiv/IQ-TREE)
-    * The samples are divided into phylogroups with [PopPUNK](https://github.com/bacpop/PopPUNK)
+    * The samples are divided into phylogroups
 * Genome-wide association study
     * The pangenome is used with a continuous or binary phenotype to conduct a genome-wide association study with [Pyseer](https://github.com/mgalardini/pyseer)
     * The wrapper scripts used to analyze and filter the data are predominantly taken from the pyseer package.
 
 Note: Be sure to cite all packages used in the pipeline. 
 
 Credit: This package structure was inspired by the snakemake workflow [MAGinator](https://github.com/Russel88/MAGinator)
@@ -85,15 +79,15 @@
 * Assembly/  
     * incomplete_assembly_files.txt - samples for which assembly failed
     *  complete_assembly_files.txt - samples for which assemblies passed 
     * {sample}/  
         * contigs.fa - edited assembly 
 
 ### Quality control: 
-The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the name of the fasta file. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
+The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the directory names. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
 
 Additional parameters that may be included:
 * --ani_cutoff : percent identity to reference cutoff (default 95)
 * --n50 : N50 cutoff (default 5000)
 * --contig_number : number of contigs cutoff (default 1000)
 
 ```sh
@@ -128,27 +122,30 @@
     * Bakta/  
         * {sample}/ - contains Bakta output for each sample
     * Unitig/  
         * unitig.pyseer.gz - the full unitig summary of all samples
     * Phylogeny/ - contains the intermediate trees 
     * Panaroo/ - contains the full pangenome summary as well as Bakta annotation for the pangenome
     * AMR/ - contains the full AMR report for each sample
-    * Kraken/ - contains the full Kraken report for each sample
     * Phylogroups/ - contains the full division process for phylogroups
     * Summary/  
         * AMR.txt - the summary of AMR hits
         * amr.png - visualization of AMR as a heatmap
         * amr_wide.txt - reformat of AMR hits from long to wide
         * core_gene_alignment.aln.iqtree - the final nwk tree
-        * db_clusters.csv - the final phylogroup clusters
-        * krakn_ag.txt - the full kraken summary
         * mash.tsv - the full mash distance matrix 
         * pan_genome_reference.faa - all the proteins in the pangenome
         * pan_genome_reference.tsv - the list of all proteins in the pangenome
         * Summary.emapper.annotations - Eggnog-Mapper annotation
+        * genes_anno.txt - annotation of each protein in the pangenome
+        * genes_long.txt - dataframe of each protein in the pangenome and corresponding proteins in each isolate
+        * genes_matrix.txt - a matrix of gene presence/absence for all isolates 
+
+#### Visualization tools:
+This output can further be visualized using the streamlit app [Panpiper streamlit](https://panpiper.streamlit.app/)
 
 ### Genome-wide association study: 
 The gene and structure presence/absence files should be the result of Panaroo or Roary - from Panaroo this is the .RTab file. The unitig file is a result of unitig-caller; this file should be gzipped. The tree file can be any newick tree - if this pipeline has been followed to this point, we would recommend the tree file from iqtree. Finally, the reference file is a tab-delimited list of files to be used for unitig annotation. The format is file.fna file.gff2 {draft, ref}. 
 
 ```sh
 panpiper -w pyseer  -o {ouput directory} -g {gene presence absence file} -p {structure presence absence file} -u {unitig file} -t {tree file from iqtree} -r {reference file}
 ```
@@ -168,13 +165,7 @@
 
 ### Run on a compute cluster
 To run on a compute cluster, a profile folder must be specified which should contain a config.yaml file. Details on what to include in the config file can be found [here](https://snakemake.readthedocs.io/en/stable/executing/cli.html#profiles).
 
 ```sh
 panpiper ... --cluster --profile {profile folder}
 ```
-
-
-### Potential errors
-1. Kraken - "Error loading hash table" - you may need to request more memory 
-2. Kraken - database download errors - I suggest downloading the database manually as it can be very glitchy 
-
```

### Comparing `panpiper-1.0.1/README.md` & `panpiper-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # Panpiper
 
 This package conducts bacterial isolate analysis for one species.  
 
 * Assembly
     * Using [shovill](https://github.com/tseemann/shovill) the paired fastq files are assembled and sorted into ones which pass and fail assembly
 * Quality control
-    * The assemblies are analyzed with [CheckM](https://github.com/Ecogenomics/CheckM) and [FastANI](https://github.com/ParBLiSS/FastANI)
+    * The assemblies are analyzed with [CheckM2](https://github.com/chklovski/CheckM2) and [FastANI](https://github.com/ParBLiSS/FastANI)
     * Based on user-defined thresholds the samples are sorted into ones which pass or don't pass requirements
 * Pangenome analysis
-    * A pangenome is created with the assemblies using [Panaroo](https://github.com/gtonkinhill/panaroo) and annotated with [AMRFinderPlus](https://github.com/ncbi/amr), [Bakta](https://github.com/oschwengers/bakta), [EggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper), and [Kraken2](https://github.com/DerrickWood/kraken2)
+    * A pangenome is created with the assemblies using [Panaroo](https://github.com/gtonkinhill/panaroo) and annotated with [AMRFinderPlus](https://github.com/ncbi/amr), [Bakta](https://github.com/oschwengers/bakta), and [EggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper)
     * The core genome alignment is used to create a phylogenetic tree with [FastTree](http://www.microbesonline.org/fasttree/), [RAxML](https://github.com/stamatak/standard-RAxML), and [IQ-TREE](https://github.com/Cibiv/IQ-TREE)
-    * The samples are divided into phylogroups with [PopPUNK](https://github.com/bacpop/PopPUNK)
+    * The samples are divided into phylogroups
 * Genome-wide association study
     * The pangenome is used with a continuous or binary phenotype to conduct a genome-wide association study with [Pyseer](https://github.com/mgalardini/pyseer)
     * The wrapper scripts used to analyze and filter the data are predominantly taken from the pyseer package.
 
 Note: Be sure to cite all packages used in the pipeline. 
 
 Credit: This package structure was inspired by the snakemake workflow [MAGinator](https://github.com/Russel88/MAGinator)
@@ -56,15 +56,15 @@
 * Assembly/  
     * incomplete_assembly_files.txt - samples for which assembly failed
     *  complete_assembly_files.txt - samples for which assemblies passed 
     * {sample}/  
         * contigs.fa - edited assembly 
 
 ### Quality control: 
-The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the name of the fasta file. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
+The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the directory names. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
 
 Additional parameters that may be included:
 * --ani_cutoff : percent identity to reference cutoff (default 95)
 * --n50 : N50 cutoff (default 5000)
 * --contig_number : number of contigs cutoff (default 1000)
 
 ```sh
@@ -99,27 +99,30 @@
     * Bakta/  
         * {sample}/ - contains Bakta output for each sample
     * Unitig/  
         * unitig.pyseer.gz - the full unitig summary of all samples
     * Phylogeny/ - contains the intermediate trees 
     * Panaroo/ - contains the full pangenome summary as well as Bakta annotation for the pangenome
     * AMR/ - contains the full AMR report for each sample
-    * Kraken/ - contains the full Kraken report for each sample
     * Phylogroups/ - contains the full division process for phylogroups
     * Summary/  
         * AMR.txt - the summary of AMR hits
         * amr.png - visualization of AMR as a heatmap
         * amr_wide.txt - reformat of AMR hits from long to wide
         * core_gene_alignment.aln.iqtree - the final nwk tree
-        * db_clusters.csv - the final phylogroup clusters
-        * krakn_ag.txt - the full kraken summary
         * mash.tsv - the full mash distance matrix 
         * pan_genome_reference.faa - all the proteins in the pangenome
         * pan_genome_reference.tsv - the list of all proteins in the pangenome
         * Summary.emapper.annotations - Eggnog-Mapper annotation
+        * genes_anno.txt - annotation of each protein in the pangenome
+        * genes_long.txt - dataframe of each protein in the pangenome and corresponding proteins in each isolate
+        * genes_matrix.txt - a matrix of gene presence/absence for all isolates 
+
+#### Visualization tools:
+This output can further be visualized using the streamlit app [Panpiper streamlit](https://panpiper.streamlit.app/)
 
 ### Genome-wide association study: 
 The gene and structure presence/absence files should be the result of Panaroo or Roary - from Panaroo this is the .RTab file. The unitig file is a result of unitig-caller; this file should be gzipped. The tree file can be any newick tree - if this pipeline has been followed to this point, we would recommend the tree file from iqtree. Finally, the reference file is a tab-delimited list of files to be used for unitig annotation. The format is file.fna file.gff2 {draft, ref}. 
 
 ```sh
 panpiper -w pyseer  -o {ouput directory} -g {gene presence absence file} -p {structure presence absence file} -u {unitig file} -t {tree file from iqtree} -r {reference file}
 ```
@@ -139,13 +142,7 @@
 
 ### Run on a compute cluster
 To run on a compute cluster, a profile folder must be specified which should contain a config.yaml file. Details on what to include in the config file can be found [here](https://snakemake.readthedocs.io/en/stable/executing/cli.html#profiles).
 
 ```sh
 panpiper ... --cluster --profile {profile folder}
 ```
-
-
-### Potential errors
-1. Kraken - "Error loading hash table" - you may need to request more memory 
-2. Kraken - database download errors - I suggest downloading the database manually as it can be very glitchy 
-
```

### Comparing `panpiper-1.0.1/panpiper/main.py` & `panpiper-1.0.2/panpiper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,16 @@
         '--dry_run', help='Only run specific snakemake command. For debug purposes', action='store_true')
     apo.add_argument(
         '--unlock', help='Unlock snakemake directory in case of unexpected exists, then exit', action='store_true')
 
     # Parameters
     # Defaults set for Bacteroides fragilis
     app = ap.add_argument_group('parameters')
+    apo.add_argument(
+        '--threads', help='Specify the number of threads', default="8", type=str)
     app.add_argument(
         '--ani_cutoff', help='Average percent identity to reference cutoff', default=95, type=float)
     app.add_argument('--contig_number',
                      help='Max number of contigs', default=1000, type=int)
     app.add_argument('--n50', help='N50 cutoff', default=5000, type=int)
     app.add_argument('--eggnog_dir', help='Path to the eggnog database directory',
                      default=os.path.join(_ROOT, "databases", "eggnog"), type=str)
```

### Comparing `panpiper-1.0.1/panpiper/test.py` & `panpiper-1.0.2/panpiper/test.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper/tests/test_main.py` & `panpiper-1.0.2/panpiper/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper/tests/test_scripts/filter_isolates.py` & `panpiper-1.0.2/panpiper/tests/test_scripts/filter_isolates.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper/tests/test_scripts/test_concat_amrfinder.py` & `panpiper-1.0.2/panpiper/tests/test_scripts/test_concat_amrfinder.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper/workflow/assembly.smk` & `panpiper-1.0.2/panpiper/workflow/assembly.smk`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper/workflow/pangenome.smk` & `panpiper-1.0.2/panpiper/workflow/pangenome.smk`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper/workflow/pyseer.smk` & `panpiper-1.0.2/panpiper/workflow/pyseer.smk`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper/workflow/quality.smk` & `panpiper-1.0.2/panpiper/workflow/quality.smk`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 param_dict = {x[0]: x[1] for x in fl}
 
 PARAMS_REF = param_dict["ref"]
 ANI_CUTOFF = param_dict["ani_cutoff"]
 CONTIG_NUMBER = param_dict["contig_number"]
 N50 = param_dict["n50"]
 CHECKM = param_dict['checkm_dir']
+THREADS = param_dict['threads']
+
 
 def read_complete_files():
     with open(SAMPLE_LIST) as f:
         raw_reads = [sample for sample in f.read().split('\n') if len(sample) > 0]
         return(raw_reads)
 READS = read_complete_files()
 
@@ -75,26 +77,27 @@
         "reformat.sh in={input.assembly} out={output.fna} minlength={params.contig} &> {log}"
 
 rule run_checkm2:
     input:
         file=os.path.join(OUT,"Quality/Samples/{file}/{file}.fna"),
     params:
         binset=os.path.join(OUT,"Quality/checkm"),
-        checkmdb=os.path.join(CHECKM,"Quality/uniref100.KO.1.dmnd"),
+        checkmdb=os.path.join(CHECKM,"uniref100.KO.1.dmnd"),
+        threads=THREADS
     conda:
         "envs/checkm2.yml"
     log:
         log=os.path.join(OUT,"report/checkm2_{file}.log"),
     benchmark:
         os.path.join(OUT,"benchmark/checkm2_{file}.benchmark"),
     output:
         stats=os.path.join(OUT,"Quality/Samples/{file}/checkm/quality_report.tsv"),
     shell:
         """
-        checkm2 predict --threads 20 --input {input} --database_path {params.checkmdb} --output-directory {params.binset} --force &> {log}
+        checkm2 predict --threads {params.threads} --input {input} --database_path {params.checkmdb} --output-directory {params.binset} --force &> {log}
         """
 
 rule checkm_to_graph:
     input:
         stats=expand(os.path.join(OUT,"Quality/Samples/{file}/checkm/quality_report.tsv"), file=READS),
     params:
         outpref=OUT,
```

### Comparing `panpiper-1.0.1/panpiper/workflow.py` & `panpiper-1.0.2/panpiper/workflow.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.1/panpiper.egg-info/PKG-INFO` & `panpiper-1.0.2/panpiper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 Metadata-Version: 2.1
 Name: panpiper
-Version: 1.0.1
+Version: 1.0.2
 Summary: Panpiper: snakemake workflow for bacterial isolate analysis
 Home-page: https://github.com/rolesucsd/Panpiper
 Author: Renee Oles
 Author-email: roles@health.ucsd.edu
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
-Requires-Dist: biopython>=1.78
-Requires-Dist: pandas>=1.0.0
-Requires-Dist: numpy>=1.19.2
-Requires-Dist: matplotlib>=3.1.0
-Requires-Dist: seaborn>=0.10.0
-Requires-Dist: scikit-learn>=0.22.0
-Requires-Dist: scipy>=1.4.0
-Requires-Dist: scikit-bio>=0.5.6
-Requires-Dist: umap-learn>=0.4.0
-Requires-Dist: dendropy>=4.5.0
-Requires-Dist: PyYAML>=5.3
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
+Requires-Dist: umap-learn
+Requires-Dist: biopython
 
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 # Panpiper
 
 This package conducts bacterial isolate analysis for one species.  
 
 * Assembly
     * Using [shovill](https://github.com/tseemann/shovill) the paired fastq files are assembled and sorted into ones which pass and fail assembly
 * Quality control
-    * The assemblies are analyzed with [CheckM](https://github.com/Ecogenomics/CheckM) and [FastANI](https://github.com/ParBLiSS/FastANI)
+    * The assemblies are analyzed with [CheckM2](https://github.com/chklovski/CheckM2) and [FastANI](https://github.com/ParBLiSS/FastANI)
     * Based on user-defined thresholds the samples are sorted into ones which pass or don't pass requirements
 * Pangenome analysis
-    * A pangenome is created with the assemblies using [Panaroo](https://github.com/gtonkinhill/panaroo) and annotated with [AMRFinderPlus](https://github.com/ncbi/amr), [Bakta](https://github.com/oschwengers/bakta), [EggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper), and [Kraken2](https://github.com/DerrickWood/kraken2)
+    * A pangenome is created with the assemblies using [Panaroo](https://github.com/gtonkinhill/panaroo) and annotated with [AMRFinderPlus](https://github.com/ncbi/amr), [Bakta](https://github.com/oschwengers/bakta), and [EggNOG-mapper](https://github.com/eggnogdb/eggnog-mapper)
     * The core genome alignment is used to create a phylogenetic tree with [FastTree](http://www.microbesonline.org/fasttree/), [RAxML](https://github.com/stamatak/standard-RAxML), and [IQ-TREE](https://github.com/Cibiv/IQ-TREE)
-    * The samples are divided into phylogroups with [PopPUNK](https://github.com/bacpop/PopPUNK)
+    * The samples are divided into phylogroups
 * Genome-wide association study
     * The pangenome is used with a continuous or binary phenotype to conduct a genome-wide association study with [Pyseer](https://github.com/mgalardini/pyseer)
     * The wrapper scripts used to analyze and filter the data are predominantly taken from the pyseer package.
 
 Note: Be sure to cite all packages used in the pipeline. 
 
 Credit: This package structure was inspired by the snakemake workflow [MAGinator](https://github.com/Russel88/MAGinator)
@@ -85,15 +79,15 @@
 * Assembly/  
     * incomplete_assembly_files.txt - samples for which assembly failed
     *  complete_assembly_files.txt - samples for which assemblies passed 
     * {sample}/  
         * contigs.fa - edited assembly 
 
 ### Quality control: 
-The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the name of the fasta file. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
+The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the directory names. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
 
 Additional parameters that may be included:
 * --ani_cutoff : percent identity to reference cutoff (default 95)
 * --n50 : N50 cutoff (default 5000)
 * --contig_number : number of contigs cutoff (default 1000)
 
 ```sh
@@ -128,27 +122,30 @@
     * Bakta/  
         * {sample}/ - contains Bakta output for each sample
     * Unitig/  
         * unitig.pyseer.gz - the full unitig summary of all samples
     * Phylogeny/ - contains the intermediate trees 
     * Panaroo/ - contains the full pangenome summary as well as Bakta annotation for the pangenome
     * AMR/ - contains the full AMR report for each sample
-    * Kraken/ - contains the full Kraken report for each sample
     * Phylogroups/ - contains the full division process for phylogroups
     * Summary/  
         * AMR.txt - the summary of AMR hits
         * amr.png - visualization of AMR as a heatmap
         * amr_wide.txt - reformat of AMR hits from long to wide
         * core_gene_alignment.aln.iqtree - the final nwk tree
-        * db_clusters.csv - the final phylogroup clusters
-        * krakn_ag.txt - the full kraken summary
         * mash.tsv - the full mash distance matrix 
         * pan_genome_reference.faa - all the proteins in the pangenome
         * pan_genome_reference.tsv - the list of all proteins in the pangenome
         * Summary.emapper.annotations - Eggnog-Mapper annotation
+        * genes_anno.txt - annotation of each protein in the pangenome
+        * genes_long.txt - dataframe of each protein in the pangenome and corresponding proteins in each isolate
+        * genes_matrix.txt - a matrix of gene presence/absence for all isolates 
+
+#### Visualization tools:
+This output can further be visualized using the streamlit app [Panpiper streamlit](https://panpiper.streamlit.app/)
 
 ### Genome-wide association study: 
 The gene and structure presence/absence files should be the result of Panaroo or Roary - from Panaroo this is the .RTab file. The unitig file is a result of unitig-caller; this file should be gzipped. The tree file can be any newick tree - if this pipeline has been followed to this point, we would recommend the tree file from iqtree. Finally, the reference file is a tab-delimited list of files to be used for unitig annotation. The format is file.fna file.gff2 {draft, ref}. 
 
 ```sh
 panpiper -w pyseer  -o {ouput directory} -g {gene presence absence file} -p {structure presence absence file} -u {unitig file} -t {tree file from iqtree} -r {reference file}
 ```
@@ -168,13 +165,7 @@
 
 ### Run on a compute cluster
 To run on a compute cluster, a profile folder must be specified which should contain a config.yaml file. Details on what to include in the config file can be found [here](https://snakemake.readthedocs.io/en/stable/executing/cli.html#profiles).
 
 ```sh
 panpiper ... --cluster --profile {profile folder}
 ```
-
-
-### Potential errors
-1. Kraken - "Error loading hash table" - you may need to request more memory 
-2. Kraken - database download errors - I suggest downloading the database manually as it can be very glitchy 
-
```

### Comparing `panpiper-1.0.1/setup.py` & `panpiper-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,53 +10,46 @@
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="panpiper",
-    version="1.0.1",
+    name="panpiper", 
+    version="1.0.2",
     license='BSD-3-Clause',
     author="Renee Oles",
     author_email="roles@health.ucsd.edu",
     description="Panpiper: snakemake workflow for bacterial isolate analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rolesucsd/Panpiper",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: BSD License",  # Updated to reflect BSD license as mentioned
+        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Development Status :: 3 - Alpha"],
     python_requires='>=3.5',
     install_requires=[
-    "setuptools",
-    "biopython>=1.78",
-    "pandas>=1.0.0",
-    "numpy>=1.19.2",
-    "matplotlib>=3.1.0",
-    "seaborn>=0.10.0",
-    "scikit-learn>=0.22.0",
-    "scipy>=1.4.0",
-    "scikit-bio>=0.5.6",
-    "umap-learn>=0.4.0",
-    "dendropy>=4.5.0",
-    "PyYAML>=5.3"  # Add PyYAML, adjust version as needed
-    ],
-    entry_points={
-        'console_scripts': ['panpiper=panpiper.main:cli']
+        "setuptools",
+        "matplotlib",
+        "seaborn",
+        "scikit-learn",
+        "umap-learn",
+        "biopython"],
+    entry_points = {
+        'console_scripts': ['panpiper = panpiper.main:cli']
     },
     include_package_data=True,
     zip_safe=False,
     package_data={
     'panpiper': [
-        'databses/*'
-        'databses/*'
         'workflow/*',  # This includes files directly under workflow
         'workflow/envs/*',  # This includes files in the envs subdirectory
         'workflow/scripts/*'  # This includes files in the scripts subdirectory
+        'databases/*'  # This includes files in the scripts subdirectory
+        'databases/checkm2/*'  # This includes files in the scripts subdirectory
         ]
     }
 )
```

