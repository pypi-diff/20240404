# Comparing `tmp/cellxgene_census-1.9.0.tar.gz` & `tmp/cellxgene_census-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.9.0.tar", last modified: Fri Dec  8 17:58:31 2023, max compression
+gzip compressed data, was "cellxgene_census-1.9.1.tar", last modified: Wed Dec 13 17:46:22 2023, max compression
```

## Comparing `cellxgene_census-1.9.0.tar` & `cellxgene_census-1.9.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.414040 cellxgene_census-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-12-08 17:58:31.414040 cellxgene_census-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.406040 cellxgene_census-1.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 17:58:31.414040 cellxgene_census-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.402040 cellxgene_census-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.406040 cellxgene_census-1.9.0/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.406040 cellxgene_census-1.9.0/src/cellxgene_census/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.410040 cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.410040 cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/huggingface/cell_dataset_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/huggingface/geneformer_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    31201 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.410040 cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17641 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14388 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.410040 cellxgene_census-1.9.0/src/cellxgene_census/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/util/_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/experimental/util/_eager_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/src/cellxgene_census/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.414040 cellxgene_census-1.9.0/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-12-08 17:58:31.000000 cellxgene_census-1.9.0/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-12-08 17:58:31.000000 cellxgene_census-1.9.0/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 17:58:31.000000 cellxgene_census-1.9.0/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-08 17:58:31.000000 cellxgene_census-1.9.0/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-08 17:58:31.000000 cellxgene_census-1.9.0/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.410040 cellxgene_census-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   175591 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.410040 cellxgene_census-1.9.0/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.410040 cellxgene_census-1.9.0/tests/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.414040 cellxgene_census-1.9.0/tests/experimental/ml/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/ml/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/ml/huggingface/test_geneformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20599 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/ml/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.414040 cellxgene_census-1.9.0/tests/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (127)    10226 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/pp/test_hvg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/pp/test_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/pp/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 17:58:31.414040 cellxgene_census-1.9.0/tests/experimental/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/experimental/util/test_csr_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/test_lts_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11256 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-12-08 17:58:18.000000 cellxgene_census-1.9.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.668691 cellxgene_census-1.9.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.664692 cellxgene_census-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.668691 cellxgene_census-1.9.1/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.668691 cellxgene_census-1.9.1/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.668691 cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.672692 cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/huggingface/cell_dataset_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/huggingface/geneformer_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31201 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.672692 cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17641 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14388 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.672692 cellxgene_census-1.9.1/src/cellxgene_census/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/util/_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/experimental/util/_eager_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/src/cellxgene_census/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-12-13 17:46:22.000000 cellxgene_census-1.9.1/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-12-13 17:46:22.000000 cellxgene_census-1.9.1/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 17:46:22.000000 cellxgene_census-1.9.1/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2023-12-13 17:46:22.000000 cellxgene_census-1.9.1/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-13 17:46:22.000000 cellxgene_census-1.9.1/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.672692 cellxgene_census-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   175591 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/tests/experimental/ml/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/ml/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/ml/huggingface/test_geneformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20599 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/ml/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/tests/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/pp/test_hvg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/pp/test_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/pp/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 17:46:22.676692 cellxgene_census-1.9.1/tests/experimental/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/experimental/util/test_csr_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/test_lts_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2023-12-13 17:46:12.000000 cellxgene_census-1.9.1/tests/test_util.py
```

### Comparing `cellxgene_census-1.9.0/LICENSE` & `cellxgene_census-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/PKG-INFO` & `cellxgene_census-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.9.0
+Version: 1.9.1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative Foundation <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.9.0/README.md` & `cellxgene_census-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/pyproject.toml` & `cellxgene_census-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/__init__.py` & `cellxgene_census-1.9.1/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.9.1/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.9.1/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/_open.py` & `cellxgene_census-1.9.1/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.9.1/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.9.1/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/_embedding.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     # Currently, all embeddings are hosted in us-west-2 so use that as a default.
     # Allow the user to override for exceptional cases.
     context = _build_soma_tiledb_context("us-west-2", context)
 
     with soma.open(embedding_uri, context=context) as E:
         # read embedding metadata and decode the JSON-encoded string
-        embedding_metadata = json.loads(E.metadata["CxG_contrib_metadata"])
+        embedding_metadata = json.loads(E.metadata["CxG_embedding_info"])
         assert isinstance(embedding_metadata, dict)
 
     return cast(Dict[str, Any], embedding_metadata)
 
 
 def get_embedding(
     census_version: str,
@@ -109,15 +109,15 @@
     context = _build_soma_tiledb_context("us-west-2", context)
 
     # Attempt to resolve census version aliases
     census_directory = get_census_version_directory()
     resolved_census_version = census_directory.get(census_version, None)
 
     with soma.open(embedding_uri, context=context) as E:
-        embedding_metadata = json.loads(E.metadata["CxG_contrib_metadata"])
+        embedding_metadata = json.loads(E.metadata["CxG_embedding_info"])
 
         if resolved_census_version is None:
             warnings.warn(
                 "Unable to determine Census version - skipping validation of Census and embedding version.",
                 stacklevel=1,
             )
         elif resolved_census_version != census_directory.get(embedding_metadata["census_version"], None):
```

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/huggingface/cell_dataset_builder.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/huggingface/cell_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/huggingface/geneformer_tokenizer.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/huggingface/geneformer_tokenizer.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/ml/pytorch.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/ml/pytorch.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/_online.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/pp/_stats.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/pp/_stats.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/util/_csr_iter.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/util/_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census/experimental/util/_eager_iter.py` & `cellxgene_census-1.9.1/src/cellxgene_census/experimental/util/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.9.1/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.9.0
+Version: 1.9.1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative Foundation <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cellxgene_census-1.9.0/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.9.1/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/README.md` & `cellxgene_census-1.9.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/conftest.py` & `cellxgene_census-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/experimental/ml/huggingface/test_geneformer.py` & `cellxgene_census-1.9.1/tests/experimental/ml/huggingface/test_geneformer.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/experimental/ml/test_pytorch.py` & `cellxgene_census-1.9.1/tests/experimental/ml/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/experimental/pp/test_hvg.py` & `cellxgene_census-1.9.1/tests/experimental/pp/test_hvg.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/experimental/pp/test_online.py` & `cellxgene_census-1.9.1/tests/experimental/pp/test_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/experimental/pp/test_stats.py` & `cellxgene_census-1.9.1/tests/experimental/pp/test_stats.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/experimental/util/test_csr_iter.py` & `cellxgene_census-1.9.1/tests/experimental/util/test_csr_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/test_acceptance.py` & `cellxgene_census-1.9.1/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/test_directory.py` & `cellxgene_census-1.9.1/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/test_get_anndata.py` & `cellxgene_census-1.9.1/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/test_get_helpers.py` & `cellxgene_census-1.9.1/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/test_lts_compat.py` & `cellxgene_census-1.9.1/tests/test_lts_compat.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/test_open.py` & `cellxgene_census-1.9.1/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.9.0/tests/test_util.py` & `cellxgene_census-1.9.1/tests/test_util.py`

 * *Files identical despite different names*

