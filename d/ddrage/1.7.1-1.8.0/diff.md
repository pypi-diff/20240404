# Comparing `tmp/ddrage-1.7.1.tar.gz` & `tmp/ddrage-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddrage-1.7.1.tar", last modified: Thu Apr 16 14:27:03 2020, max compression
+gzip compressed data, was "ddrage-1.8.0.tar", last modified: Thu Apr  4 20:02:24 2024, max compression
```

## Comparing `ddrage-1.7.1.tar` & `ddrage-1.8.0.tar`

### file list

```diff
@@ -1,47 +1,98 @@
-drwxrwxr-x   0 timm      (1000) timm      (1000)        0 2020-04-16 14:27:03.000000 ddrage-1.7.1/
-drwxrwxr-x   0 timm      (1000) timm      (1000)        0 2020-04-16 14:27:03.000000 ddrage-1.7.1/ddrage.egg-info/
--rw-rw-r--   0 timm      (1000) timm      (1000)     1147 2020-04-16 14:27:03.000000 ddrage-1.7.1/ddrage.egg-info/SOURCES.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)        1 2020-04-16 14:27:02.000000 ddrage-1.7.1/ddrage.egg-info/dependency_links.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)        7 2020-04-16 14:27:02.000000 ddrage-1.7.1/ddrage.egg-info/top_level.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)      354 2020-04-16 14:27:02.000000 ddrage-1.7.1/ddrage.egg-info/entry_points.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)      124 2020-04-16 14:27:02.000000 ddrage-1.7.1/ddrage.egg-info/requires.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)     4771 2020-04-16 14:27:02.000000 ddrage-1.7.1/ddrage.egg-info/PKG-INFO
--rw-rw-r--   0 timm      (1000) timm      (1000)       38 2020-04-16 14:27:03.000000 ddrage-1.7.1/setup.cfg
-drwxrwxr-x   0 timm      (1000) timm      (1000)        0 2020-04-16 14:27:03.000000 ddrage-1.7.1/ddrage/
--rw-rw-r--   0 timm      (1000) timm      (1000)    37100 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/mutation_model.py
-drwxrwxr-x   0 timm      (1000) timm      (1000)        0 2020-04-16 14:27:03.000000 ddrage-1.7.1/ddrage/barcode_handler/
--rw-rw-r--   0 timm      (1000) timm      (1000)    31280 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/barcode_handler/barcode_file_parser.py
-drwxrwxr-x   0 timm      (1000) timm      (1000)        0 2020-04-16 14:27:03.000000 ddrage-1.7.1/ddrage/barcode_handler/barcodes/
--rw-rw-r--   0 timm      (1000) timm      (1000)     4225 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/barcode_handler/barcodes/big.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)    80912 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/barcode_handler/barcodes/huge.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)      501 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/barcode_handler/barcodes/small.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)     1250 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/barcode_handler/barcodes/barcodes.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)     4211 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/barcode_handler/barcodes/full.txt
--rw-rw-r--   0 timm      (1000) timm      (1000)        0 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/barcode_handler/__init__.py
--rw-rw-r--   0 timm      (1000) timm      (1000)    24302 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/plotting.py
--rw-rw-r--   0 timm      (1000) timm      (1000)    26614 2020-04-16 14:23:49.000000 ddrage-1.7.1/ddrage/__main__.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     3215 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/initialization.py
-drwxrwxr-x   0 timm      (1000) timm      (1000)        0 2020-04-16 14:27:03.000000 ddrage-1.7.1/ddrage/tools/
--rw-rw-r--   0 timm      (1000) timm      (1000)     8255 2020-04-16 14:21:46.000000 ddrage-1.7.1/ddrage/tools/bbd_visualization.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     5581 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/tools/randomize_fastq.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     3137 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/tools/split_by_p7_barcode.py
--rw-rw-r--   0 timm      (1000) timm      (1000)        0 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/tools/__init__.py
--rw-rw-r--   0 timm      (1000) timm      (1000)    10770 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/tools/learn_qmodel.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     2219 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/tools/remove_annotation.py
--rw-rw-r--   0 timm      (1000) timm      (1000)        0 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/__init__.py
--rw-rw-r--   0 timm      (1000) timm      (1000)    23980 2020-04-16 14:21:46.000000 ddrage-1.7.1/ddrage/distributions.py
-drwxrwxr-x   0 timm      (1000) timm      (1000)        0 2020-04-16 14:27:03.000000 ddrage-1.7.1/ddrage/quality_profiles/
--rw-rw-r--   0 timm      (1000) timm      (1000)   113958 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/quality_profiles/L100-Q70-B.qmodel.npz
--rw-rw-r--   0 timm      (1000) timm      (1000)   143494 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/quality_profiles/L126-Q70.qmodel.npz
--rw-rw-r--   0 timm      (1000) timm      (1000)   170758 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/quality_profiles/L150-Q70.qmodel.npz
--rw-rw-r--   0 timm      (1000) timm      (1000)   113958 2018-08-21 10:52:16.000000 ddrage-1.7.1/ddrage/quality_profiles/L100-Q70-A.qmodel.npz
--rw-rw-r--   0 timm      (1000) timm      (1000)     5043 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/barcodes.py
--rw-rw-r--   0 timm      (1000) timm      (1000)    36420 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/rad_reads.py
--rw-rw-r--   0 timm      (1000) timm      (1000)    34545 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/rad_locus.py
--rw-rw-r--   0 timm      (1000) timm      (1000)    29519 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/output.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     9543 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/read_mutation_handling.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     9193 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/generation.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     9663 2020-04-16 11:00:53.000000 ddrage-1.7.1/ddrage/postprocessors.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     2109 2020-04-16 14:23:18.000000 ddrage-1.7.1/setup.py
--rw-rw-r--   0 timm      (1000) timm      (1000)     2827 2020-04-16 11:00:53.000000 ddrage-1.7.1/README.rst
--rw-rw-r--   0 timm      (1000) timm      (1000)     4771 2020-04-16 14:27:03.000000 ddrage-1.7.1/PKG-INFO
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.753764 ddrage-1.8.0/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      120 2020-12-23 14:57:43.000000 ddrage-1.8.0/.gitignore
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    12775 2024-04-04 19:49:01.000000 ddrage-1.8.0/CHANGELOG.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1079 2024-04-04 17:56:58.000000 ddrage-1.8.0/LICENSE.rst
+-rw-r--r--   0 m00am     (1000) m00am     (1000)     6069 2024-04-04 20:02:24.753764 ddrage-1.8.0/PKG-INFO
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3177 2024-04-04 19:49:01.000000 ddrage-1.8.0/README.rst
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.745764 ddrage-1.8.0/ddrage/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        0 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/__init__.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    26614 2024-04-04 19:49:01.000000 ddrage-1.8.0/ddrage/__main__.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.745764 ddrage-1.8.0/ddrage/barcode_handler/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      858 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/README.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        0 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/__init__.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    31280 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/barcode_file_parser.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.745764 ddrage-1.8.0/ddrage/barcode_handler/barcodes/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1250 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/barcodes/barcodes.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4225 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/barcodes/big.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4211 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/barcodes/full.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    80912 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/barcodes/huge.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      501 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcode_handler/barcodes/small.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     5043 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/barcodes.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    23980 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/distributions.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     9193 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/generation.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3215 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/initialization.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    37100 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/mutation_model.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    29519 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/output.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    24302 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/plotting.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     9663 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/postprocessors.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.749764 ddrage-1.8.0/ddrage/quality_profiles/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)   113958 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/quality_profiles/L100-Q70-A.qmodel.npz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)   113958 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/quality_profiles/L100-Q70-B.qmodel.npz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)   143494 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/quality_profiles/L126-Q70.qmodel.npz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)   170758 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/quality_profiles/L150-Q70.qmodel.npz
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    34545 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/rad_locus.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    36420 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/rad_reads.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     9543 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/read_mutation_handling.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.749764 ddrage-1.8.0/ddrage/tools/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        0 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/tools/__init__.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     8249 2024-04-04 19:49:01.000000 ddrage-1.8.0/ddrage/tools/bbd_visualization.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    10770 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/tools/learn_qmodel.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     5581 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/tools/randomize_fastq.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2219 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/tools/remove_annotation.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3137 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage/tools/split_by_p7_barcode.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.753764 ddrage-1.8.0/ddrage.egg-info/
+-rw-r--r--   0 m00am     (1000) m00am     (1000)     6069 2024-04-04 20:02:24.000000 ddrage-1.8.0/ddrage.egg-info/PKG-INFO
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2577 2024-04-04 20:02:24.000000 ddrage-1.8.0/ddrage.egg-info/SOURCES.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        1 2024-04-04 20:02:24.000000 ddrage-1.8.0/ddrage.egg-info/dependency_links.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      353 2024-04-04 20:02:24.000000 ddrage-1.8.0/ddrage.egg-info/entry_points.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      116 2024-04-04 20:02:24.000000 ddrage-1.8.0/ddrage.egg-info/requires.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)        7 2024-04-04 20:02:24.000000 ddrage-1.8.0/ddrage.egg-info/top_level.txt
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      104 2020-12-23 14:57:43.000000 ddrage-1.8.0/ddrage.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.749764 ddrage-1.8.0/docs/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      261 2024-04-04 19:52:29.000000 ddrage-1.8.0/docs/.readthedocs.yaml
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     8065 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/Makefile
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     7737 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/make.bat
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       59 2024-04-04 19:49:01.000000 ddrage-1.8.0/docs/requirements.txt
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.749764 ddrage-1.8.0/docs/source/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       33 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/changelog.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     9717 2024-04-04 19:49:01.000000 ddrage-1.8.0/docs/source/conf.py
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.749764 ddrage-1.8.0/docs/source/documentation/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3015 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/documentation/assumptions_and_notation.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2406 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/documentation/enzymes.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      790 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/documentation/index.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     4865 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/documentation/input_format.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    17079 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/documentation/output_format.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    13344 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/documentation/parameters.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     5722 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/documentation/tools.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     6547 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/faqs.rst
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.753764 ddrage-1.8.0/docs/source/figures/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    36709 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/overlap.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    33476 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/pd.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2959 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/plot_coverage_distribution.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     6116 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/plot_distribution_heatmap.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2230 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/plot_pd.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3333 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/plot_versus.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2142 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/plot_ztpd.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    15321 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/quality_styles.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)   114195 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/read_coverage_distribution.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    22016 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/read_structure.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    13111 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/truncation.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    54625 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/versus.svg
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)    69399 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/figures/ztpd.svg
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.753764 ddrage-1.8.0/docs/source/getting-started/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2487 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/getting-started/cookbook.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1497 2024-04-04 19:49:01.000000 ddrage-1.8.0/docs/source/getting-started/index.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     3874 2024-04-04 19:49:01.000000 ddrage-1.8.0/docs/source/getting-started/tutorial.rst
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      366 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/index.rst
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.753764 ddrage-1.8.0/docs/source/myhaiku/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2880 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/myhaiku/layout.html
+drwxrwxr-x   0 m00am     (1000) m00am     (1000)        0 2024-04-04 20:02:24.753764 ddrage-1.8.0/docs/source/myhaiku/static/
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     1128 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/myhaiku/static/alert_info_32.png
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      944 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/myhaiku/static/alert_warning_32.png
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       82 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/myhaiku/static/bg-page.png
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      165 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/myhaiku/static/bullet_orange.png
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     7034 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/myhaiku/static/haiku.css_t
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      248 2020-12-23 14:57:43.000000 ddrage-1.8.0/docs/source/myhaiku/theme.conf
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)     2253 2024-04-04 19:49:01.000000 ddrage-1.8.0/pyproject.toml
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)      104 2020-12-23 14:57:43.000000 ddrage-1.8.0/rage.py
+-rw-rw-r--   0 m00am     (1000) m00am     (1000)       38 2024-04-04 20:02:24.753764 ddrage-1.8.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ddrage-1.7.1/ddrage/mutation_model.py` & `ddrage-1.8.0/ddrage/mutation_model.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/barcode_handler/barcode_file_parser.py` & `ddrage-1.8.0/ddrage/barcode_handler/barcode_file_parser.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/barcode_handler/barcodes/big.txt` & `ddrage-1.8.0/ddrage/barcode_handler/barcodes/big.txt`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/barcode_handler/barcodes/huge.txt` & `ddrage-1.8.0/ddrage/barcode_handler/barcodes/huge.txt`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/barcode_handler/barcodes/barcodes.txt` & `ddrage-1.8.0/ddrage/barcode_handler/barcodes/barcodes.txt`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/barcode_handler/barcodes/full.txt` & `ddrage-1.8.0/ddrage/barcode_handler/barcodes/full.txt`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/plotting.py` & `ddrage-1.8.0/ddrage/plotting.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/__main__.py` & `ddrage-1.8.0/ddrage/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .postprocessors import SingletonGenerator
 from .postprocessors import HighlyRepetitiveLocusGenerator as HRLGenerator
 from .distributions import validate_probability_parameters, initialize_coverage_generators
 from .generation import initialize_quality_model, FragmentGenerator, count_fragments
 from . import barcodes
 from . import output
 
-__version__ = "1.7.1"
+__version__ = "1.8.0"
 
 
 def all_seqs_to_bytes(args):
     """Convert all sequences (overhangs, recognition sites) to bytes."""
     def to_bytes(seq):
         if isinstance(seq, bytes):
             return seq
```

### Comparing `ddrage-1.7.1/ddrage/initialization.py` & `ddrage-1.8.0/ddrage/initialization.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/tools/bbd_visualization.py` & `ddrage-1.8.0/ddrage/tools/bbd_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from tornado.ioloop import IOLoop
 
 from bokeh.application.handlers import FunctionHandler
 from bokeh.application import Application
 
 from bokeh.io import curdoc
-from bokeh.layouts import row, widgetbox
-from bokeh.models import ColumnDataSource, Span, Label, LabelSet
+from bokeh.layouts import row
+from bokeh.models import ColumnDataSource, Column, Span, Label, LabelSet
 from bokeh.models.ranges import Range1d
 from bokeh.models.widgets import Slider, TextInput
 from bokeh.plotting import figure
 from bokeh.server.server import Server
 
 
 ELEMENTS = dict()
@@ -201,15 +201,15 @@
 
     # link on_change functions to widgets
     text.on_change('value', update_title)
     for w in [a_slider, b_slider, ds_slider]:
         w.on_change('value', update_data)
 
     # Set up layouts and add to document
-    inputs = widgetbox(text, a_slider, b_slider, ds_slider, parameters_text)
+    inputs = Column(text, a_slider, b_slider, ds_slider, parameters_text)
     doc.add_root(row(inputs, plot))
     
     doc.title = "BBD with moved mean"
     
 
 def main_standalone():
     io_loop = IOLoop.current()
```

### Comparing `ddrage-1.7.1/ddrage/tools/randomize_fastq.py` & `ddrage-1.8.0/ddrage/tools/randomize_fastq.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/tools/split_by_p7_barcode.py` & `ddrage-1.8.0/ddrage/tools/split_by_p7_barcode.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/tools/learn_qmodel.py` & `ddrage-1.8.0/ddrage/tools/learn_qmodel.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/tools/remove_annotation.py` & `ddrage-1.8.0/ddrage/tools/remove_annotation.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/distributions.py` & `ddrage-1.8.0/ddrage/distributions.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/quality_profiles/L100-Q70-B.qmodel.npz` & `ddrage-1.8.0/ddrage/quality_profiles/L100-Q70-B.qmodel.npz`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/quality_profiles/L126-Q70.qmodel.npz` & `ddrage-1.8.0/ddrage/quality_profiles/L126-Q70.qmodel.npz`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/quality_profiles/L150-Q70.qmodel.npz` & `ddrage-1.8.0/ddrage/quality_profiles/L150-Q70.qmodel.npz`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/quality_profiles/L100-Q70-A.qmodel.npz` & `ddrage-1.8.0/ddrage/quality_profiles/L100-Q70-A.qmodel.npz`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/barcodes.py` & `ddrage-1.8.0/ddrage/barcodes.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/rad_reads.py` & `ddrage-1.8.0/ddrage/rad_reads.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/rad_locus.py` & `ddrage-1.8.0/ddrage/rad_locus.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/output.py` & `ddrage-1.8.0/ddrage/output.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/read_mutation_handling.py` & `ddrage-1.8.0/ddrage/read_mutation_handling.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/generation.py` & `ddrage-1.8.0/ddrage/generation.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/ddrage/postprocessors.py` & `ddrage-1.8.0/ddrage/postprocessors.py`

 * *Files identical despite different names*

### Comparing `ddrage-1.7.1/README.rst` & `ddrage-1.8.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4390216.svg 
+   :target: https://doi.org/10.5281/zenodo.4390216
+
 #############################
 ddRAGE - ddRAD Data Generator
 #############################
 
 
 ddRAGE (ddRAD Data Generator) is a software to simulate double digest restriction site associated DNA sequencing reads.
 The generated data sets can be used to test ddRAD analysis tools and validate their results.
@@ -14,20 +17,21 @@
 .. _bioconda: https://bioconda.github.io/recipes/ddrage/README.html
 
 
 *******************
 System Requirements
 *******************
 
-- python >= 3.5
+- python >= 3.8
 - numba
 - numpy
 - matplotlib
 - pyyaml
 - scipy
+- seaborn
 
 
 For the docs:
 
 - sphinx
 
 For parameter visualization:
@@ -42,23 +46,24 @@
 We recommend the installation using conda:
 
 .. code-block:: shell
 
    $ conda create -n ddrage -c bioconda ddrage
    $ source activate ddrage
 
-Alternatively, you can download the source code from `bitbucket`_ and install it using the setup script:
+Alternatively, you can download the source code from `bitbucket`_ and install it using pip:
 
 .. code-block:: shell
 
    $ git clone https://bitbucket.org/genomeinformatics/rage.git ddrage
    $ cd ddrage
-   /rage$ python setup.py install
-
-In this case you have to install the requirements listed above.
+   /ddrage$ pip install .  # basic version
+   # OR
+   # to install with support to build the documentation and visualize bbd parameters
+   /ddrage$ pip install .[documentation,BBD-visualization]
 
 
 *****
 Usage
 *****
 
 To simulate a ddRAD data set, call ddrage from the command line:
@@ -81,16 +86,16 @@
 *************
 Citing ddRAGE
 *************
 
 Our paper describing ddRAGE has been published in `Molecular Ecology Resources <http://onlinelibrary.wiley.com/doi/10.1111/1755-0998.12743/full>`_.
 You can cite it as follows:
 
-.. code-block:: text
-                
+.. code-block::
+
     Timm H, Weigand H, Weiss M, Leese F, Rahmann S. ddRAGE: A data set generator to evaluate ddRADseq analysis software. Mol Ecol Resour. 2018;18:681–690. https://doi.org/10.1111/1755-0998.12743
 
 BibTeX version:
 
 .. code-block:: latex
 
     @article{timm2018ddrage,
@@ -100,7 +105,9 @@
       volume={18},
       number={3},
       pages={681--690},
       year={2018},
       url = {http://dx.doi.org/10.1111/1755-0998.12743},
       doi = {10.1111/1755-0998.12743},
     }
+
+The source code itself is also published on `Zenodo <https://zenodo.org>`_ under the DOI `10.5281/zenodo.4390216 <https://doi.org/10.5281/zenodo.4390216>`_.
```

