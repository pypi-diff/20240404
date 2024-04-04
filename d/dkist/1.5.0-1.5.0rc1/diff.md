# Comparing `tmp/dkist-1.5.0.tar.gz` & `tmp/dkist-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-1.5.0.tar", last modified: Thu Apr  4 09:24:58 2024, max compression
+gzip compressed data, was "dkist-1.5.0rc1.tar", last modified: Tue Apr  2 20:54:09 2024, max compression
```

## Comparing `dkist-1.5.0.tar` & `dkist-1.5.0rc1.tar`

### file list

```diff
@@ -1,244 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.605861 dkist-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-04 09:24:47.000000 dkist-1.5.0/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 09:24:47.000000 dkist-1.5.0/.codespell-dict.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-04 09:24:47.000000 dkist-1.5.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-04 09:24:47.000000 dkist-1.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-04 09:24:47.000000 dkist-1.5.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-04 09:24:47.000000 dkist-1.5.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.557861 dkist-1.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.569861 dkist-1.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 09:24:47.000000 dkist-1.5.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 09:24:47.000000 dkist-1.5.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 09:24:47.000000 dkist-1.5.0/.github/ISSUE_TEMPLATE/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.569861 dkist-1.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-04 09:24:47.000000 dkist-1.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-04 09:24:47.000000 dkist-1.5.0/.github/workflows/prepare-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-04 09:24:47.000000 dkist-1.5.0/.github/workflows/sub_package_update.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-04 09:24:47.000000 dkist-1.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-04 09:24:47.000000 dkist-1.5.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 09:24:47.000000 dkist-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-04 09:24:47.000000 dkist-1.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 09:24:47.000000 dkist-1.5.0/.rtd-environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-04 09:24:47.000000 dkist-1.5.0/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)    24119 2024-04-04 09:24:47.000000 dkist-1.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-04 09:24:47.000000 dkist-1.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-04 09:24:47.000000 dkist-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-04 09:24:47.000000 dkist-1.5.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-04 09:24:47.000000 dkist-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-04 09:24:58.605861 dkist-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-04 09:24:47.000000 dkist-1.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.569861 dkist-1.5.0/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-04 09:24:47.000000 dkist-1.5.0/changelog/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-04 09:24:47.000000 dkist-1.5.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.569861 dkist-1.5.0/dkist/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.569861 dkist-1.5.0/dkist/config/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.573861 dkist-1.5.0/dkist/data/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/VISP_HEADER.hdr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/api_search_values.json
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.577861 dkist-1.5.0/dkist/data/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/5d_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/AGLKO-inv.ecsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.581861 dkist-1.5.0/dkist/data/test/EIT/
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.000010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.020010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.030011_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.040010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.050010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.060010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.080010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.090010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.100010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.110010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/efz20040301.120010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/EIT/eit_test_dataset.asdf
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96407 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/eit_dataset-0.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    96552 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/eit_dataset-0.2.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    97195 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/eit_dataset-0.3.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    99686 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/eit_dataset-1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    32741 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/eit_dataset-1.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/eit_dataset-1.2.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/globus_operation_ls_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/globus_search_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   136848 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/large_visp.asdf.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.581861 dkist-1.5.0/dkist/data/test/small_visp/
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/small_visp/0.fits
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/small_visp/1.fits
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/small_visp/2.fits
--rw-r--r--   0 runner    (1001) docker     (127)   104749 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/small_visp/test_visp.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/test_old_wcs_BRMQY.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   619185 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   619217 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   599267 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.581861 dkist-1.5.0/dkist/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.585861 dkist-1.5.0/dkist/dataset/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/tests/test_load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/tests/test_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/dkist.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.585861 dkist-1.5.0/dkist/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.585861 dkist-1.5.0/dkist/io/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.585861 dkist-1.5.0/dkist/io/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.585861 dkist-1.5.0/dkist/io/asdf/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/converters/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/converters/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/converters/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/converters/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.585861 dkist-1.5.0/dkist/io/asdf/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.589861 dkist-1.5.0/dkist/io/asdf/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.589861 dkist-1.5.0/dkist/io/asdf/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.589861 dkist-1.5.0/dkist/io/asdf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/asdf/tests/test_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/level_1_dataset_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.589861 dkist-1.5.0/dkist/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/tests/test_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/io/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.593861 dkist-1.5.0/dkist/net/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/attrs_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.593861 dkist-1.5.0/dkist/net/globus/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.593861 dkist-1.5.0/dkist/net/globus/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/tests/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/globus/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.593861 dkist-1.5.0/dkist/net/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/test_attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/test_attrs_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/net/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.597861 dkist-1.5.0/dkist/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/tests/generate_aia_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/tests/generate_eit_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/tests/generate_eit_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.597861 dkist-1.5.0/dkist/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/_model_to_graphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.597861 dkist-1.5.0/dkist/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/utils/tests/test_sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.597861 dkist-1.5.0/dkist/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/wcs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26350 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/wcs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.597861 dkist-1.5.0/dkist/wcs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/wcs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/wcs/tests/test_coupled_compound_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24398 2024-04-04 09:24:47.000000 dkist-1.5.0/dkist/wcs/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.605861 dkist-1.5.0/dkist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 09:24:58.000000 dkist-1.5.0/dkist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.601861 dkist-1.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/developer.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.601861 dkist-1.5.0/docs/howto_guides/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/howto_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/howto_guides/reproject_vbi_mosaic.md
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.601861 dkist-1.5.0/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    72150 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/logo/icon_square.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.601861 dkist-1.5.0/docs/topic_guides/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/topic_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/topic_guides/level1data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/topic_guides/loading.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/topic_guides/net.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/topic_guides/usertools.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.601861 dkist-1.5.0/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/1_astropy_and_sunpy.md
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/1_astropy_and_sunpy_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/2_search_and_asdf_download.md
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/2_search_and_asdf_download_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/3_the_dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/3_the_dataset_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/4_more_dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/5_downloading_data.md
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/6_visualization.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/tutorial/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:24:58.605861 dkist-1.5.0/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/whatsnew/1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/whatsnew/1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-04 09:24:47.000000 dkist-1.5.0/docs/whatsnew/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-04 09:24:47.000000 dkist-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-04 09:24:47.000000 dkist-1.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 09:24:58.605861 dkist-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-04-04 09:24:47.000000 dkist-1.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-04 09:24:47.000000 dkist-1.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codespell-dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.062747 dkist-1.5.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/BUG_REPORT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/prepare-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/sub_package_update.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    23150 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/309.bugfix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/344.trivial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/347.feature.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/349.doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/361.bugfix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/dkist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 20:54:08.000000 dkist-1.5.0rc1/dkist/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/dkist/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.078747 dkist-1.5.0rc1/dkist/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/VISP_HEADER.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/api_search_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.082747 dkist-1.5.0rc1/dkist/data/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/5d_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/AGLKO-inv.ecsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/data/test/EIT/
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.000010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.020010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.030011_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.040010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.050010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.060010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.080010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.090010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.100010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.110010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.120010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/eit_test_dataset.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96407 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    96552 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    97195 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.3.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    99686 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    32741 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/globus_operation_ls_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/globus_search_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   136848 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/large_visp.asdf.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/data/test/small_visp/
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/0.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/1.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/2.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   104749 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/test_visp.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_old_wcs_BRMQY.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   619185 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   619217 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   599267 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/dataset/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dkist.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/entry_points.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/asdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/level_1_dataset_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/test_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/net/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attrs_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/globus/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attrs_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_aia_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_eit_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_eit_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/_model_to_graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/test_sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26350 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/wcs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/test_coupled_compound_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24398 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/dkist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:08.000000 dkist-1.5.0rc1/dkist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/developer.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/howto_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/howto_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/howto_guides/reproject_vbi_mosaic.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    72150 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/logo/icon_square.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/topic_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/level1data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/loading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/net.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/usertools.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/3_the_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/3_the_dataset_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/4_more_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/5_downloading_data.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/6_visualization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/tox.ini
```

### Comparing `dkist-1.5.0/.coveragerc` & `dkist-1.5.0rc1/.coveragerc`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.cruft.json` & `dkist-1.5.0rc1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.flake8` & `dkist-1.5.0rc1/.flake8`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md` & `dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/BUG_REPORT.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md` & `dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.github/workflows/main.yml` & `dkist-1.5.0rc1/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
       - 'prepare-v*'
     tags:
       - 'v*'
       - '!*dev*'
       - '!*pre*'
       - '!*post*'
   pull_request:
-  release:
-    types: [published]
   schedule:
     #        ┌───────── minute (0 - 59)
     #        │ ┌───────── hour (0 - 23)
     #        │ │ ┌───────── day of the month (1 - 31)
     #        │ │ │ ┌───────── month (1 - 12 or JAN-DEC)
     #        │ │ │ │ ┌───────── day of the week (0 - 6 or SUN-SAT)
     - cron: '0 9 * * 1'  # Every Monday at 0900 UTC
```

### Comparing `dkist-1.5.0/.github/workflows/prepare-release.yml` & `dkist-1.5.0rc1/.github/workflows/prepare-release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
       - name: Update attrs
         run: |
           python -c "from dkist.net.attrs_values import attempt_local_update; attempt_local_update(user_file='./dkist/data/api_search_values.json', silence_errors=False)"
 
       - name: Commit Attrs
         run: |
-          git update-index --refresh || true
+          git update-index --refresh
           git diff-index --quiet HEAD -- || git commit -m "Update attrs values before release [skip ci]" dkist/data/api_search_values.json
 
       - name: Install towncrier
         run: python -m pip install --upgrade towncrier pre-commit
 
       - name: Run towncrier in draft to capture the output
         run: towncrier build --draft --version ${{ inputs.version }} --yes > release-changelog.rst
```

### Comparing `dkist-1.5.0/.github/workflows/sub_package_update.yml` & `dkist-1.5.0rc1/.github/workflows/sub_package_update.yml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.gitignore` & `dkist-1.5.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.pre-commit-config.yaml` & `dkist-1.5.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.readthedocs.yaml` & `dkist-1.5.0rc1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/.ruff.toml` & `dkist-1.5.0rc1/.ruff.toml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/CHANGELOG.rst` & `dkist-1.5.0rc1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-1.5.0 (2024-04-03)
-==================
-
-Features
---------
-
-- Our minimum Python version is now 3.10 inline with `SPEC-0 <https://scientific-python.org/specs/spec-0000/>`__. (`#347 <https://github.com/DKISTDC/dkist/pull/347>`_)
-
-
-Bug Fixes
----------
-
-- Fix broadcasting issues during pixel -> world conversion for models with a Ravel component. (`#309 <https://github.com/DKISTDC/dkist/pull/309>`_)
-- Fix a performance regression when dask>=2024.2.1 is installed. (`#361 <https://github.com/DKISTDC/dkist/pull/361>`_)
-
-
-Improved Documentation
-----------------------
-
-- Add a how to guide describing how to reproject VBI data. Also migrate tutorial to the latest DDT datasets. (`#349 <https://github.com/DKISTDC/dkist/pull/349>`_)
-
-
-Trivial/Internal Changes
-------------------------
-
-- Refactor various subclasses of VaryingCelestialTransform to centralise the calculations in preparation for improving performance. (`#344 <https://github.com/DKISTDC/dkist/pull/344>`_)
-
-
 1.4.0 (2024-02-26)
 ==================
 
 Bug Fixes
 ---------
 
 - Correct Fido time searching to use `endTimeMin` and `startTimeMax` (in the correct order) so that searching returns any dataset with a partially or completely overlapping time range. (`#336 <https://github.com/DKISTDC/dkist/pull/336>`_)
```

### Comparing `dkist-1.5.0/CONTRIBUTING.md` & `dkist-1.5.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/LICENSE.rst` & `dkist-1.5.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/PKG-INFO` & `dkist-1.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.5.0
+Version: 1.5.0rc1
 Summary: DKIST User Tools
 Author-email: NSO / AURA <stuart@cadair.com>
 Project-URL: repository, https://github.com/DKISTDC/dkist
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: aiohttp>=3.8
```

### Comparing `dkist-1.5.0/README.rst` & `dkist-1.5.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/changelog/README.rst` & `dkist-1.5.0rc1/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/__init__.py` & `dkist-1.5.0rc1/dkist/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/conftest.py` & `dkist-1.5.0rc1/dkist/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/VISP_HEADER.hdr` & `dkist-1.5.0rc1/dkist/data/VISP_HEADER.hdr`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/api_search_values.json` & `dkist-1.5.0rc1/dkist/data/api_search_values.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984644027729435%*

 * *Differences: {"'parameterValues'": "{0: {'values': {'maxValue': '2024-01-27T16:18:31.564623'}}, 1: {'values': "*

 * *                      "{'maxValue': '2024-01-27T16:18:31.564623'}}, 2: {'values': {'maxValue': "*

 * *                      "'2023-11-01T20:51:20.287000'}}, 3: {'values': {'maxValue': "*

 * *                      "'2023-11-01T20:51:20.287000'}}, 7: {'values': {'minValue': "*

 * *                      "0.027724481746640606}}, 8: {'values': {'minValue': 0.027724481746640606}}, "*

 * *                      "11: {'values': {'maxValue […]*

```diff
@@ -1,34 +1,34 @@
 {
     "parameterValues": [
         {
             "parameterName": "createDateMin",
             "values": {
-                "maxValue": "2024-03-29T08:18:32.313627",
+                "maxValue": "2024-01-27T16:18:31.564623",
                 "minValue": "2022-12-08T19:07:55.038280"
             }
         },
         {
             "parameterName": "createDateMax",
             "values": {
-                "maxValue": "2024-03-29T08:18:32.313627",
+                "maxValue": "2024-01-27T16:18:31.564623",
                 "minValue": "2022-12-08T19:07:55.038280"
             }
         },
         {
             "parameterName": "endTimeMin",
             "values": {
-                "maxValue": "2024-03-27T20:25:51.519000",
+                "maxValue": "2023-11-01T20:51:20.287000",
                 "minValue": "2022-02-23T20:48:55.393500"
             }
         },
         {
             "parameterName": "endTimeMax",
             "values": {
-                "maxValue": "2024-03-27T20:25:51.519000",
+                "maxValue": "2023-11-01T20:51:20.287000",
                 "minValue": "2022-02-23T20:48:55.393500"
             }
         },
         {
             "parameterName": "exposureTimeMin",
             "values": {
                 "maxValue": 1380.2332394366197,
@@ -51,22 +51,22 @@
                 ]
             }
         },
         {
             "parameterName": "qualityAverageFriedParameterMin",
             "values": {
                 "maxValue": 2.6520787500175156e+30,
-                "minValue": 0.01695005847191685
+                "minValue": 0.027724481746640606
             }
         },
         {
             "parameterName": "qualityAverageFriedParameterMax",
             "values": {
                 "maxValue": 2.6520787500175156e+30,
-                "minValue": 0.01695005847191685
+                "minValue": 0.027724481746640606
             }
         },
         {
             "parameterName": "qualityAveragePolarimetricAccuracyMin",
             "values": {
                 "maxValue": 1.3227079486518465,
                 "minValue": 0.7510039715379637
@@ -78,22 +78,22 @@
                 "maxValue": 1.3227079486518465,
                 "minValue": 0.7510039715379637
             }
         },
         {
             "parameterName": "startTimeMin",
             "values": {
-                "maxValue": "2024-03-27T19:29:13.520000",
+                "maxValue": "2023-11-01T19:53:02.868500",
                 "minValue": "2022-02-23T19:05:32.338002"
             }
         },
         {
             "parameterName": "startTimeMax",
             "values": {
-                "maxValue": "2024-03-27T19:29:13.520000",
+                "maxValue": "2023-11-01T19:53:02.868500",
                 "minValue": "2022-02-23T19:05:32.338002"
             }
         },
         {
             "parameterName": "targetTypes",
             "values": {
                 "categoricalValues": [
@@ -146,26 +146,25 @@
                 "minValue": 9.139999999997528
             }
         },
         {
             "parameterName": "highLevelSoftwareVersion",
             "values": {
                 "categoricalValues": [
-                    "Alakai_11.1.0",
-                    "Alakai_6-0",
-                    "Alakai_8-0",
-                    "Alakai_10-0",
-                    "Alakai_7-0",
-                    "Pono_6.1.5",
                     "Pono_2.1.0",
                     "Pono_1.0.0",
                     "Alakai_5-1",
                     "Pono_3.1.0",
                     "Alakai_3-0",
-                    "Alakai_4-0"
+                    "Alakai_4-0",
+                    "Alakai_11.1.0",
+                    "Alakai_6-0",
+                    "Alakai_8-0",
+                    "Alakai_10-0",
+                    "Alakai_7-0"
                 ]
             }
         },
         {
             "parameterName": "workflowName",
             "values": {
                 "categoricalValues": [
@@ -174,66 +173,62 @@
                 ]
             }
         },
         {
             "parameterName": "workflowVersion",
             "values": {
                 "categoricalValues": [
-                    "2.7.4",
-                    "2.10.3",
-                    "1.1.7",
-                    "0.16.0",
-                    "1.1.10",
-                    "2.7.2",
-                    "2.7.0",
+                    "1.4.11",
                     "2.10.1",
                     "2.0.2",
-                    "2.10.12",
                     "2.7.3",
+                    "1.4.1",
                     "1.1.5",
+                    "1.2.0",
+                    "2.10.2",
+                    "2.7.4",
                     "2.6.1",
                     "1.2.1",
                     "2.7.5",
+                    "2.10.3",
+                    "1.1.7",
                     "2.0.1",
+                    "0.16.0",
                     "1.4.8",
-                    "1.8.2",
                     "2.9.0",
-                    "2.10.7",
                     "2.3.1",
                     "2.3.0",
                     "2.10.0",
+                    "1.1.10",
+                    "2.7.2",
                     "1.0.0",
-                    "1.4.11",
-                    "1.4.1",
-                    "1.2.0",
-                    "2.10.2"
+                    "2.7.0"
                 ]
             }
         },
         {
             "parameterName": "headerDataUnitCreationDateMin",
             "values": {
-                "maxValue": "2024-03-29T07:18:09.457000",
+                "maxValue": "2024-01-27T14:17:20.001000",
                 "minValue": "2022-12-08T17:25:51.965000"
             }
         },
         {
             "parameterName": "headerDataUnitCreationDateMax",
             "values": {
-                "maxValue": "2024-03-29T07:18:09.457000",
+                "maxValue": "2024-01-27T14:17:20.001000",
                 "minValue": "2022-12-08T17:25:51.965000"
             }
         },
         {
             "parameterName": "headerVersion",
             "values": {
                 "categoricalValues": [
                     "3.6.0",
                     "4.0.0",
-                    "4.1.1",
                     "3.3.0",
                     "3.0.0",
                     "3.4.0",
                     "3.9.0",
                     "3.5.0",
                     "3.7.1",
                     "3.8.1"
```

### Comparing `dkist-1.5.0/dkist/data/test/5d_gwcs.asdf` & `dkist-1.5.0rc1/dkist/data/test/5d_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/AGLKO-inv.ecsv` & `dkist-1.5.0rc1/dkist/data/test/AGLKO-inv.ecsv`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.000010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.000010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.020010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.020010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.030011_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.030011_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.040010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.040010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.050010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.050010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.060010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.060010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.080010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.080010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.090010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.090010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.100010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.100010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.110010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.110010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/efz20040301.120010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.120010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/EIT/eit_test_dataset.asdf` & `dkist-1.5.0rc1/dkist/data/test/EIT/eit_test_dataset.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/eit_dataset-0.1.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/eit_dataset-0.2.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/eit_dataset-0.3.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.3.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/eit_dataset-1.0.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/eit_dataset-1.1.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/eit_dataset-1.2.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/globus_operation_ls_response.json` & `dkist-1.5.0rc1/dkist/data/test/globus_operation_ls_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/globus_search_response.json` & `dkist-1.5.0rc1/dkist/data/test/globus_search_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/large_visp.asdf.gz` & `dkist-1.5.0rc1/dkist/data/test/large_visp.asdf.gz`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/small_visp/0.fits` & `dkist-1.5.0rc1/dkist/data/test/small_visp/0.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/small_visp/1.fits` & `dkist-1.5.0rc1/dkist/data/test/small_visp/1.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/small_visp/2.fits` & `dkist-1.5.0rc1/dkist/data/test/small_visp/2.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/small_visp/test_visp.asdf` & `dkist-1.5.0rc1/dkist/data/test/small_visp/test_visp.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/test_old_wcs_BRMQY.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_old_wcs_BRMQY.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/dataset.py` & `dkist-1.5.0rc1/dkist/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/loader.py` & `dkist-1.5.0rc1/dkist/dataset/loader.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/tests/test_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/tests/test_load_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_load_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/tests/test_plotting.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/tests/test_tiled_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/tiled_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/dataset/utils.py` & `dkist-1.5.0rc1/dkist/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/converters/dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/converters/file_manager.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/file_manager.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/converters/models.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/converters/tiled_dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/entry_points.py` & `dkist-1.5.0rc1/dkist/io/asdf/entry_points.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/tests/conftest.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/tests/test_dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/tests/test_models.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/asdf/tests/test_tiled_dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/test_tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/dask_utils.py` & `dkist-1.5.0rc1/dkist/io/dask_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/file_manager.py` & `dkist-1.5.0rc1/dkist/io/file_manager.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/level_1_dataset_schema.yaml` & `dkist-1.5.0rc1/dkist/io/level_1_dataset_schema.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/loaders.py` & `dkist-1.5.0rc1/dkist/io/loaders.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/tests/test_file_manager.py` & `dkist-1.5.0rc1/dkist/io/tests/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/io/tests/test_fits.py` & `dkist-1.5.0rc1/dkist/io/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/logger.py` & `dkist-1.5.0rc1/dkist/logger.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/__init__.py` & `dkist-1.5.0rc1/dkist/net/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/attr_walker.py` & `dkist-1.5.0rc1/dkist/net/attr_walker.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/attrs.py` & `dkist-1.5.0rc1/dkist/net/attrs.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/attrs_values.py` & `dkist-1.5.0rc1/dkist/net/attrs_values.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/client.py` & `dkist-1.5.0rc1/dkist/net/client.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/globus/auth.py` & `dkist-1.5.0rc1/dkist/net/globus/auth.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/globus/endpoints.py` & `dkist-1.5.0rc1/dkist/net/globus/endpoints.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/globus/tests/conftest.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/globus/tests/test_auth.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/globus/tests/test_endpoints.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/globus/tests/test_transfer.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/globus/transfer.py` & `dkist-1.5.0rc1/dkist/net/globus/transfer.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/helpers.py` & `dkist-1.5.0rc1/dkist/net/helpers.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/tests/conftest.py` & `dkist-1.5.0rc1/dkist/net/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/tests/strategies.py` & `dkist-1.5.0rc1/dkist/net/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/tests/test_attr_walker.py` & `dkist-1.5.0rc1/dkist/net/tests/test_attr_walker.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/tests/test_attrs.py` & `dkist-1.5.0rc1/dkist/net/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/tests/test_attrs_values.py` & `dkist-1.5.0rc1/dkist/net/tests/test_attrs_values.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/tests/test_client.py` & `dkist-1.5.0rc1/dkist/net/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/net/tests/test_helpers.py` & `dkist-1.5.0rc1/dkist/net/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/tests/generate_aia_dataset.py` & `dkist-1.5.0rc1/dkist/tests/generate_aia_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/tests/generate_eit_test_dataset.py` & `dkist-1.5.0rc1/dkist/tests/generate_eit_test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/tests/generate_eit_tiled_dataset.py` & `dkist-1.5.0rc1/dkist/tests/generate_eit_tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/tests/test_logger.py` & `dkist-1.5.0rc1/dkist/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/utils/_model_to_graphviz.py` & `dkist-1.5.0rc1/dkist/utils/_model_to_graphviz.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/utils/inventory.py` & `dkist-1.5.0rc1/dkist/utils/inventory.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/utils/sysinfo.py` & `dkist-1.5.0rc1/dkist/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/utils/tests/test_inventory.py` & `dkist-1.5.0rc1/dkist/utils/tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/version.py` & `dkist-1.5.0rc1/dkist/version.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/wcs/models.py` & `dkist-1.5.0rc1/dkist/wcs/models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/wcs/tests/test_coupled_compound_model.py` & `dkist-1.5.0rc1/dkist/wcs/tests/test_coupled_compound_model.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist/wcs/tests/test_models.py` & `dkist-1.5.0rc1/dkist/wcs/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/dkist.egg-info/PKG-INFO` & `dkist-1.5.0rc1/dkist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.5.0
+Version: 1.5.0rc1
 Summary: DKIST User Tools
 Author-email: NSO / AURA <stuart@cadair.com>
 Project-URL: repository, https://github.com/DKISTDC/dkist
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: aiohttp>=3.8
```

### Comparing `dkist-1.5.0/dkist.egg-info/SOURCES.txt` & `dkist-1.5.0rc1/dkist.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 tox.ini
 .github/ISSUE_TEMPLATE/BUG_REPORT.md
 .github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/workflows/main.yml
 .github/workflows/prepare-release.yml
 .github/workflows/sub_package_update.yml
+changelog/309.bugfix.rst
+changelog/344.trivial.rst
+changelog/347.feature.rst
+changelog/349.doc.rst
+changelog/361.bugfix.rst
 changelog/README.rst
 dkist/__init__.py
 dkist/_version.py
 dkist/conftest.py
 dkist/dkist.cfg
 dkist/logger.py
 dkist/version.py
```

### Comparing `dkist-1.5.0/dkist.egg-info/requires.txt` & `dkist-1.5.0rc1/dkist.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/Makefile` & `dkist-1.5.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/conf.py` & `dkist-1.5.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/developer.rst` & `dkist-1.5.0rc1/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/howto_guides/reproject_vbi_mosaic.md` & `dkist-1.5.0rc1/docs/howto_guides/reproject_vbi_mosaic.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/index.rst` & `dkist-1.5.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/installation.rst` & `dkist-1.5.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/logo/icon_square.jpg` & `dkist-1.5.0rc1/docs/logo/icon_square.jpg`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/make.bat` & `dkist-1.5.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/reference.rst` & `dkist-1.5.0rc1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/topic_guides/level1data.rst` & `dkist-1.5.0rc1/docs/topic_guides/level1data.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/topic_guides/loading.rst` & `dkist-1.5.0rc1/docs/topic_guides/loading.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/topic_guides/net.rst` & `dkist-1.5.0rc1/docs/topic_guides/net.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/topic_guides/usertools.rst` & `dkist-1.5.0rc1/docs/topic_guides/usertools.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/1_astropy_and_sunpy.md` & `dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/1_astropy_and_sunpy_NOTES.md` & `dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/2_search_and_asdf_download.md` & `dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/2_search_and_asdf_download_NOTES.md` & `dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/3_the_dataset.md` & `dkist-1.5.0rc1/docs/tutorial/3_the_dataset.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/3_the_dataset_NOTES.md` & `dkist-1.5.0rc1/docs/tutorial/3_the_dataset_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/4_more_dataset.md` & `dkist-1.5.0rc1/docs/tutorial/4_more_dataset.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/5_downloading_data.md` & `dkist-1.5.0rc1/docs/tutorial/5_downloading_data.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/6_visualization.md` & `dkist-1.5.0rc1/docs/tutorial/6_visualization.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/tutorial/index.md` & `dkist-1.5.0rc1/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/docs/whatsnew/1.0.rst` & `dkist-1.5.0rc1/docs/whatsnew/1.0.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/pyproject.toml` & `dkist-1.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/pytest.ini` & `dkist-1.5.0rc1/pytest.ini`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0/tox.ini` & `dkist-1.5.0rc1/tox.ini`

 * *Files identical despite different names*

