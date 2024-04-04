# Comparing `tmp/geniml-0.2.0.tar.gz` & `tmp/geniml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geniml-0.2.0.tar", last modified: Wed Feb 28 21:46:12 2024, max compression
+gzip compressed data, was "geniml-0.3.0.tar", last modified: Thu Apr  4 16:14:45 2024, max compression
```

## Comparing `geniml-0.2.0.tar` & `geniml-0.3.0.tar`

### file list

```diff
@@ -1,157 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.101480 geniml-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-28 21:46:03.000000 geniml-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-28 21:46:03.000000 geniml-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-28 21:46:12.101480 geniml-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-28 21:46:03.000000 geniml-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.081480 geniml-0.2.0/geniml/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.085480 geniml-0.2.0/geniml/assess/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/assess/assess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/assess/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/assess/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/assess/intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12008 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/assess/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/assess/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.085480 geniml-0.2.0/geniml/atacformer/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/atacformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/atacformer/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/atacformer/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/atacformer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.085480 geniml-0.2.0/geniml/bbclient/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bbclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bbclient/bbclient.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3024 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bbclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bbclient/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bbclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.085480 geniml-0.2.0/geniml/bedshift/
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedshift/BedshiftYAMLHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedshift/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedshift/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    26025 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedshift/bedshift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.085480 geniml-0.2.0/geniml/bedspace/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedspace/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedspace/argparsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedspace/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/bedspace/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.089480 geniml-0.2.0/geniml/eval/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/ctt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/gdst.py
--rw-r--r--   0 runner    (1001) docker     (127)    18472 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/npt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/rct.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/eval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.089480 geniml-0.2.0/geniml/io/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/io/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19057 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/io/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.089480 geniml-0.2.0/geniml/likelihood/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/likelihood/build_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/likelihood/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.089480 geniml-0.2.0/geniml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/models/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.089480 geniml-0.2.0/geniml/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/nn/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.093480 geniml-0.2.0/geniml/region2vec/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/main_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/region2vec_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/region_shuffling.py
--rw-r--r--   0 runner    (1001) docker     (127)    19262 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/region2vec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.093480 geniml-0.2.0/geniml/scembed/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11317 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/scembed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.093480 geniml-0.2.0/geniml/search/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.093480 geniml-0.2.0/geniml/search/backends/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/search/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/search/backends/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/search/backends/dbbackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/search/backends/filebackend.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/search/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/search/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.093480 geniml-0.2.0/geniml/text2bednn/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/text2bednn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/text2bednn/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    19275 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/text2bednn/text2bednn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/text2bednn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.097480 geniml-0.2.0/geniml/tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/bedtools_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/hard_tokenization_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11905 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/split_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/tokenization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.097480 geniml-0.2.0/geniml/training/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/training/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/training/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.097480 geniml-0.2.0/geniml/universe/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/cc_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/ccf_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/custom_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/hmm_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/ml_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/universe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-28 21:46:03.000000 geniml-0.2.0/geniml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.101480 geniml-0.2.0/geniml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-28 21:46:12.000000 geniml-0.2.0/geniml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-02-28 21:46:12.000000 geniml-0.2.0/geniml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 21:46:12.000000 geniml-0.2.0/geniml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-28 21:46:12.000000 geniml-0.2.0/geniml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-28 21:46:12.000000 geniml-0.2.0/geniml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-28 21:46:12.000000 geniml-0.2.0/geniml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-28 21:46:03.000000 geniml-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.101480 geniml-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-28 21:46:03.000000 geniml-0.2.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-28 21:46:03.000000 geniml-0.2.0/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-28 21:46:03.000000 geniml-0.2.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-28 21:46:03.000000 geniml-0.2.0/requirements/requirements-train.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 21:46:12.101480 geniml-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-02-28 21:46:03.000000 geniml-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:12.101480 geniml-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_atacformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_batch_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_bbclient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_bedshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_region2vec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_scembed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_text2bednn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-28 21:46:03.000000 geniml-0.2.0/tests/test_tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.530187 geniml-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-04 16:14:37.000000 geniml-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 16:14:37.000000 geniml-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 16:14:45.530187 geniml-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 16:14:37.000000 geniml-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.506187 geniml-0.3.0/geniml/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.506187 geniml-0.3.0/geniml/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/assess/assess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/assess/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/assess/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/assess/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/assess/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/assess/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.510187 geniml-0.3.0/geniml/atacformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/atacformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/atacformer/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/atacformer/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/atacformer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.510187 geniml-0.3.0/geniml/bbclient/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bbclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14305 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bbclient/bbclient.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3024 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bbclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bbclient/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bbclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.510187 geniml-0.3.0/geniml/bedshift/
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedshift/BedshiftYAMLHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedshift/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedshift/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25998 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedshift/bedshift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.510187 geniml-0.3.0/geniml/bedspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedspace/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedspace/argparsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedspace/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/bedspace/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.514187 geniml-0.3.0/geniml/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/ctt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/gdst.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/npt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/rct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/eval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.514187 geniml-0.3.0/geniml/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/io/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20333 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.514187 geniml-0.3.0/geniml/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/likelihood/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/likelihood/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.514187 geniml-0.3.0/geniml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/models/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.514187 geniml-0.3.0/geniml/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/nn/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.518187 geniml-0.3.0/geniml/region2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/main_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/region2vec_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/region_shuffling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/region2vec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.518187 geniml-0.3.0/geniml/scembed/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11290 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/scembed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.522187 geniml-0.3.0/geniml/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.522187 geniml-0.3.0/geniml/search/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/backends/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/backends/dbbackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/backends/filebackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/filebackend_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.522187 geniml-0.3.0/geniml/search/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/interfaces/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/interfaces/bed2bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/interfaces/text2bed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.522187 geniml-0.3.0/geniml/search/query2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/query2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/query2vec/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/query2vec/bed2vec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/query2vec/text2vec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.522187 geniml-0.3.0/geniml/text2bednn/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.522187 geniml-0.3.0/geniml/text2bednn/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/embedder/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/embedder/fastembedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/embedder/sentembedder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16187 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/text2bednn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/text2bednn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.526187 geniml-0.3.0/geniml/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/bedtools_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/hard_tokenization_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/split_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/tokenization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.526187 geniml-0.3.0/geniml/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/training/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/training/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.526187 geniml-0.3.0/geniml/universe/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/cc_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/ccf_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/custom_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/hmm_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/ml_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/universe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-04 16:14:37.000000 geniml-0.3.0/geniml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.530187 geniml-0.3.0/geniml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 16:14:45.000000 geniml-0.3.0/geniml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-04 16:14:45.000000 geniml-0.3.0/geniml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:14:45.000000 geniml-0.3.0/geniml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 16:14:45.000000 geniml-0.3.0/geniml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 16:14:45.000000 geniml-0.3.0/geniml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 16:14:45.000000 geniml-0.3.0/geniml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-04 16:14:37.000000 geniml-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.526187 geniml-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 16:14:37.000000 geniml-0.3.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-04 16:14:37.000000 geniml-0.3.0/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 16:14:37.000000 geniml-0.3.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 16:14:37.000000 geniml-0.3.0/requirements/requirements-train.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:14:45.530187 geniml-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2213 2024-04-04 16:14:37.000000 geniml-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:45.530187 geniml-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_atacformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_batch_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_bbclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_bedshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_region2vec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_scembed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_text2bednn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-04 16:14:37.000000 geniml-0.3.0/tests/test_tokenization.py
```

### Comparing `geniml-0.2.0/LICENSE.txt` & `geniml-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/assess/assess.py` & `geniml-0.3.0/geniml/assess/assess.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     df = pd.read_csv(file, index_col=(0))
     if flexible:
         df["f_t_u"] = df["median_dist_file_to_universe_flex"]
         df["u_t_f"] = df["median_dist_universe_to_file_flex"]
     else:
         df["f_t_u"] = df["median_dist_file_to_universe"]
         df["u_t_f"] = df["median_dist_universe_to_file"]
-    df["RBS"] = get_rbs(df["f_t_u"], df["u_t_t"])
+    df["RBS"] = get_rbs(df["f_t_u"], df["u_t_f"])
     if cs_each_file:
         return df
     else:
         return df["RBS"].mean()
 
 
 def get_f_10_score(
@@ -243,16 +243,16 @@
 def get_f_10_score_from_assessment_file(file, f10_each_file=False):
     """
     Get F10 score from assessment output file
     :param str file: path to file with assessment results
     :param bool f10_each_file: if report F10 for each file, not average for the collection
     """
     df = pd.read_csv(file, index_col=(0))
-    r = df["A&U/A"]
-    p = df["A&U/U"]
+    r = df["universe&file"] / (df["universe&file"] + df["file/universe"])
+    p = df["universe&file"] / (df["universe&file"] + df["univers/file"])
     df["F_10"] = (1 + 10**2) * (p * r) / ((10**2 * p) + r)
     if f10_each_file:
         return df["F_10"]
     else:
         return df["F_10"].mean()
```

### Comparing `geniml-0.2.0/geniml/assess/cli.py` & `geniml-0.3.0/geniml/assess/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/assess/distance.py` & `geniml-0.3.0/geniml/assess/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ..utils import natural_chr_sort
 from .utils import check_if_uni_flexible, check_if_uni_sorted, prep_data, process_db_line
 
 
 def flexible_distance_between_two_regions(region, query):
     """Calculate distance between region and flexible region from flexible universe
     :param [int, int] region: region from flexible universe
-    :param int query: analysed region
+    :param int query: analyzed region
     :return int: distance
     """
     if region[0] <= query <= region[1]:
         return 0
     else:
         return min(abs(region[0] - query), abs(region[1] - query))
 
@@ -36,16 +36,16 @@
 def distance_to_closest_region(
     db, db_queue, i, current_chrom, unused_db, pos_index, flexible, uni_to_file
 ):
     """
     Calculate distance from given peak to the closest region in database
     :param file db: database file
     :param list db_queue: queue of three last positions in database
-    :param i: analysed position from the query
-    :param str current_chrom: current analysed chromosome from query
+    :param i: analyzed position from the query
+    :param str current_chrom: current analyzed chromosome from query
     :param list unused_db: list of positions from universe that were not compared to query
     :param list pos_index: which indexes from universe region use to calculate distance
     :param bool flexible: whether the universe if flexible
     :param bool uni_to_file: whether calculate distance from universe to file
     :return int: peak distance to universe
     """
     if flexible:
@@ -86,15 +86,15 @@
     waiting,
     pos_index,
 ):
     """
     Read in new universe regions closest to the peak
     :param file db: universe file
     :param str q_chrom: new peak's chromosome
-    :param str current_chrom: chromosome that was analysed so far
+    :param str current_chrom: chromosome that was analyzed so far
     :param list unused_db: list of positions from universe that were not compared to query
     :param list db_queue: que of three last positions in universe
     :param bool waiting: whether iterating through file, without calculating
      distance,  if present chromosome not present in universe
     :param list pos_index: which indexes from universe region use to calculate distance
     :return bool, str: if iterating through chromosome not present in universe; current chromosome in query
     """
```

### Comparing `geniml-0.2.0/geniml/assess/intersection.py` & `geniml-0.3.0/geniml/assess/intersection.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,18 @@
     :param list region_d: region from universe
     :param list region_q: region from query
     :param int only_in_d: number of base pair only in universe
     :param int only_in_q: number of base pair only in query
     :param bool inside_d: whether there is still part of the region from universe to analyse
     :param bool inside_q: whether there is still part of the region from query to analyse
     :param int overlap: size of overlap
-    :param int start_d: start position of currently analysed universe region
-    :param int start_q: start position of currently analysed query region
-    :param bool waiting_d: whether waiting for the query to finish chrom
-    :param bool waiting_q: whether waiting for the universe to finish chrom
+    :param int start_d: start position of currently analyzed universe region
+    :param int start_q: start position of currently analyzed query region
+    :param bool waiting_d: whether waiting for the query to finish chromosome
+    :param bool waiting_q: whether waiting for the universe to finish chromosome
     """
     if waiting_q:
         only_in_d += region_d[1] - region_d[0]
         start_d = region_d[1]
         inside_d, inside_q = False, True
     elif waiting_d:
         only_in_q += region_q[1] - region_q[0]
```

### Comparing `geniml-0.2.0/geniml/assess/likelihood.py` & `geniml-0.3.0/geniml/assess/likelihood.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     :param str  universe: path to universe file
     :param list chroms: list of chromosomes present in model
     :param ModelLH model_lh: likelihood model
     :param coverage_prefix: prefix used in uniwig for creating coverage
     :param coverage_folder: path to a folder with genome coverage by tracks
     :param str name: suffix of model file name, which contains information
      about model type
-    :param int s_index: from which position in univers line take assess region
+    :param int s_index: from which position in universe line take assess region
      start position
-    :param int e_index: from which position in univers line take assess region
+    :param int e_index: from which position in universe line take assess region
      end position
-    :return float: likelihood of univers for given model
+    :return float: likelihood of universe for given model
     """
     current_chrom = ""
     missing_chrom = ""
     empty_start = 0
     res = 0
     e = 0
     done_chrom = []
@@ -174,17 +174,17 @@
 
 
 def weigh_livelihood(start, end, model_process, model_cove, model_out, reverse):
     """
     Calculate weighted likelihood of flexible part of the region
     :param int start: start of the region
     :param int end: end of the region
-    :param array model_process: model for analysed type of flexible region
+    :param array model_process: model for analyzed type of flexible region
     :param array model_cove: model for coverage
-    :param array model_out: model for flexible region that is not being analysed
+    :param array model_out: model for flexible region that is not being analyzed
     :param bool reverse: if model_process corespondents to end we have to reverse the weighs
     :return float: likelihood of flexible part of the region
     """
     e_w = 1 / (end - start)  # weights for processed model
     c_w = np.linspace(start=e_w, stop=1, num=(end - start))  # weights for core in processed region
     if reverse:
         c_w = c_w[::-1]
```

### Comparing `geniml-0.2.0/geniml/assess/utils.py` & `geniml-0.3.0/geniml/assess/utils.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/atacformer/const.py` & `geniml-0.3.0/geniml/atacformer/const.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/atacformer/main.py` & `geniml-0.3.0/geniml/atacformer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import os
-from typing import Union, List
+from typing import List, Union
 
 import torch
 import torch.nn as nn
 from huggingface_hub import hf_hub_download
 from yaml import safe_dump, safe_load
 
 from ..models.main import ExModel
 from ..tokenization.main import ITTokenizer
 from .const import (
-    POOLING_TYPES,
-    POOLING_METHOD_KEY,
+    CONFIG_FILE_NAME,
     D_MODEL_KEY,
-    VOCAB_SIZE_KEY,
-    NUM_LAYERS_KEY,
-    NHEAD_KEY,
     DEFAULT_EMBEDDING_DIM,
-    CONFIG_FILE_NAME,
     MODEL_FILE_NAME,
+    NHEAD_KEY,
+    NUM_LAYERS_KEY,
+    POOLING_METHOD_KEY,
+    POOLING_TYPES,
     UNIVERSE_FILE_NAME,
+    VOCAB_SIZE_KEY,
 )
 
 
 class Atacformer(nn.Module):
     def __init__(
         self,
         vocab_size: int,
```

### Comparing `geniml-0.2.0/geniml/atacformer/utils.py` & `geniml-0.3.0/geniml/atacformer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 from glob import glob
 from math import ceil
+from typing import List, Tuple
 
 import torch
-from torch.utils.data import Dataset
-from torch.nn.utils.rnn import pad_sequence
 from genimtools.utils import read_tokens_from_gtok
+from torch.nn.utils.rnn import pad_sequence
+from torch.utils.data import Dataset
 
-from .const import MASK_RATE, REPLACE_WITH_MASK_RATE, REPLACE_WITH_RANDOM_RATE, KEEP_RATE
+from .const import KEEP_RATE, MASK_RATE, REPLACE_WITH_MASK_RATE, REPLACE_WITH_RANDOM_RATE
 
 
 class AtacformerMLMDataset(Dataset):
     def __init__(
         self,
         data: str,
         mask_token_id: int,
@@ -40,15 +41,15 @@
 
         # get list of all files
         self.files = glob(os.path.join(data, "*.gtok"))
 
     def __len__(self):
         return len(self.files)
 
-    def __getitem__(self, idx) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    def __getitem__(self, idx) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         This should return a tuple of (tokens, masked_tokens, mask_ids).
         """
         # load the data
         tokens = torch.tensor(read_tokens_from_gtok(self.files[idx]))
         masked_tokens = tokens.clone()
 
@@ -68,16 +69,16 @@
                 masked_tokens[i] = torch.randint(self.vocab_size, (1,))
             else:
                 pass  # do nothing, keep the original token
 
         return tokens, masked_tokens, mask_ids
 
     def collate_batch(
-        batch: list[tuple[torch.Tensor, torch.Tensor, torch.Tensor]], padding_token: int
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
+        self, batch: List[Tuple[torch.Tensor, torch.Tensor, torch.Tensor]], padding_token: int
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         Collate function for the MLM dataset. This should take a batch of
         (tokens, masked_tokens, mask_ids) and return a tuple of (tokens, masked_tokens, mask_ids) that are padded
 
         :param list[tuple[torch.Tensor, torch.Tensor, torch.Tensor]] batch: Batch of (tokens, masked_tokens, mask_ids)
         :param int padding_token: Token to use for padding
         """
```

### Comparing `geniml-0.2.0/geniml/bbclient/bbclient.py` & `geniml-0.3.0/geniml/bbclient/bbclient.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 import gzip
 import os
 import shutil
 from logging import getLogger
 from typing import List, NoReturn, Union
 
+import boto3
 import requests
+from botocore.exceptions import ClientError
 from ubiquerg import is_url
 
 from .._version import __version__
 from ..io.io import BedSet, RegionSet
 from ..io.utils import is_gzipped
 from .const import (
     BEDFILE_URL_PATTERN,
     BEDSET_URL_PATTERN,
+    DEFAULT_BUCKET_NAME,
     DEFAULT_BEDBASE_API,
     DEFAULT_BEDFILE_EXT,
     DEFAULT_BEDFILE_SUBFOLDER,
     DEFAULT_BEDSET_EXT,
     DEFAULT_BEDSET_SUBFOLDER,
+    DEFAULT_BUCKET_FOLDER,
     DEFAULT_CACHE_FOLDER,
     MODULE_NAME,
 )
-from .utils import BedCacheManager, get_bbclient_path_folder
+from .utils import BedCacheManager, get_abs_path
 
 _LOGGER = getLogger(MODULE_NAME)
 
 
 class BBClient(BedCacheManager):
     def __init__(
         self,
-        cache_folder: str = DEFAULT_CACHE_FOLDER,
+        cache_folder: Union[str, os.PathLike] = DEFAULT_CACHE_FOLDER,
         bedbase_api: str = DEFAULT_BEDBASE_API,
     ):
         """
         BBClient to deal with download files from bedbase and caching them.
 
         :param cache_folder: path to local folder as cache of files from bedbase,
         if not given it will be the environment variable `BBCLIENT_CACHE`
         :param bedbase_api: url to bedbase
         """
-        # get default cache folder from environment variable set by user
-        super().__init__(get_bbclient_path_folder(cache_folder))
+        cache_folder = get_abs_path(cache_folder)
+        super().__init__(cache_folder)
+
         self.bedbase_api = bedbase_api
 
     def load_bedset(self, bedset_id: str) -> BedSet:
         """
-        Loads a BED set from cache, or downloads and caches it plus BED files in it if it doesn't exist
+        Load a BEDset from cache, or download and add it to the cache with its BED files
 
-        :param bedset_id: unique identifier of BED set
+        :param BedSet: BedSet object
         """
 
         file_path = self._bedset_path(bedset_id)
 
         if os.path.exists(file_path):
             _LOGGER.info(f"BED set {bedset_id} already exists in cache.")
             with open(file_path, "r") as file:
-                extracted_data = file.readlines()
+                extracted_data = file.read().splitlines()
         else:
             extracted_data = self._download_bedset_data(bedset_id)
             # write the identifiers of BED files in the BedSet to a local .txt file
             with open(file_path, "w") as file:
                 for value in extracted_data:
                     file.write(value + "\n")
             _LOGGER.info(f"BED set {bedset_id} downloaded and cached successfully.")
@@ -75,24 +80,25 @@
         Download BED set from BEDbase API and return the list of identifiers of BED files in the set
 
         :param bedset_id: unique identifier of a BED set
         :return: the list of identifiers of BED files in the set
         """
         bedset_url = BEDSET_URL_PATTERN.format(bedbase_api=self.bedbase_api, bedset_id=bedset_id)
         response = requests.get(bedset_url)
-        data = response.json()
-        extracted_data = [entry.get("record_identifier") for entry in data["bedfile_metadata"]]
+        data = response.json()["results"]
+        extracted_data = [entry.get("id") for entry in data]
 
         return extracted_data
 
     def load_bed(self, bed_id: str) -> RegionSet:
         """
         Loads a BED file from cache, or downloads and caches it if it doesn't exist
 
         :param bed_id: unique identifier of a BED file
+        :return: the RegionSet object
         """
         file_path = self._bedfile_path(bed_id)
 
         if os.path.exists(file_path):
             _LOGGER.info(f"BED file {bed_id} already exists in cache.")
         else:
             file_path = self._bedfile_path(bed_id)
@@ -126,16 +132,16 @@
                     file.write(bedfile_id + "\n")
         return bedset_id
 
     def add_bed_to_cache(self, bedfile: Union[RegionSet, str]) -> str:
         """
         Add a BED file to the cache
 
-        :param bedfile: a RegionSet class or a path to a BED file to be added to cache
-        :return: the identifier if the BedFile object
+        :param bedfile: a RegionSet object or a path or url to the BED file
+        :return: the RegionSet identifier
         """
         if isinstance(bedfile, str):
             bedfile = RegionSet(bedfile)
         elif not isinstance(bedfile, RegionSet):
             raise TypeError(
                 f"Input must be a RegionSet or a path to a BED file, not {type(bedfile)}"
             )
@@ -159,20 +165,104 @@
                     # https://docs.python.org/3/library/gzip.html
                     with open(bedfile.path, "rb") as f_in:
                         with gzip.open(file_path, "wb") as f_out:
                             shutil.copyfileobj(f_in, f_out)
 
         return bedfile_id
 
+    def add_bed_to_s3(
+        self,
+        identifier: str,
+        bucket: str = DEFAULT_BUCKET_NAME,
+        endpoint_url: str = None,
+        aws_access_key_id: str = None,
+        aws_secret_access_key: str = None,
+        s3_path: str = DEFAULT_BUCKET_FOLDER,
+    ) -> str:
+        """
+        Add a cached BED file to S3
+
+        :param identifier: the unique identifier of the BED file
+        :param bucket: the name of the bucket
+        :param endpoint_url: the URL of the S3 endpoint [Default: set up by the environment vars]
+        :param aws_access_key_id: the access key of the AWS account [Default: set up by the environment vars]
+        :param aws_secret_access_key: the secret access key of the AWS account [Default: set up by the environment vars]
+        :param s3_path: the path on S3
+
+        :return: full path on S3
+        """
+        s3_client = boto3.client(
+            "s3",
+            endpoint_url=endpoint_url,
+            aws_access_key_id=aws_access_key_id,
+            aws_secret_access_key=aws_secret_access_key,
+        )
+        local_file_path = self.seek(identifier)
+        bed_file_name = os.path.basename(local_file_path)
+        s3_bed_path = os.path.join(identifier[0], identifier[1], bed_file_name)
+        if s3_path:
+            s3_bed_path = os.path.join(s3_path, s3_bed_path)
+
+        s3_client.upload_file(local_file_path, bucket, s3_bed_path)
+        _LOGGER.info(f"Project was uploaded successfully to s3://{bucket}/{s3_bed_path}")
+        return s3_bed_path
+
+    def get_bed_from_s3(
+        self,
+        identifier: str,
+        bucket: str = DEFAULT_BUCKET_NAME,
+        endpoint_url: str = None,
+        aws_access_key_id: str = None,
+        aws_secret_access_key: str = None,
+        s3_path: str = DEFAULT_BUCKET_FOLDER,
+    ) -> str:
+        """
+        Get a cached BED file from S3 and cache it locally
+
+        :param identifier: the unique identifier of the BED file
+        :param bucket: the name of the bucket
+        :param endpoint_url: the URL of the S3 endpoint [Default: set up by the environment vars]
+        :param aws_access_key_id: the access key of the AWS account [Default: set up by the environment vars]
+        :param aws_secret_access_key: the secret access key of the AWS account [Default: set up by the environment vars]
+        :param s3_path: the path on S3
+
+        :return: bed file id
+        :raise FileNotFoundError: if the identifier does not exist in cache
+        """
+        s3_bed_path = os.path.join(
+            identifier[0], identifier[1], f"{identifier}{DEFAULT_BEDFILE_EXT}"
+        )
+        if s3_path:
+            s3_bed_path = os.path.join(s3_path, s3_bed_path)
+
+        s3_client = boto3.client(
+            "s3",
+            endpoint_url=endpoint_url,
+            aws_access_key_id=aws_access_key_id,
+            aws_secret_access_key=aws_secret_access_key,
+        )
+        try:
+            s3_client.download_file(
+                bucket, s3_bed_path, self._bedfile_path(identifier, create=True)
+            )
+        except ClientError as e:
+            if e.response["Error"]["Code"] == "404":
+                raise FileNotFoundError(f"{identifier} does not exist in S3.")
+            else:
+                raise e
+
+        return identifier
+
     def seek(self, identifier: str) -> str:
         """
         Get local path to BED file or BED set with specific identifier
 
         :param identifier: the unique identifier
         :return: the local path of the file
+        :raise FileNotFoundError: if the identifier does not exist in cache
         """
 
         # check if any BED set has that identifier
         file_path = self._bedset_path(identifier, False)
         if os.path.exists(file_path):
             return file_path
         else:
```

### Comparing `geniml-0.2.0/geniml/bbclient/cli.py` & `geniml-0.3.0/geniml/bbclient/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/bbclient/utils.py` & `geniml-0.3.0/geniml/bbclient/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import gzip
 import os
 from io import BytesIO
+from pathlib import Path
 from typing import Optional
 
 import genomicranges
 import pandas as pd
 
 from .const import DEFAULT_CACHE_FOLDER
 
 
 class BedCacheManager:
     def __init__(self, cache_folder: str):
         self.cache_folder = cache_folder
         self.create_cache_folder()
 
     def create_cache_folder(self, subfolder_path: Optional[str] = None) -> None:
-        """Create cache folder if it doesn't exist"""
+        """
+        Create cache folder if it doesn't exist
+
+        :param subfolder_path: path to the subfolder
+        """
         if subfolder_path is None:
             subfolder_path = self.cache_folder
 
         full_path = os.path.abspath(subfolder_path)
         if not os.path.exists(full_path):
             os.makedirs(full_path)
 
@@ -58,12 +63,20 @@
         ]
         df.columns = header[: len(df.columns)]
         gr = genomicranges.from_pandas(df)
 
         return gr
 
 
-def get_bbclient_path_folder(path: str = DEFAULT_CACHE_FOLDER):
+def get_abs_path(path: str = DEFAULT_CACHE_FOLDER, create_folder: bool = True) -> str:
     """
-    Get the cache folder path either from input or environment variable '$BBCLIENT_CACHE'
+    Get absolute path to the folder and create it if it doesn't exist
+
+    :param path: path to the folder
+    :param create_folder: create folder if it doesn't exist
+
+    :return: absolute path to the folder
     """
-    return os.path.expandvars(path)
+    absolute_cache_folder = os.path.expandvars(path)
+    if create_folder:
+        Path(absolute_cache_folder).mkdir(parents=True, exist_ok=True)
+    return absolute_cache_folder
```

### Comparing `geniml-0.2.0/geniml/bedshift/BedshiftYAMLHandler.py` & `geniml-0.3.0/geniml/bedshift/BedshiftYAMLHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import logging
 import os
 import sys
+
 import yaml
-import logging
 
 
 class BedshiftYAMLHandler(object):
     def __init__(self, bedshifter, yaml_fp, logger=None):
         """
         Handles Bedshift perturbations from yaml files
```

### Comparing `geniml-0.2.0/geniml/bedshift/arguments.py` & `geniml-0.3.0/geniml/bedshift/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+
 from geniml.bedshift._version import __version__
 
 
 class _VersionInHelpParser(argparse.ArgumentParser):
     def format_help(self):
         """Add version information to help text."""
         return (
```

### Comparing `geniml-0.2.0/geniml/bedshift/bedshift.py` & `geniml-0.3.0/geniml/bedshift/bedshift.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """ Perturb regions in bedfiles """
 
 import logging
-import logmuse
 import math
-import numpy as np
 import os
-import pandas as pd
 import random
 import sys
 
-from geniml.bedshift._version import __version__
-from geniml.bedshift import arguments
-from geniml.bedshift import BedshiftYAMLHandler
-
+import logmuse
+import numpy as np
+import pandas as pd
 from genimtools.ailist import AIList, Interval
 
+from geniml.bedshift import BedshiftYAMLHandler, arguments
+from geniml.bedshift._version import __version__
+
 _LOGGER = logging.getLogger(__name__)
 
 __all__ = ["Bedshift"]
 
 
 class Bedshift(object):
     """
```

### Comparing `geniml-0.2.0/geniml/bedspace/argparsers.py` & `geniml-0.3.0/geniml/bedspace/argparsers.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/bedspace/cli.py` & `geniml-0.3.0/geniml/bedspace/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/cli.py` & `geniml-0.3.0/geniml/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/eval/cli.py` & `geniml-0.3.0/geniml/eval/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 def build_subparser(parser):
     """
     Builds argument parser to support the eval command line interface.
     """
     sp = parser.add_subparsers(dest="subcommand")
     msg_by_cmd = {
         "gdst": "Genome distance scaling test",
-        "npt": "Neighorhood preserving test",
+        "npt": "Neighborhood preserving test",
         "ctt": "Cluster tendency test",
         "rct": "Reconstruction test",
         "bin-gen": "Generate binary embeddings",
     }
     subparsers = {}
     for k, v in msg_by_cmd.items():
         subparsers[k] = sp.add_parser(k, description=v, help=v)
```

### Comparing `geniml-0.2.0/geniml/eval/ctt.py` & `geniml-0.3.0/geniml/eval/ctt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 import os
 import pickle
 
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
-import argparse
-import glob
-import multiprocessing as mp
-import random
-import time
 
+from typing import Tuple, List
 import numpy as np
-import pandas as pd
-from sklearn.decomposition import PCA
 from sklearn.neighbors import NearestNeighbors
 
-from .const import *
-from .utils import cosine_distance, genome_distance, load_genomic_embeddings
+from .const import CTT_QUANTILE_MAX, CTT_QUANTILE_MIN, CTT_TEST_RATIO
+from .utils import load_genomic_embeddings
 
 
 def get_ctt_score(
     path: str,
     embed_type: str,
     seed: int = 42,
     num_data: int = 10000,
@@ -74,55 +68,55 @@
     if x + y == 0:
         raise ZeroDivisionError("The denominator is zero")
 
     return y / (x + y)
 
 
 def get_ctt_batch(
-    batch: list[tuple[str, str]],
+    batch: List[Tuple[str, str]],
     seed: int = 42,
     num_data: int = 10000,
     save_path: str = None,
     num_workers: int = 10,
-) -> list[tuple[str, float]]:
+) -> List[Tuple[str, float]]:
     """Runs the cluster tendency test (CTT) on a batch of models.
 
     Args:
         batch (list[tuple[str, str]]): A list of (model path, model type)
             tuples. Model type could be "region2vec" or "base".
         seed (int, optional): Random seed. Defaults to 42.
         num_data (int, optional): Number of embeddings used for evaluation.
             Defaults to 10000.
         save_path (str, optional): Save the results to save_path. Defaults to
             None.
         num_workers (int, optional): Number of parallel processes used.
             Defaults to 10.
 
     Returns:
-        list[tuple[str, float]]: A list of (model path, CTT score) tuples.
+        List[Tuple[str, float]]: A list of (model path, CTT score) tuples.
     """
     ctt_arr = []
     for path, embed_type in batch:
         ctt = get_ctt_score(path, embed_type, seed, num_data, num_workers)
         # print(f"{'/'.join(path.split('/')[-3:])}: {ctt:.4f}")
         ctt_arr.append((path, ctt))
     if save_path:
         os.makedirs(os.path.dirname(save_path), exist_ok=True)
         with open(save_path, "wb") as f:
             pickle.dump(ctt_arr, f)
     return ctt_arr
 
 
 def ctt_eval(
-    batch: list[tuple[str, str]],
+    batch: List[Tuple[str, str]],
     num_runs: int = 20,
     num_data: int = 10000,
     save_folder: str = None,
     num_workers: int = 10,
-) -> list[tuple[str, list[float]]]:
+) -> List[Tuple[str, list[float]]]:
     """Runs the CTT on a batch of models for multiple times.
 
     Runs the cluster tendency test (CTT) for a batch of models for num_runs
     times with different random seeds.
 
 
     Args:
@@ -151,12 +145,12 @@
     for results in results_seeds:
         for i, res in enumerate(results):
             ctt_res[i].append(res[1])
             assert res[0] == batch[i][0], "key == batch[i][0]"
 
     mean_ctt = [np.array(r).mean() for r in ctt_res]
     std_ctt = [np.array(r).std() for r in ctt_res]
-    models = [t[0] for t in batch]
+    # models = [t[0] for t in batch]
     for i in range(len(mean_ctt)):
         print(f"{batch[i][0]}\n CTT (std): {mean_ctt[i]:.4f} ({std_ctt[i]:.4f}) \n")
     ctt_arr = [(batch[i][0], ctt_res[i]) for i in range(len(batch))]
     return ctt_arr
```

### Comparing `geniml-0.2.0/geniml/eval/gdst.py` & `geniml-0.3.0/geniml/eval/gdst.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import os
+from typing import List, Tuple
 import pickle
 from typing import Union
 
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
-import argparse
-import glob
 import multiprocessing as mp
-import random
-import time
 from multiprocessing.queues import Queue
 
 import numpy as np
-from gensim.models import Word2Vec
 from sklearn.linear_model import LinearRegression
 
-from .const import *
+from .const import GENOME_DIST_SCALAR
 from .utils import cosine_distance, genome_distance, load_genomic_embeddings
 
 
-def sample_from_vocab(vocab: list[str], num_samples: int, seed: int = 42) -> list[str]:
+def sample_from_vocab(vocab: List[str], num_samples: int, seed: int = 42) -> List[str]:
     """Samples regions from vocab.
 
     Samples regions proportionally from each chromosome.
 
     Args:
         vocab (list[str]): A list of regions.
         num_samples (int): Number of regions to sample.
@@ -77,15 +73,15 @@
 def get_gdst_score(
     path: str,
     embed_type: str,
     num_samples: int = 10000,
     seed: int = 42,
     queue: Queue = None,
     worker_id: int = None,
-) -> Union[float, tuple[int, str, float]]:
+) -> Union[float, Tuple[int, str, float]]:
     """Runs the GDST on a model.
 
     Args:
         path (str): The path to a model.
         embed_type (str): The model type: "region2vec" or "base".
         num_samples (int, optional): Number of embeddings used for evaluation.
             Defaults to 10000.
@@ -117,15 +113,15 @@
     if queue:
         queue.put((worker_id, path, slope))
         return worker_id, path, slope
     else:
         return slope
 
 
-def writer_multiprocessing(save_path: str, num: int, q: Queue) -> list[tuple[str, float]]:
+def writer_multiprocessing(save_path: str, num: int, q: Queue) -> List[Tuple[str, float]]:
     """Writes results from multiple processes to a list.
 
     Args:
         save_path (str): The path to the saved results.
         num (int): The number of results.
         q (Queue): A multiprocessing queue.
 
@@ -143,20 +139,20 @@
             os.makedirs(os.path.dirname(save_path), exist_ok=True)
             with open(save_path, "wb") as f:
                 pickle.dump(results, f)
     return results
 
 
 def get_gdst_score_batch(
-    batch: list[tuple[str, str]],
+    batch: List[Tuple[str, str]],
     num_samples: int = 10000,
     seed: int = 42,
     save_path: str = None,
     num_workers: int = 1,
-) -> list[tuple[str, float]]:
+) -> List[Tuple[str, float]]:
     """Runs the GDST on a batch of models.
 
     Args:
         batch (list[tuple[str, str]]): A list of (model path, model type) tuples.
         num_samples (int, optional): Number of embeddings used for evaluation.
             Defaults to 10000.
         seed (int, optional): Random seed. Defaults to 42.
@@ -195,20 +191,20 @@
                 process.get()
             queue.put("kill")
             gds_arr = writer.get()
     return gds_arr
 
 
 def gdst_eval(
-    batch: list[tuple[str, str]],
+    batch: List[Tuple[str, str]],
     num_runs: int = 20,
     num_samples: int = 1000,
     save_folder: str = None,
     num_workers: int = 10,
-) -> list[tuple[str, list[float]]]:
+) -> List[Tuple[str, List[float]]]:
     """Runs the GDST on a batch of models for multiple times.
 
     Args:
         batch (list[tuple[str, str]]): A list of (model path, model type) tuples.
         num_runs (int, optional): Number of runs. Defaults to 20.
         num_samples (int, optional): Number of embeddings used for evaluation.
             Defaults to 1000.
```

### Comparing `geniml-0.2.0/geniml/eval/npt.py` & `geniml-0.3.0/geniml/eval/npt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 import os
-import pickle
-from typing import Union
 
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
-import argparse
+
+import pickle
+from typing import Union, List, Tuple, Dict
+
 import multiprocessing as mp
-import time
 from multiprocessing.queues import Queue
-
-import matplotlib.pyplot as plt
 import numpy as np
-from gensim.models import Word2Vec
-from matplotlib.lines import Line2D
 
 from .utils import genome_distance, load_genomic_embeddings
 
 
 def get_topk_embed(
     i: int, K: int, embed: np.ndarray, dist: str = "cosine"
-) -> tuple[np.ndarray, np.ndarray]:
+) -> Tuple[np.ndarray, np.ndarray]:
     """Gets the nearest K embedding indexes to the i-th embedding.
 
     Args:
         i (int): The index for the query embedding.
         K (int): The number of nearest embeddings to select.
         embed (np.ndarray): An array of embedding vectors
         dist (str, optional): The distance function used. Defaults to "cosine".
@@ -47,79 +43,79 @@
         denom = ((embed[i : i + 1] + embed) > 0.0).sum(axis=1)
         sims = (nom / denom)[0]
         indexes = np.argsort(-sims)[1 : K + 1]
         s = sims[indexes]
     return indexes, s
 
 
-def find_Kneighbors(region_array: list[tuple[str, int, int]], index: int, K: int) -> list[int]:
+def find_kneighbors(region_array: List[Tuple[str, int, int]], index: int, k: int) -> List[int]:
     """Finds the indexes of the K nearest regions of a query region on genome.
 
     region_array must be sorted, and all regions are on the same chromosome.
 
     Args:
         region_array (list[tuple[str, int, int]]): A list of (chromosome, start
             position, end position) tuples.
         index (int): The index of the query region.
-        K (int): Specifies the number of nearest neighbors of the query region.
+        k (int): Specifies the number of nearest neighbors of the query region.
 
     Returns:
         list[int]: A list of indexes of the K nearest neighbors in
             region_array.
     """
-    if len(region_array) < K:
-        K = len(region_array)
+    if len(region_array) < k:
+        k = len(region_array)
     qregion = region_array[index]
-    left_idx = max(index - K, 0)
-    right_idx = min(index + K, len(region_array) - 1)
+    left_idx = max(index - k, 0)
+    right_idx = min(index + k, len(region_array) - 1)
     rdist_arr = []
     for idx in range(left_idx, right_idx + 1):
         rdist_arr.append(genome_distance(qregion, region_array[idx]))
     rdist_arr = np.array(rdist_arr)
-    Kneighbors_idx = np.argsort(rdist_arr)[1 : K + 1]
+    Kneighbors_idx = np.argsort(rdist_arr)[1 : k + 1]
     Kneighbors_idx = Kneighbors_idx + left_idx
     return Kneighbors_idx
 
 
 def calculate_overlap_bins(
     local_idx: int,
     K: int,
     chromo: str,
-    region_array: list[tuple[str, int, int]],
+    region_array: List[Tuple[str, int, int]],
     region2index: dict[str, int],
     embed_rep: np.ndarray,
     res: int = 10,
     dist: str = "cosine",
     same_chromo: bool = True,
 ) -> np.ndarray:
     """Calculates the overlap ratios for a region.
 
-    Calculates the overlap ratios for a region between its K-nearest neighor
-    set obtained using genome distance and its K-nearest neighor set obtained
+    Calculates the overlap ratios for a region between its K-nearest neighbor
+    set obtained using genome distance and its K-nearest neighbor set obtained
     using embedding distance. If res < K, then calculates ratios for size
     res*1, res*2, ..., min(res*n, K).
 
     Args:
         local_idx (int): The local index of a region on its chromosome.
         K (int): Specifies the number of nearest neighbors.
         chromo (str): Chromosome.
         region_array (list[tuple[str, int, int]]): A list of (chromosome, start
             position, end position) tuples.
         region2index (dict[str, int]): A dictionary of (region, index).
         embed_rep (np.ndarray): An array of embedding vectors.
         res (int, optional): Resolution. Size of neighborhood set. Defaults to
             10.
         dist (str, optional): Distance function. Defaults to "cosine".
-        same_chromo (bool, optional): Whether to find nearest neighors on the
+        same_chromo (bool, optional): Whether to find nearest neighbors on the
             same chromosome in the embedding space. Defaults to True.
 
     Returns:
         np.ndarray: An array of overlap ratios.
     """
-    Kindices = find_Kneighbors(region_array, local_idx, K)
+    Kindices = find_kneighbors(region_array, local_idx, K)
     if len(Kindices) == 0:
         return 0
     str_kregions = [
         f"{chromo}:{region_array[k][0]}-{region_array[k][1]}" for k in Kindices
     ]  # sorted in ascending order
     _Krdist_global_indices = np.array([region2index[r] for r in str_kregions])
 
@@ -147,34 +143,29 @@
 
     return np.array(bin_overlaps)
 
 
 def cal_snpr(ratio_embed: np.ndarray, ratio_random: np.ndarray) -> np.ndarray:
     """Calculates SNPR values.
 
-    Args:
-        ratio_embed (np.ndarray): Overlap ratios for query embeddings.
-        ratio_random (np.ndarray): Overlap ratios for random embeddings.
+    :param ratio_embed: Overlap ratios for query embeddings.
+    :param ratio_random: Overlap ratios for random embeddings.
 
-    Returns:
-        np.ndarray: SNPR values.
+    :return: SNPR values.
     """
     res = np.log10((ratio_embed + 1.0e-10) / (ratio_random + 1.0e-10))
     res = np.maximum(res, 0)
     return res
 
 
-var_dict = {}
-
-
 def worker_func(
     i: int,
     K: int,
     chromo: str,
-    region_array: list[tuple[str, int, int]],
+    region_array: List[Tuple[str, int, int]],
     embed_type: str,
     resolution: int,
     dist: str,
 ) -> np.ndarray:
     """Wrapper for calculate_overlap_bins
 
     Args:
@@ -186,14 +177,16 @@
         embed_type (str): Embedding type, "region2vec" or "base".
         resolution (int): Resolution.
         dist (str): Distance function.
 
     Returns:
         np.ndarray: An array of overlap ratios.
     """
+    var_dict = {}
+
     if embed_type == "embed":
         embeds = var_dict["embed_rep"]
     elif embed_type == "random":
         embeds = var_dict["ref_embed"]
     nprs = calculate_overlap_bins(
         i,
         K,
@@ -204,39 +197,40 @@
         resolution,
         dist,
     )
     return nprs
 
 
 def init_worker(
-    embed_rep: np.ndarray, ref_embed: np.ndarray, region2index: dict[str, int]
+    embed_rep: np.ndarray, ref_embed: np.ndarray, region2index: Dict[str, int]
 ) -> None:
     """Initializes data used by workers.
 
     Args:
         embed_rep (np.ndarray): Query embeddings.
         ref_embed (np.ndarray): Random embeddings.
         region2index (dict[str, int]): A region to index dictionary.
     """
+    var_dict = {}
     var_dict["embed_rep"] = embed_rep
     var_dict["ref_embed"] = ref_embed
     var_dict["region2vec_index"] = region2index
 
 
 def get_npt_score(
     model_path: str,
     embed_type: str,
     K: int,
     num_samples: int = 100,
     seed: int = 0,
     resolution: int = 10,
     dist: str = "cosine",
     num_workers: int = 10,
-) -> dict[str, Union[int, np.ndarray, str]]:
-    """Runs the NPT on a mdoel.
+) -> Dict[str, Union[int, np.ndarray, str]]:
+    """Runs the NPT on a model.
 
     If num_samples > 0, then randomly sample num_samples regions proportional
     from each chromosome. If num_samples == 0, all regions are used in the
     test. If K > resolution, then returns an array of NPT scores; otherwise,
     returns one NPT score.
 
     Args:
@@ -382,15 +376,15 @@
         "SNPR": snprs,
         "Resolution": resolution,
         "Path": model_path,
     }
     return result
 
 
-def writer_multiprocessing(save_path: str, num: int, q: Queue) -> list[tuple[str, float]]:
+def writer_multiprocessing(save_path: str, num: int, q: Queue) -> List[Tuple[str, float]]:
     """Writes results from multiple processes to a list.
 
     Args:
         save_path (str): The path to the saved results.
         num (int): The number of results.
         q (Queue): A multiprocessing queue.
 
@@ -408,23 +402,23 @@
             os.makedirs(os.path.dirname(save_path), exist_ok=True)
             with open(save_path, "wb") as f:
                 pickle.dump(results, f)
     return results
 
 
 def get_npt_score_batch(
-    batch: list[tuple[str, str]],
+    batch: List[Tuple[str, str]],
     K: int,
     num_samples: int = 100,
     num_workers: int = 10,
     seed: int = 0,
     resolution: int = 10,
     dist: str = "cosine",
     save_path: str = None,
-) -> list[dict[str, Union[int, np.ndarray, str]]]:
+) -> List[Dict[str, Union[int, np.ndarray, str]]]:
     """Runs the NPT on a batch of models.
 
     Args:
         batch (list[tuple[str, str]]): A list of (model path, model type) tuples.
         K (int): Specifies the number of nearest neighbors.
         num_samples (int, optional): Number of embeddings used for evaluation.
             Defaults to 100.
@@ -458,23 +452,23 @@
         os.makedirs(os.path.dirname(save_path), exist_ok=True)
         with open(save_path, "wb") as f:
             pickle.dump(result_list, f)
     return result_list
 
 
 def npt_eval(
-    batch: list[tuple[str, str]],
+    batch: List[Tuple[str, str]],
     K: int,
     num_samples: int = 100,
     num_workers: int = 10,
     num_runs: int = 20,
     resolution: int = 10,
     dist: str = "cosine",
     save_folder: str = None,
-) -> list[tuple[str, np.ndarray, int]]:
+) -> List[Tuple[str, np.ndarray, int]]:
     """Runs the NPT on a batch of models for multiple times.
 
     Args:
         batch (list[tuple[str, str]]): A list of (model path, model type) tuples.
         K (int): Specifies the number of nearest neighbors.
         num_samples (int, optional): Number of embeddings used for evaluation.
             Defaults to 100.
@@ -485,15 +479,15 @@
             Defaults to 10.
         dist (str, optional): Distance function. Defaults to "cosine".
         save_folder (str, optional): Folder to save the results from each run.
             Defaults to None.
 
     Returns:
         list[tuple[str, np.ndarray, int]]: A list of (model path, snprs from
-            num_runs, resoultion) tuples.
+            num_runs, resolution) tuples.
     """
     results_seeds = []
     assert resolution <= K, "resolution <= K"
     for seed in range(num_runs):
         print(f"----------------Run {seed}----------------")
         save_path = os.path.join(save_folder, f"npt_eval_seed{seed}") if save_folder else None
         result_list = get_npt_score_batch(
```

### Comparing `geniml-0.2.0/geniml/eval/rct.py` & `geniml-0.3.0/geniml/eval/rct.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/eval/utils.py` & `geniml-0.3.0/geniml/eval/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-import argparse
-import glob
-import multiprocessing as mp
-import os
 import pickle
-import time
-from typing import Union
+from typing import Union, List, Tuple, Dict
 
 import numpy as np
 from gensim.models import Word2Vec
 
 
-def genome_distance(u: tuple[int, int], v: tuple[int, int]) -> float:
+def genome_distance(u: Tuple[int, int], v: Tuple[int, int]) -> float:
     """Computes the genome distance between two regions.
 
     Assumes that the two regions, u and v, are on the same chromosome.
 
     Args:
         u (tuple[int, int]): A region denoted by its start and end positions.
         v (tuple[int, int]): A region denoted by its start and end positions.
@@ -63,33 +58,33 @@
 
     Returns:
         BaseEmbeddings: A BaseEmbeddings object for binary embeddings.
     """
     vocab = []
     with open(universe_file, "r") as f:
         for line in f:
-            eles = line.strip().split("\t")
-            region = f"{eles[0]}:{eles[1]}-{eles[2]}"
+            elements = line.strip().split("\t")
+            region = f"{elements[0]}:{elements[1]}-{elements[2]}"
             vocab.append(region)
     vocab_dict = {v: i for i, v in enumerate(vocab)}
     print("vocab size is", len(vocab))
     bin_embeds = np.zeros((len(vocab), len(tokenized_files)))
     for i, token_file in enumerate(tokenized_files):
         with open(token_file, "r") as f:
             for line in f:
-                eles = line.strip().split("\t")
-                region = f"{eles[0]}:{eles[1]}-{eles[2]}"
+                elements = line.strip().split("\t")
+                region = f"{elements[0]}:{elements[1]}-{elements[2]}"
                 if region in vocab_dict:
                     bin_embeds[vocab_dict[region]][i] = 1
     bin_embed_obj = BaseEmbeddings(bin_embeds, vocab)
     return bin_embed_obj
 
 
 def get_pca_embeddings(
-    bin_embed_obj: BaseEmbeddings, dim: int, kwargs: dict[str, Union[int, float]] = {}
+    bin_embed_obj: BaseEmbeddings, dim: int, kwargs: Dict[str, Union[int, float]] = {}
 ) -> BaseEmbeddings:
     """Gets PCA embeddings from binary embeddings.
 
     Args:
         bin_embed_obj (BaseEmbeddings): A BaseEmbeddings object for binary embeddings.
         dim (int): Number of dimensions for PCA embeddings.
         kwargs (dict[str, Union[int, float]], optional): Parameters passed to
@@ -102,15 +97,15 @@
 
     embeds = PCA(n_components=dim, **kwargs).fit_transform(bin_embed_obj.embeddings)
     pca_embed_obj = BaseEmbeddings(embeds, bin_embed_obj.vocab)
     return pca_embed_obj
 
 
 def get_umap_embeddings(
-    bin_embed_obj: BaseEmbeddings, dim: int, kwargs: dict[str, Union[int, float]] = {}
+    bin_embed_obj: BaseEmbeddings, dim: int, kwargs: Dict[str, Union[int, float]] = {}
 ) -> BaseEmbeddings:
     """Gets UMAP embeddings from binary embeddings.
 
     Args:
         bin_embed_obj (BaseEmbeddings): A BaseEmbeddings object for binary embeddings.
         dim (int): Number of dimensions for UMAP embeddings.
         kwargs (dict[str, Union[int, float]], optional): Parameters passed to
@@ -133,15 +128,15 @@
         base_embed_obj (BaseEmbeddings): A BaseEmbeddings object.
         file_name (str): Save the BaseEmbeddings object to file_name.
     """
     with open(file_name, "wb") as f:
         pickle.dump(base_embed_obj, f)
 
 
-def load_base_embeddings(path: str) -> tuple[np.ndarray, list[str]]:
+def load_base_embeddings(path: str) -> Tuple[np.ndarray, List[str]]:
     """Loads a BaseEmbeddings object.
 
     Args:
         path (str): The path to a BaseEmbeddings object.
 
     Returns:
         tuple[np.ndarray, list[str]]: Embedding vectors and the corresponding
@@ -150,15 +145,15 @@
     with open(path, "rb") as f:
         base_embed_obj = pickle.load(f)
     return base_embed_obj.embeddings, base_embed_obj.vocab
 
 
 def load_genomic_embeddings(
     model_path: str, embed_type: str = "region2vec"
-) -> tuple[np.ndarray, list[str]]:
+) -> Tuple[np.ndarray, List[str]]:
     """Loads genomic region embeddings based on the type.
 
     Args:
         model_path (str): The path to a saved model.
         embed_type (str, optional): The model type. Defaults to "region2vec".
             Can be "region2vec" or "base".
 
@@ -172,36 +167,36 @@
         embed_rep = model.wv.vectors
         return embed_rep, regions_r2v
     elif embed_type == "base":
         embed_rep, regions_r2v = load_base_embeddings(model_path)
         return embed_rep, regions_r2v
 
 
-def sort_key(x: str) -> tuple[int, int]:
+def sort_key(x: str) -> Tuple[int, int]:
     """Extracts chromosome in number and the start position of a region.
 
     Args:
         x (str): A region in the chr:start-end position.
 
     Returns:
         tuple[int, int]: Chromosome in number and the start position.
     """
-    eles = x.split(":")
-    chr_idx = eles[0][3:]
+    elements = x.split(":")
+    chr_idx = elements[0][3:]
     try:
         idx = int(chr_idx)
     except ValueError:
         idx = 23
         for c in chr_idx:
             idx += ord(c)
-    start = int(eles[1].split("-")[0].strip())
+    start = int(elements[1].split("-")[0].strip())
     return idx, start
 
 
-def get_vocab(model_path: str, type: str = "base", ordered: bool = True) -> list[str]:
+def get_vocab(model_path: str, type: str = "base", ordered: bool = True) -> List[str]:
     """Gets vocab from a model.
 
     Args:
         model_path (str): The path to a saved model.
         type (str, optional): The embedding type. Defaults to "base".
         ordered (bool, optional): Choose whether to sort the regions. Defaults
             to True.
@@ -216,22 +211,22 @@
     elif type == "base":
         _, regions_r2v = load_base_embeddings(model_path)
     if ordered:
         regions_r2v = sorted(regions_r2v, key=sort_key)
     return regions_r2v
 
 
-def write_vocab(vocab: list[str], file_name: str) -> None:
+def write_vocab(vocab: List[str], file_name: str) -> None:
     """Writes a list of regions to a file.
 
     Args:
         vocab (list[str]): A list of regions in the format of chr:start-end.
         file_name (str): Saves vocab as file_name.
     """
     with open(file_name, "w") as f:
         for v in vocab:
-            eles = v.split(":")
-            chr = eles[0].strip()
-            s, e = eles[1].split("-")
+            elements = v.split(":")
+            chr = elements[0].strip()
+            s, e = elements[1].split("-")
             s = s.strip()
             e = e.strip()
             f.write(f"{chr}\t{s}\t{e}\n")
```

### Comparing `geniml-0.2.0/geniml/io/const.py` & `geniml-0.3.0/geniml/io/const.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/io/io.py` & `geniml-0.3.0/geniml/io/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import gzip
+import logging
 import os
-from typing import List, Union, NoReturn
-import pyarrow
-from ubiquerg import is_url
+from hashlib import md5
+from typing import List, NoReturn, Union
 
+import genomicranges
 import numpy as np
 import pandas as pd
-import genomicranges
 from iranges import IRanges
-from hashlib import md5
+from ubiquerg import is_url
 
 from .const import (
     MAF_CENTER_COL_NAME,
     MAF_CHROMOSOME_COL_NAME,
     MAF_END_COL_NAME,
     MAF_ENTREZ_GENE_ID_COL_NAME,
     MAF_FILE_DELIM,
     MAF_HUGO_SYMBOL_COL_NAME,
     MAF_NCBI_BUILD_COL_NAME,
     MAF_START_COL_NAME,
     MAF_STRAND_COL_NAME,
 )
-from .utils import extract_maf_col_positions, is_gzipped, read_bedset_file
-from .exceptions import BackedFileNotAvailableError
+from .exceptions import BackedFileNotAvailableError, BEDFileReadError
+from .utils import compute_md5sum_bedset, extract_maf_col_positions, is_gzipped, read_bedset_file
+
+_LOGGER = logging.getLogger("bbclient")
 
 
 class Region:
     def __init__(self, chr: str, start: int, stop: int):
         """
         Instantiate a Region object.
 
@@ -47,15 +49,15 @@
         """
         Instantiate a RegionSet object. This can be backed or not backed. It represents a set of genomic regions.
 
         If you specify `backed` as True, then the bed file will not be loaded into memory. This is useful for large
         bed files. You can still iterate over the regions, but you cannot index into them.
 
         :param regions: path, or url to bed file or list of Region objects
-        :param backed: whether to load the bed file into memory or not
+        :param backed: whether to load the bed file into memory or not [Default: False]
         """
         # load from file
         if isinstance(regions, str):
             self.backed = backed
             self.regions: List[Region] = []
             self.path = regions
 
@@ -82,21 +84,16 @@
                     self.is_gzipped = True
                     with gzip.open(self.path, "rt") as file:
                         self.length = sum(1 for line in file if line.strip())
 
             else:
                 if is_gzipped(regions):
                     df = self._read_gzipped_file(regions)
-
                 else:
-                    # if file is gzipped, catch error and open using gzip
-                    try:
-                        df = pd.read_csv(regions, sep="\t", header=None, engine="pyarrow")
-                    except pyarrow.lib.ArrowInvalid:
-                        df = self._read_gzipped_file(regions)
+                    df = self._read_file_pd(regions, sep="\t", header=None, engine="pyarrow")
 
                 _regions = []
                 df.apply(
                     lambda row: _regions.append(Region(row[0], row[1], row[2])),
                     axis=1,
                 )
 
@@ -110,30 +107,50 @@
             self.regions = regions
             self.length = len(self.regions)
         else:
             raise ValueError("regions must be a path to a bed file or a list of Region objects")
 
         self._identifier = None
 
-    @staticmethod
-    def _read_gzipped_file(file_path: str) -> pd.DataFrame:
+    def _read_gzipped_file(self, file_path: str) -> pd.DataFrame:
         """
         Read a gzipped file into a pandas dataframe
 
         :param file_path: path to gzipped file
         :return: pandas dataframe
         """
-        return pd.read_csv(
+        return self._read_file_pd(
             file_path,
             sep="\t",
             compression="gzip",
             header=None,
             engine="pyarrow",
         )
 
+    def _read_file_pd(self, *args, **kwargs) -> pd.DataFrame:
+        """
+        Read bed file into a pandas DataFrame, and skip header rows if needed
+
+        :return: pandas dataframe
+        """
+        max_rows = 5
+        row_count = 0
+        while row_count <= max_rows:
+            try:
+                df = pd.read_csv(*args, **kwargs, skiprows=row_count)
+                if row_count > 0:
+                    _LOGGER.info(f"Skipped {row_count} rows while standardization. File: '{args}'")
+                df = df.dropna(axis=1)
+                return df
+            except (pd.errors.ParserError, pd.errors.EmptyDataError) as _:
+                if row_count <= max_rows:
+                    row_count += 1
+            # if can't open file after 5 attempts try to open it with gzip
+        return self._read_gzipped_file(*args)
+
     def __len__(self):
         return self.length
 
     def __getitem__(self, key):
         if self.backed:
             raise NotImplementedError("Backed RegionSets do not currently support indexing.")
         else:
@@ -155,16 +172,30 @@
                 open_func = gzip.open
                 mode = "rt"
             else:
                 open_func = open
                 mode = "r"
 
             with open_func(self.path, mode) as f:
+                skipped_lines = 0
+                max_skipped_lines = 5
                 for line in f:
-                    chr, start, stop = line.split("\t")[:3]
+
+                    try:
+                        chr, start, stop = line.split("\t")[:3]
+                    except ValueError as _:
+                        if skipped_lines < max_skipped_lines:
+                            skipped_lines += 1
+                            continue
+                        else:
+                            raise BEDFileReadError(f"Could not read line bed file")
+                    if skipped_lines > 0:
+                        _LOGGER.info(
+                            f"Skipped {skipped_lines} lines while opening file. File: '{self.path}'"
+                        )
                     yield Region(chr, int(start), int(stop))
         else:
             for region in self.regions:
                 yield region
 
     @property
     def identifier(self) -> str:
@@ -317,17 +348,15 @@
         if self._bedset_identifier is not None:
             return self._bedset_identifier
 
         elif self._bedset_identifier is None:
             bedfile_ids = []
             for bedfile in self.region_sets:
                 bedfile_ids.append(bedfile.compute_bed_identifier())
-            self._bedset_identifier = md5(
-                ";".join(sorted(bedfile_ids)).encode("utf-8")
-            ).hexdigest()
+            self._bedset_identifier = compute_md5sum_bedset(bedfile_ids)
 
             return self._bedset_identifier
 
 
 class SNP:
     """
     Python representation of a SNP
```

### Comparing `geniml-0.2.0/geniml/io/utils.py` & `geniml-0.3.0/geniml/io/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import gzip
 import os
+from hashlib import md5
 from typing import Dict, List, Union
 
 from .const import (
-    MAF_CHROMOSOME_COL_NAME,
     MAF_CENTER_COL_NAME,
+    MAF_CHROMOSOME_COL_NAME,
+    MAF_COLUMN,
     MAF_END_COL_NAME,
     MAF_ENTREZ_GENE_ID_COL_NAME,
     MAF_FILE_DELIM,
     MAF_HUGO_SYMBOL_COL_NAME,
     MAF_NCBI_BUILD_COL_NAME,
     MAF_START_COL_NAME,
     MAF_STRAND_COL_NAME,
-    MAF_COLUMN,
 )
 
 
 def is_gzipped(file: str) -> bool:
     """
     Check if a file is gzipped.
 
@@ -66,14 +67,31 @@
             MAF_END_COL_NAME: get_index_from_header(header, MAF_END_COL_NAME),
             MAF_STRAND_COL_NAME: get_index_from_header(header, MAF_STRAND_COL_NAME),
         }
     return col_positions
 
 
 def read_bedset_file(file_path: str) -> List[str]:
-    """Load a bedset from a text file"""
+    """
+    Load a bedset from a text file
+
+    :param file_path: path to the file
+
+    :return: list of bed identifiers
+    """
     bed_identifiers = []
 
     with open(file_path, "r") as f:
         for line in f:
             bed_identifiers.append(line.strip())
     return bed_identifiers
+
+
+def compute_md5sum_bedset(bedset: List[str]) -> str:
+    """
+    Compute the md5sum of a bedset
+
+    :param bedset: list of bed identifiers
+
+    :return: md5sum of the bedset
+    """
+    return md5("".join(bedset).encode()).hexdigest()
```

### Comparing `geniml-0.2.0/geniml/likelihood/build_model.py` & `geniml-0.3.0/geniml/likelihood/build_model.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/likelihood/cli.py` & `geniml-0.3.0/geniml/likelihood/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/models/main.py` & `geniml-0.3.0/geniml/models/main.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/nn/main.py` & `geniml-0.3.0/geniml/nn/main.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/region2vec/cli.py` & `geniml-0.3.0/geniml/region2vec/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/region2vec/const.py` & `geniml-0.3.0/geniml/region2vec/const.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/region2vec/experimental.py` & `geniml-0.3.0/geniml/region2vec/experimental.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 from typing import List, Tuple
 
 import torch
 import torch.nn as nn
 from rich.progress import track
+from torch.utils.data import Dataset
 
+from .const import DEFAULT_N_SHUFFLES, DEFAULT_NS_POWER, DEFAULT_WINDOW_SIZE, MODULE_NAME
 from .utils import shuffle_documents
-from .const import MODULE_NAME, DEFAULT_WINDOW_SIZE, DEFAULT_N_SHUFFLES, DEFAULT_NS_POWER
-
-from torch.utils.data import Dataset
 
 _LOGGER = logging.getLogger(MODULE_NAME)
 
 
 class Region2VecDataset(Dataset):
     def __init__(self, samples: List[Tuple[List[any], any]]):
         self.samples = samples
```

### Comparing `geniml-0.2.0/geniml/region2vec/main.py` & `geniml-0.3.0/geniml/region2vec/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import os
 from logging import getLogger
 from typing import List, Union
 
 import numpy as np
 import torch
-
-from rich.progress import track
 from huggingface_hub import hf_hub_download
+from rich.progress import track
 
-from ..models import ExModel
 from ..io import Region, RegionSet
+from ..models import ExModel
 from ..tokenization.main import ITTokenizer, Tokenizer
-
-from .models import Region2Vec
-from .utils import (
-    Region2VecDataset,
-    train_region2vec_model,
-    export_region2vec_model,
-    load_local_region2vec_model,
-)
 from .const import (
-    MODULE_NAME,
-    DEFAULT_WINDOW_SIZE,
+    CONFIG_FILE_NAME,
     DEFAULT_EMBEDDING_DIM,
-    DEFAULT_MIN_COUNT,
     DEFAULT_EPOCHS,
-    UNIVERSE_FILE_NAME,
+    DEFAULT_MIN_COUNT,
+    DEFAULT_WINDOW_SIZE,
     MODEL_FILE_NAME,
-    CONFIG_FILE_NAME,
-    POOLING_TYPES,
+    MODULE_NAME,
     POOLING_METHOD_KEY,
+    POOLING_TYPES,
+    UNIVERSE_FILE_NAME,
+)
+from .models import Region2Vec
+from .utils import (
+    Region2VecDataset,
+    export_region2vec_model,
+    load_local_region2vec_model,
+    train_region2vec_model,
 )
-
 
 _GENSIM_LOGGER = getLogger("gensim")
 _LOGGER = getLogger(MODULE_NAME)
 
 # demote gensim logger to warning
 _GENSIM_LOGGER.setLevel("WARNING")
 
@@ -222,15 +219,15 @@
         epochs: int = DEFAULT_EPOCHS,
         min_count: int = DEFAULT_MIN_COUNT,
         num_cpus: int = 1,
         seed: int = 42,
         save_checkpoint_path: str = None,
         gensim_params: dict = {},
         load_from_checkpoint: str = None,
-    ) -> np.ndarray:
+    ) -> bool:
         """
         Train the model.
 
         :param dataset Region2VecDataset: Dataset to train on.
         :param int window_size: Window size for the model.
         :param int epochs: Number of epochs to train for.
         :param int min_count: Minimum count for a region to be included in the vocabulary.
@@ -295,21 +292,21 @@
             path,
             checkpoint_file=checkpoint_file,
             universe_file=universe_file,
             config_file=config_file,
         )
 
     def encode(
-        self, regions: Union[Region, List[Region]], pooling: POOLING_TYPES = None
+        self, regions: Union[Region, List[Region], RegionSet], pooling: POOLING_TYPES = None
     ) -> np.ndarray:
         """
         Get the vector for a region.
 
-        :param Region region: Region to get the vector for.
-        :param str pooling: Pooling type to use.
+        :param regions: Region to get the vector for.
+        :param pooling: Pooling type to use.
 
         :return np.ndarray: Vector for the region.
         """
         # allow for overriding the pooling method
         pooling = pooling or self.pooling_method
 
         # data validation
```

### Comparing `geniml-0.2.0/geniml/region2vec/main_legacy.py` & `geniml-0.3.0/geniml/region2vec/main_legacy.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
 import multiprocessing
+import os
 from typing import List
 
 import numpy as np
 
 from . import utils
 from .region2vec_train import main as region2_train
 from .region_shuffling import main as sent_gen
```

### Comparing `geniml-0.2.0/geniml/region2vec/models.py` & `geniml-0.3.0/geniml/region2vec/models.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/region2vec/pooling.py` & `geniml-0.3.0/geniml/region2vec/pooling.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/region2vec/region2vec_train.py` & `geniml-0.3.0/geniml/region2vec/region2vec_train.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,17 +161,17 @@
         msg += f"loss {loss:>12.4f} lr {lr_scheduler.lr:>5.4f} vocab_size {len(model.wv.index_to_key):>12d} ({utils.time_str(epoch_timer.t())}/{utils.time_str(est_time)})"
         utils.log(msg)
         lr_scheduler.step()
 
     with open(os.path.join(model_dir, "loss_all.pickle"), "wb") as f:
         pickle.dump(loss_all, f)
 
-    elasped_time = run_timer.t()
+    elapsed_time = run_timer.t()
     cur_time = datetime.datetime.now().strftime("%x-%X")
-    utils.log(f"[{cur_time}] Training finished, training Time {utils.time_str(elasped_time)}")
+    utils.log(f"[{cur_time}] Training finished, training Time {utils.time_str(elapsed_time)}")
     # remove intermediate datasets
     os.system(f"rm -rf {data_folder}")  # remove the generated shuffled datasets
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Region2Vec training")
     parser.add_argument(
```

### Comparing `geniml-0.2.0/geniml/region2vec/region_shuffling.py` & `geniml-0.3.0/geniml/region2vec/region_shuffling.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             break
         # determine whether to create a new dataset
         files = glob.glob(os.path.join(DATA_FOLDER, f"pool{worker_id}*used"))
         if len(files) == 0:
             time.sleep(1)  # wait for 10 seconds
             # print('Waiting for the data to be consumed',end="\r")
         else:
-            # delete the used dataset and generate a new dataset in the same foler
+            # delete the used dataset and generate a new dataset in the same folder
             sel_file = files[random.randint(0, len(files) - 1)]
             fname = sel_file.split("/")[-1][:-4]
             os.system(f"rm -f {sel_file}")  # delete the dataset
             dpath = os.path.join(DATA_FOLDER, fname + "creating")
             with open(dpath, "w") as f:
                 pass
             if args.tokenization_mode == "hard":
```

### Comparing `geniml-0.2.0/geniml/region2vec/utils.py` & `geniml-0.3.0/geniml/region2vec/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,43 @@
+import glob
 import logging
 import os
-import glob
+import random
 import select
 import shutil
 import sys
 import time
-import random
-
 from concurrent.futures import ThreadPoolExecutor
-from typing import Dict, List, Union, Tuple, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, List, Tuple, Union
 
 import numpy as np
 import torch
-
-from yaml import safe_dump, safe_load
 from genimtools.utils import read_tokens_from_gtok
+from yaml import safe_dump, safe_load
 
 if TYPE_CHECKING:
     from gensim.models import Word2Vec as GensimWord2Vec
 
 from ..const import GTOK_EXT
-from ..tokenization.main import Tokenizer, ITTokenizer
+from ..tokenization.main import ITTokenizer, Tokenizer
 from .const import (
-    LR_TYPES,
+    CONFIG_FILE_NAME,
+    DEFAULT_EMBEDDING_DIM,
+    DEFAULT_EPOCHS,
     DEFAULT_INIT_LR,
+    DEFAULT_MIN_COUNT,
     DEFAULT_MIN_LR,
-    MODULE_NAME,
-    CONFIG_FILE_NAME,
+    DEFAULT_WINDOW_SIZE,
+    EMBEDDING_DIM_KEY,
+    EMBEDDING_DIM_KEY_OLD,
+    LR_TYPES,
     MODEL_FILE_NAME,
+    MODULE_NAME,
     UNIVERSE_FILE_NAME,
     VOCAB_SIZE_KEY,
-    EMBEDDING_DIM_KEY,
-    EMBEDDING_DIM_KEY_OLD,
-    DEFAULT_EMBEDDING_DIM,
-    DEFAULT_WINDOW_SIZE,
-    DEFAULT_EPOCHS,
-    DEFAULT_MIN_COUNT,
 )
 from .models import Region2Vec
 
 _LOGGER = logging.getLogger(MODULE_NAME)
 
 
 def prRed(skk: str) -> None:
```

### Comparing `geniml-0.2.0/geniml/scembed/annotation.py` & `geniml-0.3.0/geniml/scembed/annotation.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/scembed/argparser.py` & `geniml-0.3.0/geniml/scembed/argparser.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/scembed/cli.py` & `geniml-0.3.0/geniml/scembed/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/scembed/main.py` & `geniml-0.3.0/geniml/scembed/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,34 +4,33 @@
 
 import numpy as np
 import scanpy as sc
 import torch
 from huggingface_hub import hf_hub_download
 from rich.progress import track
 
-from ..region2vec.utils import (
-    export_region2vec_model,
-    load_local_region2vec_model,
-    train_region2vec_model,
-)
-from ..region2vec.main import Region2Vec
-from ..tokenization import ITTokenizer, Tokenizer
 from ..region2vec.const import (
-    POOLING_TYPES,
+    CONFIG_FILE_NAME,
     DEFAULT_EMBEDDING_DIM,
-    DEFAULT_WINDOW_SIZE,
-    DEFAULT_MIN_COUNT,
     DEFAULT_EPOCHS,
+    DEFAULT_MIN_COUNT,
+    DEFAULT_WINDOW_SIZE,
     MODEL_FILE_NAME,
-    UNIVERSE_FILE_NAME,
-    CONFIG_FILE_NAME,
     POOLING_METHOD_KEY,
+    POOLING_TYPES,
+    UNIVERSE_FILE_NAME,
 )
-from ..region2vec.utils import Region2VecDataset
-
+from ..region2vec.main import Region2Vec
+from ..region2vec.utils import (
+    Region2VecDataset,
+    export_region2vec_model,
+    load_local_region2vec_model,
+    train_region2vec_model,
+)
+from ..tokenization import ITTokenizer, Tokenizer
 from .const import MODULE_NAME
 
 _GENSIM_LOGGER = getLogger("gensim")
 _LOGGER = getLogger(MODULE_NAME)
 
 # demote gensim logger to warning
 _GENSIM_LOGGER.setLevel("WARNING")
```

### Comparing `geniml-0.2.0/geniml/scembed/utils.py` & `geniml-0.3.0/geniml/scembed/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 import os
 from glob import glob
-from typing import Tuple, List
+from typing import List, Tuple
 
 import scanpy as sc
-
 import torch
+from genimtools.utils import read_tokens_from_gtok
+from rich.progress import track
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset
-from rich.progress import track
-from genimtools.utils import read_tokens_from_gtok
 
 from .const import DEFAULT_CHUNK_SIZE
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AnnDataChunker:
```

### Comparing `geniml-0.2.0/geniml/search/backends/abstract.py` & `geniml-0.3.0/geniml/search/backends/abstract.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/search/backends/dbbackend.py` & `geniml-0.3.0/geniml/search/backends/dbbackend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import logging
 import os
 from typing import Dict, List, Union
 
-import logmuse
 import numpy as np
 from qdrant_client import QdrantClient
 from qdrant_client.models import PointStruct, VectorParams
 
-from ...const import PKG_NAME
-from ..const import *
+from geniml.const import PKG_NAME
+from geniml.search.const import (
+    DEFAULT_COLLECTION_NAME,
+    DEFAULT_QDRANT_CONFIG,
+    DEFAULT_QDRANT_HOST,
+    DEFAULT_QDRANT_PORT,
+    DEFAULT_QUANTIZATION_CONFIG,
+)
+
 from ..utils import verify_load_inputs
 from .abstract import EmSearchBackend
 
 _LOGGER = logging.getLogger(PKG_NAME)
 
 
 class QdrantBackend(EmSearchBackend):
@@ -29,14 +35,17 @@
         """
         Connect to Qdrant on commandline first:
         (Ubuntu Linux terminal)
         sudo docker run -p 6333:6333     -v $(pwd)/qdrant_storage:/qdrant/storage     qdrant/qdrant
 
         :param config: the vector parameter
         :param collection: name of collection
+        :param qdrant_host: host of qdrant server
+        :param qdrant_port: port of qdrant server
+        :param qdrant_api_key: api key
         """
         super().__init__()
         self.collection = collection
         self.config = config
         self.url = os.environ.get("QDRANT_HOST", qdrant_host)
         self.port = os.environ.get("QDRANT_PORT", qdrant_port)
         self.qd_client = QdrantClient(
@@ -139,17 +148,15 @@
 
     def __len__(self) -> int:
         """
         Return the number of embeddings in the backend
         """
         return self.qd_client.get_collection(collection_name=self.collection).vectors_count
 
-    def retrieve_info(
-        self, ids: Union[List[int], int], with_vec: bool = False
-    ) -> Union[
+    def retrieve_info(self, ids: Union[List[int], int], with_vec: bool = False) -> Union[
         Dict[str, Union[int, List[float], Dict[str, str]]],
         List[Dict[str, Union[int, List[float], Dict[str, str]]]],
     ]:
         """
         With a given list of storage ids, return the information of these vectors
 
         :param ids: list of ids, or a single id
```

### Comparing `geniml-0.2.0/geniml/search/backends/filebackend.py` & `geniml-0.3.0/geniml/search/backends/filebackend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,198 +1,213 @@
-from typing import Dict, List, Tuple, Union
+import os.path
+from typing import Dict, List, Union
 
 from ... import _LOGGER
+import hnswlib
 
-try:
-    import hnswlib
-
-    DEP_HNSWLIB = True
-except ImportError:
-    DEP_HNSWLIB = False
-    _LOGGER.error(
-        "HNSWBackend requires hnswlib. Install hnswlib, or ignore this if you don't need HNSWBackend"
-    )
+DEP_HNSWLIB = True
+# try:
+#
+#
+#
+# except ImportError:
+#     DEP_HNSWLIB = False
+#     _LOGGER.error(
+#         "HNSWBackend requires hnswlib. Install hnswlib, or ignore this if you don't need HNSWBackend"
+#     )
 
 import numpy as np
 
-from ..const import *
-from ..utils import verify_load_inputs
+from geniml.search.const import (
+    DEFAULT_DIM,
+    DEFAULT_EF,
+    DEFAULT_HNSW_SPACE,
+    DEFAULT_INDEX_PATH,
+    DEFAULT_M,
+)
 from .abstract import EmSearchBackend
+from ..utils import verify_load_inputs
 
-if not DEP_HNSWLIB:
-
-    class HNSWBackend(EmSearchBackend):
-        pass
-
-else:
-
-    class HNSWBackend(EmSearchBackend):
-        """A search backend that uses a local HNSW index to store and search embeddings"""
-
-        # the index
-        idx: hnswlib.Index
-        payloads: dict  # in the format of {<id>: <info dict>}, equivalent to payloads in Qdrant
-        idx_path: str  # local path where the index is saved to
-
-        def __init__(
-            self,
-            local_index_path: str = DEFAULT_INDEX_PATH,
-            space: str = DEFAULT_HNSW_SPACE,
-            dim: int = DEFAULT_DIM,
-            ef: int = DEFAULT_EF,
-            m: int = DEFAULT_M,
-        ):
-            """
-            Initiate the backend
-
-            :param local_index_path: local path where the index is saved to
-            :param space: possible options are l2, cosine or ip
-            :param dim: dimension of vectors that will be stored
-            :param ef: defines a construction time/accuracy trade-off, higher ef -> more accurate but slower
-            :param m: connected with internal dimensionality of the data, higher M -> higher accuracy/run_time
-            when ef is fixed
-            """
-
-            # initiate the index
-            self.idx = hnswlib.Index(space=space, dim=dim)  # possible options are l2, cosine or ip
-            self.idx.init_index(max_elements=0, ef_construction=ef, M=m)
-
-            # save the index to local file path
+# if not DEP_HNSWLIB:
+#
+#     class HNSWBackend(EmSearchBackend):
+#         pass
+#
+# else:
+
+
+class HNSWBackend(EmSearchBackend):
+    """A search backend that uses a local HNSW index to store and search embeddings"""
+
+    # instance variables, should not be class variables
+
+    def __init__(
+        self,
+        local_index_path: str = DEFAULT_INDEX_PATH,
+        payloads: dict = {},
+        space: str = DEFAULT_HNSW_SPACE,
+        dim: int = DEFAULT_DIM,
+        ef: int = DEFAULT_EF,
+        m: int = DEFAULT_M,
+    ):
+        """
+        Initiate the backend
+
+        :param local_index_path: local path where the index is saved to
+        :param space: possible options are l2, cosine or ip
+        :param dim: dimension of vectors that will be stored
+        :param ef: defines a construction time/accuracy trade-off, higher ef -> more accurate but slower
+        :param m: connected with internal dimensionality of the data, higher M -> higher accuracy/run_time
+        when ef is fixed
+        """
+        # super(HNSWBackend, self).__init__()
+        # initiate the index
+        self.idx = hnswlib.Index(space=space, dim=dim)  # possible options are l2, cosine or ip
+        self.idx.init_index(max_elements=0, ef_construction=ef, M=m)
+
+        # load from local index that already store vectors
+        if os.path.exists(local_index_path):
+            self.idx.load_index(local_index_path)
+            _LOGGER.info(f"Using index {local_index_path} with {self.idx.element_count} points.")
+            self.payloads = payloads
+            # self.payloads = {}
+        # save the index to local file path
+        else:
+            _LOGGER.info(f"Index {local_index_path} does not exist, creating it.")
             self.idx.save_index(local_index_path)
             self.payloads = {}
-            self.idx_path = local_index_path
+        # self.payloads = payloads
+        self.idx_path = local_index_path
 
-        def load(
-            self,
-            vectors: np.ndarray,
-            ids: Union[np.ndarray, None] = None,
-            payloads: Union[List[Dict[str, str]], None] = None,
-        ):
-            """
-            Upload embedding vectors into the hnsw index, and store their hnsw index id and payloads into metadata
-
-            :param vectors: embedding vectors, a np.ndarray with shape of (n, <vector size>)
-            :param ids: list of n point ids, or None to generate ids automatically
-            :param payloads: optional list of n dictionaries that contain vector metadata
-            :return:
-            """
-
-            # increase max_elements to contain new loadings
-            current_max = self.idx.get_max_elements()
-
-            if not ids:
-                new_max = current_max + vectors.shape[0]
-                ids = np.arange(start=current_max, stop=new_max)
-            else:
-                new_max = ids.amax()
-
-            # check if the number of embedding vectors and labels are same
-            verify_load_inputs(vectors, ids, payloads)
-
-            if payloads:
-                for i in range(len(payloads)):
-                    self.payloads[ids[i]] = payloads[i]
-
-            # update hnsw index and load embedding vectors
-            self.idx.load_index(self.idx_path, max_elements=new_max)
-            self.idx.add_items(vectors, ids)
-
-            # save hnsw index to local file
-            self.idx.save_index(self.idx_path)
-
-        def search(
-            self,
-            query: np.ndarray,
-            limit: int,
-            with_payload: bool = True,
-            with_vectors: bool = True,
-            offset: int = 0,
-        ) -> Union[
-            List[Dict[str, Union[int, float, Dict[str, str], List[float]]]],
-            List[List[Dict[str, Union[int, float, Dict[str, str], List[float]]]]],
-        ]:
-            """
-            With query vector(s), get the limit nearest neighbors.
-
-            :param query: the query vector, np.ndarray with shape of (1, dim) or (dim, )
-            :param limit: number of nearest neighbors to search for query vector
-            :param with_payload: whether payload is included in the result
-            :param with_vectors: whether the stored vector is included in the result
-            :param offset: the offset of the search results
-            :return: if the shape of query vector is (<dim>, ), a list of limit dictionaries will be returned,
-            the format of dictionary will be:
-            {
-                "id": <id>
-                "distance": <distance>
-                "payload": {
-                    <information of the vector>
-                }
-                "vector": [<the vector>]
+    def load(
+        self,
+        vectors: np.ndarray,
+        ids: Union[np.ndarray, None] = None,
+        payloads: Union[List[Dict[str, str]], None] = None,
+    ):
+        """
+        Upload embedding vectors into the hnsw index, and store their hnsw index id and payloads into metadata
+
+        :param vectors: embedding vectors, a np.ndarray with shape of (n, <vector size>)
+        :param ids: list of n point ids, or None to generate ids automatically
+        :param payloads: optional list of n dictionaries that contain vector metadata
+        :return:
+        """
+
+        # increase max_elements to contain new loadings
+        current_max = self.idx.get_max_elements()
+
+        if not ids:
+            new_max = current_max + vectors.shape[0]
+            ids = np.arange(start=current_max, stop=new_max)
+        else:
+            new_max = ids.amax()
+
+        # check if the number of embedding vectors and labels are same
+        verify_load_inputs(vectors, ids, payloads)
+
+        if payloads:
+            for i in range(len(payloads)):
+                self.payloads[ids[i]] = payloads[i]
+
+        # update hnsw index and load embedding vectors
+        self.idx.load_index(self.idx_path, max_elements=new_max)
+        self.idx.add_items(vectors, ids)
+
+        # save hnsw index to local file
+        self.idx.save_index(self.idx_path)
+
+    def search(
+        self,
+        query: np.ndarray,
+        limit: int,
+        with_payload: bool = True,
+        with_vectors: bool = True,
+        offset: int = 0,
+    ) -> Union[
+        List[Dict[str, Union[int, float, Dict[str, str], List[float]]]],
+        List[List[Dict[str, Union[int, float, Dict[str, str], np.ndarray]]]],
+    ]:
+        """
+        With query vector(s), get the limit nearest neighbors.
+
+        :param query: the query vector, np.ndarray with shape of (1, dim) or (dim, )
+        :param limit: number of nearest neighbors to search for query vector
+        :param with_payload: whether payload is included in the result
+        :param with_vectors: whether the stored vector is included in the result
+        :param offset: the offset of the search results
+        :return: if the shape of query vector is (<dim>, ), a list of limit dictionaries will be returned,
+        the format of dictionary will be:
+        {
+            "id": <id>
+            "distance": <distance>
+            "payload": {
+                <information of the vector>
             }
-            if the shape of query vector is (n, <dim>), a 2d list will be returned,
-            which is a list of n * list of limit dictionaries
-            """
-            ids, distances = self.idx.knn_query(query, k=limit + offset)
-            # ids and distances are 2d array
-            ids = ids.tolist()
-            distances = distances.tolist()
-
-            output_list = []
-            for i in range(len(ids)):
-                search_list = []
-                result_id = ids[i]
-                result_distances = distances[i]
+            "vector": [<the vector>]
+        }
+        if the shape of query vector is (n, <dim>), a 2d list will be returned,
+        which is a list of n * list of limit dictionaries
+        """
+        ids, distances = self.idx.knn_query(query, k=limit + offset)
+        # ids and distances are 2d array
+        ids = ids.tolist()
+        distances = distances.tolist()
+
+        output_list = []
+        for i in range(len(ids)):
+            search_list = []
+            result_id = ids[i]
+            result_distances = distances[i]
+            if with_vectors:
+                result_vectors = self.idx.get_items(result_id, return_type="numpy")
+            for j in range(limit):
+                output_dict = {"id": result_id[j], "distance": result_distances[j]}
+                if with_payload:
+                    output_dict["payload"] = self.payloads[result_id[j]]
                 if with_vectors:
-                    result_vectors = self.idx.get_items(result_id)
-                for j in range(limit):
-                    output_dict = {"id": result_id[j], "distance": result_distances[j]}
-                    if with_payload:
-                        output_dict["payload"] = self.payloads[result_id[j]]
-                    if with_vectors:
-                        output_dict["vector"] = result_vectors[j]
-                    search_list.append(output_dict)
-                output_list.append(search_list)
-
-            if len(output_list) == 1:
-                return output_list[0]
-            else:
-                return output_list
-
-        def __len__(self) -> int:
-            return self.idx.element_count
-
-        def retrieve_info(
-            self, ids: Union[List[int], int], with_vec: bool = False
-        ) -> Union[
-            Dict[str, Union[int, List[float], Dict[str, str]]],
-            List[Dict[str, Union[int, List[float], Dict[str, str]]]],
-        ]:
-            """
-            With an id or a list of storage ids, return the information of these vectors
-            :param ids: storage id, or a list of ids
-            :param with_vec: whether the stored vector is included in the result
-            :return:
-            """
-            if not isinstance(ids, list):
-                # retrieve() only takes iterable input
-                ids = [ids]
-            output_list = []
-            for id_ in ids:
-                output_dict = {"id": id_, "payload": self.payloads[id_]}
-                output_list.append(output_dict)
-
-            if with_vec:
-                vecs = self.idx.get_items(ids)
-                for i in range(len(vecs)):
-                    output_list[i]["vector"] = vecs[i]
-
-            # with just one id, only the dictionary instead of the list will be returned
-            if len(output_list) == 1:
-                return output_list[0]
-            else:
-                return output_list
+                    output_dict["vector"] = result_vectors[j]
+                search_list.append(output_dict)
+            output_list.append(search_list)
+
+        if len(output_list) == 1:
+            return output_list[0]
+        else:
+            return output_list
+
+    def __len__(self) -> int:
+        return self.idx.element_count
+
+    def retrieve_info(self, ids: Union[List[int], int], with_vec: bool = False) -> Union[
+        Dict[str, Union[int, List[float], Dict[str, str]]],
+        List[Dict[str, Union[int, List[float], Dict[str, str]]]],
+    ]:
+        """
+        With an id or a list of storage ids, return the information of these vectors
+        :param ids: storage id, or a list of ids
+        :param with_vec: whether the stored vector is included in the result
+        :return:
+        """
+        if not isinstance(ids, list):
+            # retrieve() only takes iterable input
+            ids = [ids]
+        output_list = []
+        for id_ in ids:
+            output_dict = {"id": id_, "payload": self.payloads[id_]}
+            output_list.append(output_dict)
+
+        if with_vec:
+            vecs = self.idx.get_items(ids, return_type="numpy")
+            for i in range(len(vecs)):
+                output_list[i]["vector"] = vecs[i]
+
+        # with just one id, only the dictionary instead of the list will be returned
+        if len(output_list) == 1:
+            return output_list[0]
+        else:
+            return output_list
 
-        def __str__(self):
-            return "HNSWBackend with {} items".format(len(self))
+    def __str__(self):
+        return "HNSWBackend with {} items".format(len(self))
 
-        def __repr__(self):
-            return "HNSWBackend with {} items".format(len(self))
+    def __repr__(self):
+        return "HNSWBackend with {} items".format(len(self))
```

### Comparing `geniml-0.2.0/geniml/search/const.py` & `geniml-0.3.0/geniml/search/const.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/text2bednn/const.py` & `geniml-0.3.0/geniml/text2bednn/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,28 @@
+# metadata from csv
+DEFAULT_GENOME_KEY = "sample_genome"
+DEFAULT_SERIES_KEY = "gse"
+DEFAULT_FILE_KEY = "file"
+BIO_GPT_REPO = "microsoft/biogpt"
+
+
 DEFAULT_TRAIN_P = 0.85 * 0.9
 DEFAULT_VALIDATE_P = 0.85 * 0.1
 
 # sentence transformer model from hugging face
 DEFAULT_NL_EMBEDDING_MODEL = "sentence-transformers/all-MiniLM-L12-v2"
+DEFAULT_MAX_SEQ_LENGTH = 1000
 
 DEFAULT_NUM_EPOCHS = 1000
 DEFAULT_NUM_UNITS = 256
 DEFAULT_NUM_EXTRA_HIDDEN_LAYERS = 0
 DEFAULT_BATCH_SIZE = 1
 DEFAULT_OPTIMIZER_NAME = "Adam"
-DEFAULT_LOSS_NAME = "mean_squared_error"
+DEFAULT_LOSS_NAME = "cosine_embedding_loss"
+DEFAULT_MARGIN = 0.0
 # embedding dimension of Region2Vec: https://huggingface.co/databio/r2v-ChIP-atlas-hg38
 DEFAULT_EMBEDDING_DIM = (100,)
 # default learning rate of Adam optimizer
 DEFAULT_LEARNING_RATE = 0.001
 
 # if validation loss does not improve after patience*epoches, training stops
 DEFAULT_PATIENCE = 0.2
@@ -21,12 +30,12 @@
 DEFAULT_VECTOR_KEY = "vector"
 DEFAULT_METADATA_KEY = "metadata"
 DEFAULT_FILENAME_KEY = "name"
 
 DEFAULT_DATALOADER_SHUFFLE = True
 MODULE_NAME = "text2bednn"
 CONFIG_FILE_NAME = "config.yaml"
-TORCH_MODEL_FILE_NAME_PATTERN = "v2c2v2c_{callback}_{checkpoint}.pt"
+TORCH_MODEL_FILE_NAME_PATTERN = "v2v_{callback}_{checkpoint}.pt"
 DEFAULT_MUST_TRAINED = True
 DEFAULT_PLOT_FILE_NAME = "training_history"
 DEFAULT_PLOT_TITLE = "Diagram of loss and epochs"
 DEFAULT_HUGGINGFACE_MODEL_NAME = "checkpoint.pt"
```

### Comparing `geniml-0.2.0/geniml/text2bednn/text2bednn.py` & `geniml-0.3.0/geniml/text2bednn/text2bednn.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import math
 import os
 from typing import Dict, List, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
-from fastembed.embedding import FlagEmbedding
 from huggingface_hub import hf_hub_download
 from torch.nn import CosineEmbeddingLoss, CosineSimilarity, Linear, MSELoss, ReLU, Sequential
 from yaml import safe_dump, safe_load
 
-from ..search.backends import HNSWBackend, QdrantBackend
 from .const import *
 from .utils import arrays_to_torch_dataloader, dtype_check
 
 _LOGGER = logging.getLogger(MODULE_NAME)
 
 
 class Vec2Vec(Sequential):
@@ -27,15 +25,15 @@
         num_extra_hidden_layers: int,
     ):
         if not isinstance(num_units, list):
             num_units = [num_units] * (1 + num_extra_hidden_layers)
         # check if number of layers match length of num_units
         if len(num_units) != 1 + num_extra_hidden_layers:
             raise ValueError("list of units number does not match number of layers")
-        # input and first hiden layer
+        # input and first hidden layer
         current_layer_units_num = num_units[0]
         layers_list = [Linear(in_features=input_dim, out_features=current_layer_units_num), ReLU()]
         previous_layer_units_num = current_layer_units_num
 
         # extra hidden layer
         for i in range(num_extra_hidden_layers):
             current_layer_units_num = num_units[i + 1]
@@ -50,15 +48,15 @@
 
         super().__init__(*layers_list)
 
 
 class Vec2VecFNN:
     def __init__(self, model_path: Union[str, None] = None):
         """
-        Initializate Vec2VecFNNtorch.
+        Initialize Vec2VecFNNtorch.
 
         :param model_path: path to the pretrained model on huggingface.
         """
         # initialize the feedforward neural network model, which is a torch.nn.Sequential
         # self.model =
         self.model = None
         # whether the model is trained
@@ -155,36 +153,43 @@
 
         :param input_vecs: input embedding vectors
         :return: the output of the neural network model
         """
         # pytorch tensor's default dtype is float 32
         return self.model(torch.from_numpy(dtype_check(input_vecs))).detach().numpy()
 
-    def compile(self, optimizer: str, loss: str, learning_rate: float):
+    def compile(
+        self,
+        optimizer: str,
+        loss: str,
+        learning_rate: float,
+        margin: Union[float, None] = DEFAULT_MARGIN,
+    ):
         """
-        Configures the model for training.
+        Configure the model for training. This includes setting the optimizer and loss function.
 
         :param optimizer: the name of optimizer
         :param loss: the name of loss function
         :param learning_rate: the learning rate of model backpropagation
+        :param margin: should be a number from −1−1 to 1, 0 to 0.5 is suggested, only for CosineEmbeddingLoss
         """
 
         # set optimizer
         if optimizer == "Adam":
             self.optimizer = torch.optim.Adam(self.model.parameters(), learning_rate)
 
         elif optimizer == "SGD":
             self.optimizer = torch.optim.SGD(self.model.parameters(), learning_rate)
 
         else:
             raise ValueError("Please give a valid name of optimizer")
 
         # set loss function
         if loss == "cosine_embedding_loss":
-            self.loss_fn = CosineEmbeddingLoss()
+            self.loss_fn = CosineEmbeddingLoss(margin=margin)
         elif loss == "cosine_similarity":
             self.loss_fn = CosineSimilarity()
         elif loss == "mean_squared_error":
             self.loss_fn = MSELoss()
         else:
             raise ValueError("Please give a valid name of loss function")
 
@@ -203,33 +208,37 @@
         early_stop: bool = False,
         patience: float = DEFAULT_PATIENCE,
         opt_name: str = DEFAULT_OPTIMIZER_NAME,
         loss_func: str = DEFAULT_LOSS_NAME,
         num_epochs: int = DEFAULT_NUM_EPOCHS,
         batch_size: int = DEFAULT_BATCH_SIZE,
         learning_rate: float = DEFAULT_LEARNING_RATE,
+        training_target: Union[np.ndarray, None] = None,
+        validating_target: Union[np.ndarray, None] = None,
         **kwargs,
     ):
         """
         Based on https://pytorch.org/tutorials/beginner/introyt/trainingyt.html
         Fit the feedforward neural network
 
         :param training_X: embedding vectors of metadata, np.ndarray with shape of (n, <dim>)
         :param training_Y: embedding vectors of region set, np.ndarray with shape of (n, <dim>)
         :param validating_data: validating data, which contains validating X and validating Y
         :param save_best: whether the best performance model is saved after each epoch (based on validation loss)
         :param folder_path: the path to the folder to save the model and config
         :param best_model_file_name: the name of the file of saved best model
-        :param early_stop: whether the training should be stoped early to prevent overfitting
+        :param early_stop: whether the training should be stopped early to prevent overfitting
         :param patience: the percentage of epoches to stop training if no validation loss improvement
         :param opt_name: name of optimizer
         :param loss_func: name of loss function
         :param num_epochs: number of training epoches
         :param batch_size: size of batch for training
         :param learning_rate: learning rate of optimizer
+        :param training_target:
+        :param validating_target:
         :param kwargs: see units and layers in reinit_model()
         """
         # if current model is empty, add layers
         if self.model is None:
             # dimensions of input and output
             input_dim = training_X.shape[1]
             output_dim = training_Y.shape[1]
@@ -243,33 +252,40 @@
             self.model = Vec2Vec(
                 input_dim=input_dim,
                 output_dim=output_dim,
                 num_units=self.config["num_units"],
                 num_extra_hidden_layers=self.config["num_extra_hidden_layers"],
             )
 
+        if training_target is None:
+            training_target = np.repeat(1, training_X.shape[0])
         # raise the error if validating data is needed but not provided
         if validating_data is not None:
             validating_X, validating_Y = validating_data
+            if validating_target is None:
+                validating_target = np.repeat(1, validating_X.shape[0])
             validating_data = arrays_to_torch_dataloader(
-                validating_X, validating_Y, batch_size=batch_size, shuffle=False
+                validating_X, validating_Y, validating_target, batch_size=batch_size, shuffle=False
             )
+
             self.most_recent_train["val_loss"] = []
         elif save_best or early_stop:
             raise ValueError("Validating data is not provided")
         if save_best and folder_path is None:
             raise ValueError(
                 "ValueError: Path to folder where the best performance model will be saved is required"
             )
 
         # compile the model
         self.compile(optimizer=opt_name, loss=loss_func, learning_rate=learning_rate)
 
         # convert training data from np.ndarray to DataLoader
-        training_data = arrays_to_torch_dataloader(training_X, training_Y, batch_size)
+        training_data = arrays_to_torch_dataloader(
+            training_X, training_Y, training_target, batch_size
+        )
 
         best_val_loss = 1_000_000.0
         patience_count = 0
         self.most_recent_train["loss"] = []
 
         for epoch in range(num_epochs):
             # gradient tracking is on
@@ -280,17 +296,17 @@
             # statistics for batch normalization.
             self.model.eval()
 
             if validating_data is not None:
                 running_val_loss = 0.0
                 # disable gradient computation
                 with torch.no_grad():
-                    for i, (val_x, val_y) in enumerate(validating_data):
+                    for i, (val_x, val_y, val_target) in enumerate(validating_data):
                         val_output = self.model(val_x)
-                        val_loss = self.calc_loss(val_output, val_y)
+                        val_loss = self.calc_loss(val_output, val_y, val_target)
                         running_val_loss += val_loss
 
                 avg_val_loss = running_val_loss / (i + 1)
                 self.most_recent_train["val_loss"].append(avg_val_loss)
                 # logging training and validating loss
                 _LOGGER.info(f"EPOCH {epoch + 1}: loss: -{avg_loss} - val_loss: -{avg_val_loss}")
 
@@ -327,179 +343,81 @@
         One epoch's training loop
 
         :return: the average training loss of one epoch
         """
         epoch_loss = 0.0
 
         # train on each batch
-        for i, (x, y) in enumerate(training_data):
+        for i, (x, y, target) in enumerate(training_data):
             # zero gradients for every batch
             self.optimizer.zero_grad()
 
             # batch prediction
             outputs = self.model(x)
 
             # compute loss and gradients
-            batch_loss = self.calc_loss(outputs, y)
+            batch_loss = self.calc_loss(outputs, y, target)
             batch_loss.backward()
 
             # adjust learning weights
             self.optimizer.step()
 
             # gather loss and report
             epoch_loss += batch_loss.item()
         return epoch_loss / (i + 1)
 
-    def calc_loss(self, outputs: torch.Tensor, y: torch.Tensor, **kwargs) -> torch.Tensor:
+    def calc_loss(
+        self, outputs: torch.Tensor, y: torch.Tensor, target: torch.Tensor
+    ) -> torch.Tensor:
         """
-        Calculating loss when different loss funcion is given
+        Calculating loss when different loss function is given
 
         :param outputs: the output of model
         :param y: the correct label
+        :param target:
         :return: the loss
+
         """
 
         if not self.config["loss"]:
             raise ValueError("Please compile the model first")
 
         # when all targets are 1
         # loss = 1 - cos(output, y)
         # https://pytorch.org/docs/stable/generated/torch.nn.CosineEmbeddingLoss.html
         elif self.config["loss"] == "cosine_embedding_loss":
-            target = kwargs.get("target") or torch.tensor(1.0).repeat(len(y))
             return self.loss_fn(outputs, y, target)
         else:
             return self.loss_fn(outputs, y)
 
     def plot_training_hist(
         self,
         save_path: Union[str, None] = None,
         plot_file_name: Union[str, None] = DEFAULT_PLOT_FILE_NAME,
         title: Union[str, None] = DEFAULT_PLOT_TITLE,
-    ):
+    ) -> None:
         """
         Plot the training & validating loss of the most recent training
 
         :param save_path: the path of folder where image will be saved
         :param plot_file_name: the file name of the png file
         :param title: the title in the image
-        :return:
+        :return: None
         """
 
         epoch_range = range(1, len(self.most_recent_train["loss"]) + 1)
         train_loss = self.most_recent_train["loss"]
+        plt.figure()
         plt.plot(epoch_range, train_loss, "r", label="Training loss")
         if self.most_recent_train["val_loss"]:
             valid_loss = self.most_recent_train["val_loss"]
             plt.plot(epoch_range, valid_loss, "b", label="Validation loss")
         plt.title(title)
         plt.legend()
         if save_path:
             plt.savefig(os.path.join(save_path, plot_file_name))
         else:
             plt.show()
+        plt.close()
 
     def __repr__(self):
         return f"Vec2Vec(input_dimension={self.config['input_dim']}, output_dimension={self.config['output_dim']}, trained={self.trained})"
-
-
-class Text2BEDSearchInterface(object):
-    """
-    search backend interface
-    """
-
-    def __init__(
-        self,
-        nl2vec_model: Union[FlagEmbedding, None],
-        vec2vec_model: Union[Vec2VecFNN, str, None],
-        search_backend: Union[QdrantBackend, HNSWBackend, None],
-    ):
-        """
-        initiate the search interface
-
-        :param nl2vec_model: model that embed natural language to vectors
-        :param vec2vec_model: model that map natural language embedding vectors to region set embedding vectors
-        :param search_backend: search backend that can store vectors and perform KNN search
-        """
-        # load the natural language encoder model
-        if isinstance(nl2vec_model, type(None)):
-            # default FlagEmbedding
-            self.set_flagembedding()
-        else:
-            self.nl2vec = nl2vec_model
-
-        # load the vec2vec model
-        if isinstance(vec2vec_model, Vec2VecFNN):
-            self.vec2vec = vec2vec_model
-        elif isinstance(vec2vec_model, str):
-            self.set_vec2vec(vec2vec_model)
-
-        # init search backend
-        if isinstance(search_backend, type(None)):
-            # init a default HNSWBackend if input is None
-            self.search_backend = HNSWBackend()
-        else:
-            self.search_backend = search_backend
-
-    def set_vec2vec(self, model_name: str):
-        """
-        With a given model_path or huggingface repo, set the vec2vec model
-
-        :param model_name: the path where the model file is saved, or the hugging face repo
-        """
-        self.vec2vec = Vec2VecFNN(model_name)
-
-    def set_flagembedding(self, model_repo: str = DEFAULT_NL_EMBEDDING_MODEL):
-        """
-        With a given huggingface repo, set the nl2vec model as a FlagEmbedding
-
-        :param model_repo: the model repository
-        see https://qdrant.github.io/fastembed/examples/Supported_Models/
-        :return:
-        """
-        _LOGGER.info(f"Setting sentence transformer model {model_repo}")
-        self.nl2vec = FlagEmbedding(model_name=model_repo)
-
-    def nl_vec_search(
-        self,
-        query: Union[str, np.ndarray],
-        limit: int = 10,
-        # offset: int = 0,
-        with_payload: bool = True,
-        with_vectors: bool = False,
-        **kwargs,
-    ) -> List[Dict[str, Union[int, float, Dict[str, str], List[float]]]]:
-        """
-        Given an input natural language, suggest region sets
-
-        :param query: searching input string
-        :param limit: number of results (nearst neighbor in vectors)
-        :param offset: the offset of the search results
-        :param with_payload: whether payloads of vectors in database will be returned [Default: True]
-        :param with_vectors: whether vectors in database will be returned [Default: False]
-        :return: a list of dictionary that contains the search results in this format:
-            {
-                "id": <id>
-                "score": <score>
-                "payload": {
-                    <information of the vector>
-                }
-                "vector": [<the vector>]
-            }
-        """
-
-        # first, get the embedding of the query string
-        if isinstance(query, str):
-            query = next(self.nl2vec.embed(query))
-        search_vector = self.vec2vec.embedding_to_embedding(query)
-        # perform the KNN search among vectors stored in backend
-        return self.search_backend.search(
-            search_vector,
-            limit,
-            with_payload=with_payload,
-            with_vectors=with_vectors,
-            # offset=offset)
-            **kwargs,
-        )
-
-    def __repr__(self):
-        return f"Text2BEDSearchInterface(nl2vec_model={self.nl2vec}, vec2vec_model={self.vec2vec}, search_backend={self.search_backend})"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geniml-0.2.0/geniml/tokenization/bedtools_tokenizer.py` & `geniml-0.3.0/geniml/tokenization/bedtools_tokenizer.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/tokenization/cli.py` & `geniml-0.3.0/geniml/tokenization/cli.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/tokenization/hard_tokenization_batch.py` & `geniml-0.3.0/geniml/tokenization/hard_tokenization_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     Tokenizes raw BED files specified by file_list. First, checks existing files
     in token_folder. If token_folder has all the tokenized BED files, then does
     nothing. Otherwise, tokenizes raw BED files that are in file_list but not
     in token_folder.
 
     Args:
-        raw_data_folder (str): The foder where raw BED files reside.
+        raw_data_folder (str): The folder where raw BED files reside.
         token_folder (str): The folder to store tokenized BED files.
         universe (str): The path to a universe file.
         file_list (str): The path to a file which contains selected BED files per row.
         bedtools (str): The path to a bedtools binary.
         fraction (float): A parameter for bedtools.intersect.
     """
     usize = 0
```

### Comparing `geniml-0.2.0/geniml/tokenization/main.py` & `geniml-0.3.0/geniml/tokenization/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 from abc import ABC, abstractmethod
 from typing import List, Union
 
 import numpy as np
 import scanpy as sc
 from genimtools.tokenizers import (
     Region as GRegion,
-    TreeTokenizer as GTreeTokenizer,
+)
+from genimtools.tokenizers import (
     TokenizedRegionSet as GTokenizedRegionSet,
+)
+from genimtools.tokenizers import (
+    TreeTokenizer as GTreeTokenizer,
+)
+from genimtools.tokenizers import (
     Universe as GUniverse,
 )
 from huggingface_hub import hf_hub_download
 from rich.progress import track
 
 from geniml.tokenization.split_file import split_file
 
-from .const import UNIVERSE_FILE_NAME, CHR_KEY, START_KEY, END_KEY
 from ..io import Region, RegionSet
+from .const import CHR_KEY, END_KEY, START_KEY, UNIVERSE_FILE_NAME
 from .hard_tokenization_batch import main as hard_tokenization
-from .utils import time_str, Timer
+from .utils import Timer, time_str
 
 
 class Tokenizer(ABC):
     @abstractmethod
     def tokenize(self, *args, **kwargs):
         raise NotImplementedError
 
@@ -218,15 +224,15 @@
     """Tokenizes raw BED files in parallel.
 
     This is the main function for hard tokenization. It uses multiple processes to
     speed up the tokenization process.
 
     Args:
         src_folder (str): The folder where raw BED files reside.
-        dst_folder (str): The foder to store tokenized BED files.
+        dst_folder (str): The folder to store tokenized BED files.
         universe_file (str): The path to a universe file.
         fraction (float, optional): A parameter for bedtools.intersect.
             Defaults to 1e-9.
         file_list (list[str], optional): A list of files (just names not full
             paths) that need to be tokenized. Defaults to None and uses all BED
             files in src_folder.
         num_workers (int, optional): Number of processes used. Defaults to 10.
```

### Comparing `geniml-0.2.0/geniml/tokenization/split_file.py` & `geniml-0.3.0/geniml/tokenization/split_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """Splits a list of files into num_parts non-overlapping batches.
 
     This is a helper function for tokenization in parallel. The dest_folder
     must be empty.
 
     Args:
         file_path (str): The path to a file with BED file names per row.
-        dest_folder (str): The folder to store splitted file lists.
+        dest_folder (str): The folder to store split file lists.
         num_parts (int): Number of batches to split.
     """
     if os.path.exists(dest_folder):
         print("Folder exists")
         return
     os.makedirs(dest_folder)
     count = get_file_rows(file_path)
```

### Comparing `geniml-0.2.0/geniml/tokenization/utils.py` & `geniml-0.3.0/geniml/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/training/adapters.py` & `geniml-0.3.0/geniml/training/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 from typing import Tuple, Union
-from lightning.pytorch.utilities.types import OptimizerLRScheduler
 
+import lightning as L
 import torch
 import torch.nn as nn
-import lightning as L
+from lightning.pytorch.utilities.types import OptimizerLRScheduler
 
+from ..atacformer import AtacformerExModel
 from ..nn import GradientReversal
 from ..region2vec import Region2VecExModel
 from ..scembed import ScEmbed
-from ..atacformer import AtacformerExModel
-
 from .const import BATCH_CORRECTION_ADVERSARIAL_TRAINING_MODES
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class CellTypeFineTuneAdapter(L.LightningModule):
     """
```

### Comparing `geniml-0.2.0/geniml/training/utils.py` & `geniml-0.3.0/geniml/training/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import contextlib
 import random
 from random import shuffle
-from typing import Tuple, List
+from typing import List, Tuple
 
-import torch
 import scanpy as sc
-
+import torch
 from rich.progress import track
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset
 
 from ..tokenization.main import ITTokenizer
```

### Comparing `geniml-0.2.0/geniml/universe/cc_universe.py` & `geniml-0.3.0/geniml/universe/cc_universe.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/universe/ccf_universe.py` & `geniml-0.3.0/geniml/universe/ccf_universe.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     inter_pos[track >= lower] = 1
     inter_pos[track > upper] = 2
     save_regions(inter_pos, chrom, bedname, track)
 
 
 def ccf_universe(cove, file_out, cove_prefix="all"):
     """
-    Creat cut-off flexible universe based on coverage track
+    Create cut-off flexible universe based on coverage track
     :param str cove: path to coverage folder
     :param str file_out: output file
     :param str cove_prefix: prefixed used for creating signal tracks
     """
     if os.path.isfile(file_out):
         raise Exception(f"File : {file_out} exists")
     file = os.path.join(cove, f"{cove_prefix}_core.bw")
```

### Comparing `geniml-0.2.0/geniml/universe/cli.py` & `geniml-0.3.0/geniml/universe/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "--merge",
         help="distance between output peaks that should be merged into one in output universe",
         default=0,
         type=int,
     )
     parser.add_argument(
         "--filter-size",
-        help="minimal siez of the region in the universe",
+        help="minimal size of the region in the universe",
         default=0,
         type=int,
     )
     parser.add_argument("--cutoff", help="cutoff value used for making universe", type=int)
 
     return parser
```

### Comparing `geniml-0.2.0/geniml/universe/custom_distribution.py` & `geniml-0.3.0/geniml/universe/custom_distribution.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/universe/hmm_universe.py` & `geniml-0.3.0/geniml/universe/hmm_universe.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     coverage_folder,
     out_file,
     prefix="all",
     normalize=True,
     save_max_cove=False,
 ):
     """
-    Create HMM based univers from coverage
+    Create HMM based universe from coverage
     :param str coverage_folder: path to folder with coverage files
     :param str start: start coverage file name
     :param str end: end coverage file name
     :param str core: core coverage file name
     :param str out_file: path to the output file with universe
     :param bool normalize: whether to normalize file
     :param bool save_max_cove: whether to save the maximum
```

### Comparing `geniml-0.2.0/geniml/universe/ml_universe.py` & `geniml-0.3.0/geniml/universe/ml_universe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import importlib.util
 import os
 from functools import cmp_to_key
 
 import numpy as np
 
 from geniml.likelihood.build_model import ModelLH
 
 from ..utils import natural_chr_sort, read_chromosome_from_bw, timer_func
 from .utils import find_full, predictions_to_bed
 
-
-import importlib.util
-
 package_name = "numba"
 
 if importlib.util.find_spec(package_name) is None:
 
     def process_part(
         cove,
         model_start=np.array([[]]),
```

### Comparing `geniml-0.2.0/geniml/universe/models.py` & `geniml-0.3.0/geniml/universe/models.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml/universe/utils.py` & `geniml-0.3.0/geniml/universe/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     return start_e, end_s
 
 
 def predictions_to_bed(states, chrom, bedname, save_max_cove=False, cove_file=None):
     """
     Save HMM prediction into a file
     :param ndarray states: result of HMM prediction
-    :param str chrom: which chromosome is being analysed
+    :param str chrom: which chromosome is being analyzed
     :param str bedname: path to the output file
     :param bool save_max_cove: whether to save the maximum peak coverage to output
      file, can result in nonstandard bed file
     :param str cove_file: file with core coverage, require for saving maximum peak coverage
     """
     ind = np.argwhere(states != 3)
     ind = ind.flatten()
@@ -75,15 +75,15 @@
     with open(bedname, "a") as f:
         f.writelines(to_file)
 
 
 def find_full_full_pos(seq, gap_size=1000, area_size=500):
     """Look for nonzero positions in coverage matrix, when most of the positions are zero
     :param ndarray seq: vector with information about non-zero positions
-    :param int gap_size: size of minium gap between non-zero positions that are separated
+    :param int gap_size: size of minimum gap between non-zero positions that are separated
     :param int area_size: size of the area around non-zero positions to be included in the result
     :return list: list of starts of non-zero regions and list of ends of non-zero regions
     """
     size = len(seq)
     seq = np.argwhere(seq >= 1).flatten()
     starts, ends = [], []
     if seq[0] > gap_size:
@@ -97,15 +97,15 @@
     ends.append(min(int(seq[-1] + area_size), size))
     return starts, ends
 
 
 def find_full_empty_pos(seq, gap_size=10000, area_size=1000):
     """Look for nonzero positions in coverage matrix, when most of the positions are nonzero
     :param ndarray seq: vector with information about non-zero positions
-    :param int gap_size: size of minium gap between non-zero positions that are separated
+    :param int gap_size: size of minimum gap between non-zero positions that are separated
     :param int area_size: size of the area around non-zero positions to be included in the result
     :return list: list of starts of non-zero regions and list of ends of non-zero regions
     """
     size = len(seq)
     seq = np.argwhere(seq == 0).flatten()
     starts, ends = [], []
     gap_len = 0
```

### Comparing `geniml-0.2.0/geniml/utils.py` & `geniml-0.3.0/geniml/utils.py`

 * *Files identical despite different names*

### Comparing `geniml-0.2.0/geniml.egg-info/SOURCES.txt` & `geniml-0.3.0/geniml.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -80,23 +80,36 @@
 geniml/scembed/const.py
 geniml/scembed/exceptions.py
 geniml/scembed/main.py
 geniml/scembed/models.py
 geniml/scembed/utils.py
 geniml/search/__init__.py
 geniml/search/const.py
+geniml/search/filebackend_tools.py
 geniml/search/utils.py
 geniml/search/backends/__init__.py
 geniml/search/backends/abstract.py
 geniml/search/backends/dbbackend.py
 geniml/search/backends/filebackend.py
+geniml/search/interfaces/__init__.py
+geniml/search/interfaces/abstract.py
+geniml/search/interfaces/bed2bed.py
+geniml/search/interfaces/text2bed.py
+geniml/search/query2vec/__init__.py
+geniml/search/query2vec/abstract.py
+geniml/search/query2vec/bed2vec.py
+geniml/search/query2vec/text2vec.py
 geniml/text2bednn/__init__.py
 geniml/text2bednn/const.py
 geniml/text2bednn/text2bednn.py
 geniml/text2bednn/utils.py
+geniml/text2bednn/embedder/__init__.py
+geniml/text2bednn/embedder/abstract.py
+geniml/text2bednn/embedder/fastembedder.py
+geniml/text2bednn/embedder/sentembedder.py
 geniml/tokenization/__init__.py
 geniml/tokenization/bedtools_tokenizer.py
 geniml/tokenization/cli.py
 geniml/tokenization/const.py
 geniml/tokenization/hard_tokenization_batch.py
 geniml/tokenization/main.py
 geniml/tokenization/split_file.py
```

### Comparing `geniml-0.2.0/setup.py` & `geniml-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,20 @@
         "geniml.training",
         "geniml.region2vec",
         "geniml.scembed",
         "geniml.tokenization",
         "geniml.universe",
         "geniml.io",
         "geniml.text2bednn",
+        "geniml.text2bednn.embedder",
         "geniml.bbclient",
         "geniml.search",
         "geniml.search.backends",
+        "geniml.search.interfaces",
+        "geniml.search.query2vec",
         "geniml.nn",
     ],
     version=version,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Genomic interval toolkit",
     classifiers=[
```

### Comparing `geniml-0.2.0/tests/test_atacformer.py` & `geniml-0.3.0/tests/test_atacformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import os
+import lightning as L
 import pytest
-
 import torch
-import lightning as L
-
 from torch.utils.data import DataLoader
-from torch.nn.utils.rnn import pad_sequence
+
 from geniml.atacformer.main import Atacformer, AtacformerExModel
 from geniml.atacformer.utils import AtacformerMLMDataset
 from geniml.tokenization.main import ITTokenizer
 from geniml.training.adapters import MLMAdapter
 
 
 @pytest.fixture
@@ -18,46 +15,50 @@
 
 
 @pytest.fixture
 def data():
     return "tests/data/gtok_sample/"
 
 
+@pytest.mark.skip("Too new to test")
 def test_atacformer_dataset():
     path_to_data = "tests/data/gtok_sample/"
     dataset = AtacformerMLMDataset(path_to_data, 999, 10_000)
 
     assert dataset is not None
     assert all([isinstance(x, tuple) for x in dataset])
 
 
+@pytest.mark.skip("Too new to test")
 def test_atacformer_init():
     model = Atacformer(
         10_000,  # vocab_size of 10,000 regions
     )
     assert model is not None
 
     input = torch.randint(0, 10_000, (32, 128))
     output = model(input)
     assert output.shape == (32, 128, 768)
 
 
+@pytest.mark.skip("Too new to test")
 def test_atacformer_exmodel_init(universe_file: str):
     tokenizer = ITTokenizer(universe_file)
     model = AtacformerExModel(
         tokenizer=tokenizer,
     )
 
     # these are the defaults
     assert model._model.d_model == 768
     assert model._model.vocab_size == 2436
     assert model._model.nhead == 8
     assert model._model.num_layers == 6
 
 
+@pytest.mark.skip("Too new to test")
 def test_train_atacformer_ex_model(universe_file: str, data: str):
     # make tokenizer and model
     tokenizer = ITTokenizer(universe_file)
     model = AtacformerExModel(
         tokenizer=tokenizer,
     )
```

### Comparing `geniml-0.2.0/tests/test_batch_correction.py` & `geniml-0.3.0/tests/test_batch_correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import pytest
-
 import lightning as L
-
+import pytest
 from torch.utils.data import DataLoader
+
 from geniml.scembed import ScEmbed
 from geniml.scembed.utils import BatchCorrectionDataset, BCBatchCollator
 from geniml.training.adapters import AdversarialBatchCorrectionAdapter
 
 
 @pytest.fixture
 def universe_file():
```

### Comparing `geniml-0.2.0/tests/test_bbclient.py` & `geniml-0.3.0/tests/test_bbclient.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import os
+from unittest.mock import Mock
 
+import boto3
+import botocore
 import genomicranges
 import pytest
+
 from geniml.bbclient import BBClient
 from geniml.io import BedSet, RegionSet
 
 DATA_TEST_FOLDER = os.path.join(
     os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
     "tests",
     "data",
@@ -39,56 +43,62 @@
 
 
 @pytest.fixture
 def local_bedfile_list():
     return ALL_BEDFILE_PATH
 
 
+class TestBedCaching:
+    pass
+
+
 class TestBBClientCaching:
     def test_init(self, cache_path):
         """
         Test initialization of BBClient
         """
         bbclient = BBClient(cache_folder=cache_path)
-        assert bbclient is not None
+        assert isinstance(bbclient, BBClient)
 
     def test_init_no_cache_folder(self):
         """
         Test initialization of BBClient without cache folder
         """
         with pytest.raises(TypeError):
             BBClient(cache_folder=None)
 
-    def test_bed_caching_from_path(self, tmp_path, local_bedfile_path):
+    @pytest.mark.parametrize("bedfile_path", ALL_BEDFILE_PATH)
+    def test_bed_caching_from_path(self, bedfile_path, tmp_path):
         bbclient = BBClient(cache_folder=tmp_path)
-        bedfile_id = bbclient.add_bed_to_cache(local_bedfile_path)
+        bedfile_id = bbclient.add_bed_to_cache(bedfile_path)
         assert bedfile_id is not None
 
-    def test_bed_caching_from_region_set(self, tmp_path, local_bedfile_path):
+    @pytest.mark.parametrize("bedfile_path", ALL_BEDFILE_PATH)
+    def test_bed_caching_from_region_set(self, tmp_path, bedfile_path):
         bbclient = BBClient(cache_folder=tmp_path)
-        bedfile = RegionSet(local_bedfile_path)
+        bedfile = RegionSet(bedfile_path)
         bbclient.add_bed_to_cache(bedfile)
         path_in_cache = bbclient.seek(bedfile.identifier)
         assert bedfile.compute_bed_identifier() == os.path.split(path_in_cache)[1].split(".")[0]
 
     def test_bedset_caching(self, tmp_path, local_bedfile_list):
         bbclient = BBClient(cache_folder=tmp_path)
         bedset = BedSet(local_bedfile_list)
         bedset_id = bbclient.add_bedset_to_cache(bedset)
         path_in_cache = bbclient.seek(bedset_id)
         assert bedset_id == os.path.split(path_in_cache)[1].split(".")[0]
 
-    def test_error_bed_not_in_cache(self, tmp_path, local_bedfile_path):
+    def test_bed_not_in_cache_error(self, tmp_path, local_bedfile_path):
         bbclient = BBClient(cache_folder=tmp_path)
         # skip caching
         bedfile = RegionSet(local_bedfile_path)
         with pytest.raises(FileNotFoundError):
             bbclient.seek(bedfile.identifier)
 
-    def test_error_bedset_not_in_cache(self, tmp_path, local_bedfile_list):
+    def test_bedset_not_in_cache_error(self, tmp_path, local_bedfile_list):
         bbclient = BBClient(cache_folder=tmp_path)
         bedset_id = BedSet(local_bedfile_list).identifier
         with pytest.raises(FileNotFoundError):
             bbclient.seek(bedset_id)
 
     def test_remove_bed_from_cache(self, tmp_path, local_bedfile_path):
         bbclient = BBClient(cache_folder=tmp_path)
@@ -104,14 +114,47 @@
         bedset_id = bbclient.add_bedset_to_cache(bedset)
         assert bbclient.seek(bedset_id)
         bbclient.remove_bedset_from_cache(bedset_id)
         with pytest.raises(FileNotFoundError):
             bbclient.seek(bedset_id)
 
 
+class TestS3Caching:
+    def test_upload_s3(self, mocker, local_bedfile_path, tmp_path):
+        bbclient = BBClient(cache_folder=tmp_path)
+        bedfile_id = bbclient.add_bed_to_cache(local_bedfile_path)
+        upload_mock = mocker.patch(
+            "boto3.s3.inject.upload_file",
+        )
+        bbclient.add_bed_to_s3(bedfile_id, s3_path="test_test")
+        assert upload_mock.called
+
+    def test_download_s3(self, mocker, local_bedfile_path, tmp_path):
+        bbclient = BBClient(cache_folder=tmp_path)
+        download_mock = mocker.patch(
+            "boto3.s3.inject.download_file",
+        )
+        bbclient.get_bed_from_s3("test_id", s3_path="test_test")
+        assert download_mock.called
+
+    def test_download_s3_404(self, mocker, local_bedfile_path, tmp_path):
+        bbclient = BBClient(cache_folder=tmp_path)
+        download_mock = mocker.patch(
+            "boto3.s3.inject.download_file",
+            side_effect=botocore.exceptions.ClientError(
+                {"Error": {"Code": "404"}}, "operation_name"
+            ),
+        )
+        with pytest.raises(FileNotFoundError):
+            bbclient.get_bed_from_s3("test_id", s3_path="test_test")
+
+        assert download_mock.called
+
+
+# TODO: rewrite it so that it makes the requests
 # @pytest.mark.bedbase
 @pytest.mark.skipif(
     "not config.getoption('--bedbase')",
     reason="Only run when --bedbase is given",
 )
 def test_bedbase_caching(tmp_path, bedset_id, bedfile_id, request):
     """
```

### Comparing `geniml-0.2.0/tests/test_finetuning.py` & `geniml-0.3.0/tests/test_finetuning.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import torch
+import pytest
+
 import lightning as L
 import scanpy as sc
-
-from torch.utils.data import DataLoader
+import torch
 from sklearn.model_selection import train_test_split
+from torch.utils.data import DataLoader
 
+from geniml.region2vec.main import Region2Vec, Region2VecExModel
 from geniml.tokenization.main import ITTokenizer
+from geniml.training import CellTypeFineTuneAdapter
 from geniml.training.utils import (
-    generate_fine_tuning_dataset,
     FineTuningDataset,
     collate_finetuning_batch,
+    generate_fine_tuning_dataset,
 )
-from geniml.training import CellTypeFineTuneAdapter
-from geniml.region2vec.main import Region2Vec, Region2VecExModel
 
 
 def test_generate_finetuning_dataset():
     t = ITTokenizer("tests/data/universe.bed")
     adata = sc.read_h5ad("tests/data/pbmc_hg38.h5ad")
 
     pos, neg, pos_labels, neg_labels = generate_fine_tuning_dataset(
@@ -30,24 +31,26 @@
     assert len(pos) == len(neg)
     assert len(pos) == len(pos_labels)
     assert len(neg) == len(neg_labels)
     # not sure why the below doesnt work right now
     # assert len(pos) == sum([(n * (n - 1)) for n in adata.obs.groupby("cell_type").size()])
 
 
+@pytest.mark.skip("Too slow for CI/CD. Mostly a development tool anyways.")
 def test_init_celltype_adapter():
     model = Region2VecExModel(
         tokenizer="tests/data/universe.bed",
     )
     adapter = CellTypeFineTuneAdapter(model)
     assert adapter is not None
-    assert isinstance(adapter.nn_model, Region2Vec)
-    assert adapter.nn_model.projection.num_embeddings == len(model.tokenizer)
+    assert isinstance(adapter.r2v_model, Region2Vec)
+    assert adapter.r2v_model.projection.num_embeddings == len(model.tokenizer)
 
 
+@pytest.mark.skip("Too slow for CI/CD. Mostly a development tool anyways.")
 def test_train_with_adapter():
     # make models
     model = Region2VecExModel(
         tokenizer="tests/data/universe.bed",
     )
     adapter = CellTypeFineTuneAdapter(model)
 
@@ -89,14 +92,15 @@
         # num_workers=multiprocessing.cpu_count() - 2,
     )
 
     trainer = L.Trainer(profiler="simple", min_epochs=3)
     trainer.fit(adapter, train_dataloaders=train_dataloader, val_dataloaders=test_dataloader)
 
 
+@pytest.mark.skip("Too slow for CI/CD. Mostly a development tool anyways.")
 def test_train_export():
     # make models
     model = Region2VecExModel(
         tokenizer="tests/data/universe.bed",
     )
     adapter = CellTypeFineTuneAdapter(model)
```

### Comparing `geniml-0.2.0/tests/test_io.py` & `geniml-0.3.0/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import pytest
 import os
 
-from geniml.io.io import SNP, Maf, Region, RegionSet
-from geniml.io.exceptions import GenimlBaseError
 import genomicranges
+import pytest
+
+from geniml.io.exceptions import GenimlBaseError
+from geniml.io.io import SNP, Maf, Region, RegionSet
 
 DATA_TEST_FOLDER = os.path.join(
     os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
     "tests",
     "data",
     "io_data",
 )
```

### Comparing `geniml-0.2.0/tests/test_region2vec.py` & `geniml-0.3.0/tests/test_region2vec.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,63 +54,59 @@
     y = model.forward(x)
     assert y.shape == (10, 100)
 
 
 def test_r2v_pytorch_tokenizer_is_file_on_disk(universe_file: str):
     model = Region2VecExModel(tokenizer=universe_file)
     assert model is not None
-    assert len(model.tokenizer) == 2380
+    assert len(model.tokenizer) == 2435
 
 
 def test_r2v_pytorch_tokenizer_is_on_hf():
     model = Region2VecExModel(tokenizer="databio/r2v-ChIP-atlas-hg38-v2")
     assert model is not None
     assert len(model.tokenizer) == 1_698_713
 
 
 def test_r2v_pytorch_exmodel_train(universe_file: str):
     model = Region2VecExModel(tokenizer=ITTokenizer(universe_file))
     assert model is not None
 
-    rs1 = list(RegionSet("tests/data/to_tokenize.bed"))
-    rs2 = list(RegionSet("tests/data/to_tokenize2.bed"))
-    rs3 = rs1[0:10] + rs2[0:10]
+    dataset = Region2VecDataset("tests/data/gtok_sample/", convert_to_str=True)
 
-    loss = model.train([rs1, rs2, rs3], epochs=10)
-    assert loss[0] > loss[-1]
+    loss = model.train(dataset, epochs=10, min_count=1)
+    assert loss
 
 
 def test_r2v_pytorch_encode(universe_file: str):
     model = Region2VecExModel(tokenizer=ITTokenizer(universe_file))
     assert model is not None
 
     r = Region("chr1", 63403166, 63403785)
     embedding = model.encode(r)
     assert embedding is not None
     assert isinstance(embedding, np.ndarray)
-    assert embedding.shape == (100,)
+    assert embedding.shape == (1, 100)
 
     rs = RegionSet("tests/data/to_tokenize.bed")
     embedding = model.encode(list(rs))
     assert embedding is not None
     assert isinstance(embedding, np.ndarray)
-    assert embedding.shape == (100,)
+    assert embedding.shape == (13, 100)
 
 
 def test_save_load_pytorch_exmodel(universe_file: str):
     model = Region2VecExModel(tokenizer=ITTokenizer(universe_file))
     assert model is not None
 
-    rs1 = list(RegionSet("tests/data/to_tokenize.bed"))
-    rs2 = list(RegionSet("tests/data/to_tokenize2.bed"))
-    rs3 = rs1[0:10] + rs2[0:10]
+    dataset = Region2VecDataset("tests/data/gtok_sample/", convert_to_str=True)
+    loss = model.train(dataset, epochs=10, min_count=1)
 
-    loss = model.train([rs1, rs2, rs3], epochs=10)
     before_embedding = model.encode(Region("chr1", 63403166, 63403785))
-    assert loss[0] > loss[-1]
+    assert loss
     try:
         # save the model
         model.export("tests/data/test_model/")
         assert os.path.exists("tests/data/test_model/checkpoint.pt")
         assert os.path.exists("tests/data/test_model/universe.bed")
 
         # load in
@@ -124,10 +120,10 @@
         try:
             os.remove("tests/data/test_model/checkpoint.pt")
             os.remove("tests/data/test_model/universe.bed")
             os.remove("tests/data/test_model/config.yaml")
             os.rmdir("tests/data/test_model/")
         except Exception as e:
             # just try to remove it, if it doesn't work, then pass, means something
-            # else wrong occured up the stack
+            # else wrong occurred up the stack
             print(e)
             pass
```

### Comparing `geniml-0.2.0/tests/test_scembed.py` & `geniml-0.3.0/tests/test_scembed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import os
 import sys
 
 import pytest
 import scanpy as sc
-
-from tqdm import tqdm
 from genimtools.utils import write_tokens_to_gtok
+from tqdm import tqdm
+
 from geniml.region2vec.utils import Region2VecDataset
-from geniml.tokenization.main import ITTokenizer
 from geniml.scembed.main import ScEmbed
+from geniml.tokenization.main import ITTokenizer
 
 # add parent directory to path
 sys.path.append("../")
 
 
 # set to DEBUG to see more info
 logging.basicConfig(level=logging.INFO)
@@ -44,27 +44,31 @@
     assert model
 
 
 def test_model_training(universe_file: str, pbmc_data: sc.AnnData):
     # remove gensim logging
     logging.getLogger("gensim").setLevel(logging.ERROR)
     model = ScEmbed(tokenizer=ITTokenizer(universe_file))  # set to 1 for testing
-    model.train(pbmc_data, epochs=3)
+
+    dataset = Region2VecDataset("tests/data/gtok_sample/", convert_to_str=True)
+    model.train(dataset, epochs=3, min_count=1)
 
     # keep only columns with values > 0
     pbmc_data = pbmc_data[:, pbmc_data.X.sum(axis=0) > 0]
 
     assert model.trained
 
 
-def test_model_train_and_export(universe_file: str, pbmc_data: sc.AnnData):
+def test_model_train_and_export(universe_file: str):
     # remove gensim logging
     logging.getLogger("gensim").setLevel(logging.ERROR)
     model = ScEmbed(tokenizer=ITTokenizer(universe_file))  # set to 1 for testing
-    model.train(pbmc_data, epochs=3)
+
+    dataset = Region2VecDataset("tests/data/gtok_sample/", convert_to_str=True)
+    model.train(dataset, epochs=3, min_count=1)
 
     assert model.trained
 
     # save
     try:
         model.export("tests/data/model-tests")
         model = ScEmbed.from_pretrained("tests/data/model-tests")
@@ -83,16 +87,16 @@
     model = ScEmbed(hf_model)
     embeddings = model.encode(pbmc_data)
     assert embeddings.shape[0] == pbmc_data.shape[0]
 
 
 @pytest.mark.skip(reason="This is for my own testing")
 def test_end_to_end_training():
-    from umap import UMAP
     import matplotlib.pyplot as plt
+    from umap import UMAP
 
     data_path = os.path.expandvars("$HOME/Desktop/buenrostro2018.h5ad")
     tokens_path = os.path.expandvars("$HOME/Desktop/tokens")
     universe_path = os.path.expandvars("$HOME/Desktop/universe.bed")
     export_path = os.path.expandvars("$HOME/Desktop/scembed-model")
 
     # try to remove tokens folder if it exists
```

### Comparing `geniml-0.2.0/tests/test_tokenization.py` & `geniml-0.3.0/tests/test_tokenization.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # tokenize a bed file
     bed_file = "tests/data/to_tokenize.bed"
 
     # read in the bed file to test
     rs = RegionSet(bed_file)
 
     # tokenize
-    tokens = t.tokenize(rs)
+    tokens = t.tokenize(rs, ids_only=False)
     region_tokens = tokens.regions
 
     # filter out UNK tokens
     assert len(region_tokens) == 14  # one of the regions gets split into two tokens
     region_tokens = [t for t in region_tokens if t.chr != "chrUNK"]
 
     # count tokens
@@ -59,15 +59,15 @@
     # tokenize a bed file
     bed_file = "tests/data/to_tokenize.bed"
 
     # read in the bed file to test
     rs = RegionSet(bed_file)
 
     # tokenize
-    tokens = t.tokenize(rs)
+    tokens = t.tokenize(rs, ids_only=False)
     region_tokens = tokens.regions
 
     # filter out UNK tokens
     assert len(region_tokens) == 14  # one of the regions gets split into two tokens
     region_tokens = [t for t in region_tokens if t.chr != "chrUNK"]
 
     # count tokens
```

