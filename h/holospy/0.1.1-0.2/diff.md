# Comparing `tmp/holospy-0.1.1.tar.gz` & `tmp/holospy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holospy-0.1.1.tar", last modified: Sat Dec  2 16:05:17 2023, max compression
+gzip compressed data, was "holospy-0.2.tar", last modified: Thu Apr  4 16:03:10 2024, max compression
```

## Comparing `holospy-0.1.1.tar` & `holospy-0.2.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.047061 holospy-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.035061 holospy-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.035061 holospy-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1238 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.035061 holospy-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/workflows/package_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-12-02 16:05:02.000000 holospy-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-02 16:05:02.000000 holospy-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-12-02 16:05:02.000000 holospy-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-02 16:05:02.000000 holospy-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2023-12-02 16:05:02.000000 holospy-0.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2023-12-02 16:05:02.000000 holospy-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35155 2023-12-02 16:05:02.000000 holospy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43601 2023-12-02 16:05:17.047061 holospy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-12-02 16:05:02.000000 holospy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.035061 holospy-0.1.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.035061 holospy-0.1.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    18979 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/_static/hyperspy_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.039061 holospy-0.1.1/doc/api/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/api/reconstruct.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/api/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/api/tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/citing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.039061 holospy-0.1.1/doc/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/user_guide/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/user_guide/electron_holography.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.039061 holospy-0.1.1/doc/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)    61567 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/user_guide/images/holography_argand_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)   128508 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/user_guide/images/holography_unwrapped_phase.png
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/user_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-12-02 16:05:02.000000 holospy-0.1.1/doc/user_guide/metadata_structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.039061 holospy-0.1.1/holospy/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.043061 holospy-0.1.1/holospy/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1358560 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)  1353256 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/hyperspy_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.043061 holospy-0.1.1/holospy/signals/
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33985 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/signals/hologram_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.043061 holospy-0.1.1/holospy/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.047061 holospy-0.1.1/holospy/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/tests/signals/test_hologram_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/tests/signals/test_hologram_image_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/tests/test_non-uniform_not-implemented.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2023-12-02 16:05:02.000000 holospy-0.1.1/holospy/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 16:05:17.047061 holospy-0.1.1/holospy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43601 2023-12-02 16:05:16.000000 holospy-0.1.1/holospy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-12-02 16:05:17.000000 holospy-0.1.1/holospy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 16:05:16.000000 holospy-0.1.1/holospy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-02 16:05:16.000000 holospy-0.1.1/holospy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-02 16:05:16.000000 holospy-0.1.1/holospy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-02 16:05:16.000000 holospy-0.1.1/holospy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-12-02 16:05:02.000000 holospy-0.1.1/prepare_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2023-12-02 16:05:02.000000 holospy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-02 16:05:02.000000 holospy-0.1.1/releasing_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 16:05:17.047061 holospy-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.983966 holospy-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.983966 holospy-0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-04 16:02:58.000000 holospy-0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 16:02:58.000000 holospy-0.2/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 16:02:58.000000 holospy-0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1238 2024-04-04 16:02:58.000000 holospy-0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-04 16:02:58.000000 holospy-0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.983966 holospy-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/package_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-04 16:02:58.000000 holospy-0.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 16:02:58.000000 holospy-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 16:02:58.000000 holospy-0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 16:02:58.000000 holospy-0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-04 16:02:58.000000 holospy-0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-04 16:02:58.000000 holospy-0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35155 2024-04-04 16:02:58.000000 holospy-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-04-04 16:03:09.995966 holospy-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-04 16:02:58.000000 holospy-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 16:02:58.000000 holospy-0.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    21844 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy-banner-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    21771 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy-banner-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   103104 2024-04-04 16:02:58.000000 holospy-0.2/doc/_static/holospy.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/reconstruct.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 16:02:58.000000 holospy-0.2/doc/api/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 16:02:58.000000 holospy-0.2/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-04 16:02:58.000000 holospy-0.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 16:02:58.000000 holospy-0.2/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 16:02:58.000000 holospy-0.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-04 16:02:58.000000 holospy-0.2/doc/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 16:02:58.000000 holospy-0.2/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/electron_holography.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/doc/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    61567 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/images/holography_argand_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)   128508 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/images/holography_unwrapped_phase.png
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-04 16:02:58.000000 holospy-0.2/doc/user_guide/metadata_structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.987966 holospy-0.2/holospy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-04 16:02:58.000000 holospy-0.2/holospy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-04 16:02:58.000000 holospy-0.2/holospy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1358560 2024-04-04 16:02:58.000000 holospy-0.2/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)  1353256 2024-04-04 16:02:58.000000 holospy-0.2/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-04 16:02:58.000000 holospy-0.2/holospy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-04 16:02:58.000000 holospy-0.2/holospy/hyperspy_extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-04 16:02:58.000000 holospy-0.2/holospy/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 16:02:58.000000 holospy-0.2/holospy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34208 2024-04-04 16:02:58.000000 holospy-0.2/holospy/signals/hologram_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/signals/test_hologram_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/signals/test_hologram_image_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tests/test_non-uniform_not-implemented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-04 16:02:58.000000 holospy-0.2/holospy/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/holospy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 16:03:09.000000 holospy-0.2/holospy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-04 16:02:58.000000 holospy-0.2/prepare_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-04 16:02:58.000000 holospy-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-04 16:02:58.000000 holospy-0.2/releasing_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:03:09.995966 holospy-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:03:09.995966 holospy-0.2/upcoming_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-04 16:02:58.000000 holospy-0.2/upcoming_changes/README.rst
```

### Comparing `holospy-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `holospy-0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `holospy-0.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/.github/workflows/doc.yml` & `holospy-0.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/.github/workflows/release.yml` & `holospy-0.2/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     runs-on: ubuntu-latest
     name: Upload to pypi
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
     - name: Download dist
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
 
     - name: Display downloaded files
       run: |
         ls -shR
       working-directory: dist
 
     - uses: pypa/gh-action-pypi-publish@release/v1
@@ -48,8 +48,8 @@
     name: Create GitHub Release
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
       - name: Create Release
         if: ${{ startsWith(github.ref, 'refs/tags/') && github.repository_owner == 'hyperspy' }}
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
+        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564
```

### Comparing `holospy-0.1.1/.github/workflows/tests.yml` & `holospy-0.2/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             PYTHON_VERSION: '3.8'
           - os: ubuntu
             PYTHON_VERSION: '3.11'
           - os: ubuntu
             PYTHON_VERSION: '3.12'
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: get repository name
         shell: bash
         run: echo "REPOSITORY_NAME=${GITHUB_REPOSITORY#*/}" >> $GITHUB_ENV
 
@@ -36,15 +36,15 @@
         if: ${{ github.repository_owner != 'hyperspy' }}
         # Needs to fetch the tags from upstream to get the
         # correct version with setuptools_scm
         run: |
           git remote add upstream https://github.com/hyperspy/${{ env.REPOSITORY_NAME }}.git
           git fetch upstream --tags
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: ${{ matrix.PYTHON_VERSION }}
 
       - name: Display version
         run: |
           python --version
@@ -60,10 +60,10 @@
 
       - name: Run test suite
         run: |
           pytest --pyargs holospy --cov=. --cov-report=xml
 
       - name: Upload coverage to Codecov
         if: ${{ always() }}
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `holospy-0.1.1/.readthedocs.yaml` & `holospy-0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/CHANGES.rst` & `holospy-0.2/CHANGES.rst`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,37 @@
 Changelog entries for the development version are available at
 https://holospy.readthedocs.io/en/latest/changes.html
 
 .. towncrier-draft-entries:: |release| [UNRELEASED]
 
 .. towncrier release notes start
 
+0.2 (2024-04-04)
+================
+
+Deprecations
+------------
+
+- The positional arguments ``holo_data`` and ``holo_sampling`` of :func:`~.reconstruct.reconstruct` have been renamed to ``data`` and ``sampling``, respectively. (`#26 <https://github.com/hyperspy/holospy/issues/26>`_)
+
+
+Improved Documentation
+----------------------
+
+- Add holoSpy logo (`#26 <https://github.com/hyperspy/holospy/issues/26>`_)
+
+
+Maintenance
+-----------
+
+- Use ruff for linting and formatting; check NPY2011. (`#28 <https://github.com/hyperspy/holospy/issues/28>`_)
+- Fix numpy 1.25 deprecation. (`#29 <https://github.com/hyperspy/holospy/issues/29>`_)
+- Enable numpydoc and nitpicky; fix docstrings. (`#30 <https://github.com/hyperspy/holospy/issues/30>`_)
+
+
 0.1.1 (2023-12-02)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix getting version from metadata (`#16 <https://github.com/hyperspy/holospy/issues/16>`_)
```

### Comparing `holospy-0.1.1/CONTRIBUTING.rst` & `holospy-0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/LICENSE` & `holospy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/PKG-INFO` & `holospy-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: holospy
-Version: 0.1.1
-Summary: Analysis of (off-axis) holography data with HyperSpy.
+Version: 0.2
+Summary: Analysis of (off-axis) electron holography data with HyperSpy.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -676,57 +676,57 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <http://www.gnu.org/philosophy/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://hyperspy.org/holospy
 Project-URL: Bug Reports, https://github.com/hyperspy/holospy/issues
 Project-URL: Source, https://github.com/hyperspy/holospy
-Keywords: data analysis,microscopy,electron microscopy,Off-axis holography
+Keywords: python,hyperspy,data analysis,microscopy,electron microscopy,electron holography,Off-axis holography,STEM,TEM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.5.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: pydata-sphinx-theme>=0.13; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-favicon; extra == "doc"
 Requires-Dist: sphinxcontrib-towncrier; extra == "doc"
 Requires-Dist: towncrier; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: holospy[doc]; extra == "dev"
 Requires-Dist: holospy[tests]; extra == "dev"
 
 
 [![Tests](https://github.com/hyperspy/holospy/actions/workflows/tests.yml/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/hyperspy/holospy/graph/badge.svg?token=XB1QDTXQ86)](https://codecov.io/gh/hyperspy/holospy)
 [![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![DOI](https://zenodo.org/badge/2233998.svg)](https://zenodo.org/badge/latestdoi/2233998)
 
 **HoloSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the [HyperSpy](https://hyperspy.org) library. It is
 aimed at helping with the analysis of (off-axis) electron holography data.
 
 Go to the documentation for instructions on how to install HoloSpy and start an
 analysis: [Read the docs](https://holospy.readthedocs.io).
```

### Comparing `holospy-0.1.1/doc/Makefile` & `holospy-0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/doc/conf.py` & `holospy-0.2/doc/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 import hyperspy.api as hs
-import numpydoc
-from packaging.version import Version
 
 
 # Set logging level to `ERROR` to avoid exspy warning in documentation
 hs.set_log_level("ERROR")
 
 
 # -- Project information -----------------------------------------------------
@@ -34,29 +32,31 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     # numpydoc is necessary to parse the docstring using sphinx
     # otherwise the nitpicky option will raise many warnings
-    # "numpydoc",
+    "numpydoc",
+    "sphinx_design",
     "sphinx_favicon",
     "sphinx.ext.autodoc",
     "sphinx.ext.githubpages",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinxcontrib.towncrier",
 ]
 
 linkcheck_ignore = [
     "https://onlinelibrary.wiley.com",  # 403 Client Error: Forbidden for url
 ]
 
 intersphinx_mapping = {
     "dask": ("https://docs.dask.org/en/latest", None),
+    "exspy": ("https://hyperspy.org/exspy", None),
     "hyperspy": ("https://hyperspy.org/hyperspy-doc/current/", None),
     "kikuchipy": ("https://kikuchipy.org/en/latest/", None),
     "matplotlib": ("https://matplotlib.org/stable", None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "python": ("https://docs.python.org/3", None),
 }
 
@@ -87,36 +87,41 @@
         {
             "name": "Gitter",
             "url": "https://gitter.im/hyperspy/hyperspy",
             "icon": "fab fa-gitter",
         },
     ],
     "logo": {
-        "image_light": "_static/hyperspy_logo.png",
-        "image_dark": "_static/hyperspy_logo.png",
+        "image_light": "_static/holospy-banner-light.svg",
+        "image_dark": "_static/holospy-banner-dark.svg",
     },
     "header_links_before_dropdown": 6,
 }
 
 # -- Options for sphinx_favicon extension -----------------------------------
 
-favicons = {"rel": "icon", "href": "logo_sq.svg", "type": "image/svg+xml"}
+favicons = [
+    "holospy.ico",
+]
 
 # Check links to API when building documentation
-nitpicky = False
-# Remove when fixed in hyperspy
-nitpick_ignore_regex = [(r"py:.*", r"hyperspy.api.*")]
+nitpicky = True
 
 # -- Options for numpydoc extension -----------------------------------
 
+numpydoc_show_class_members = False
 numpydoc_xref_param_type = True
 numpydoc_xref_ignore = {"type", "optional", "default", "of"}
 
-if Version(numpydoc.__version__) >= Version("1.6.0rc0"):
-    numpydoc_validation_checks = {"all", "ES01", "EX01", "GL02", "GL03", "SA01", "SS06"}
+autoclass_content = "both"
+
+autodoc_default_options = {
+    "show-inheritance": True,
+}
+toc_object_entries_show_parents = "hide"
 
 # -- Options for towncrier_draft extension -----------------------------------
 
 # Options: draft/sphinx-version/sphinx-release
 towncrier_draft_autoversion_mode = "draft"
 towncrier_draft_include_empty = False
 towncrier_draft_working_directory = ".."
```

### Comparing `holospy-0.1.1/doc/make.bat` & `holospy-0.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/doc/user_guide/bibliography.rst` & `holospy-0.2/doc/user_guide/bibliography.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/doc/user_guide/electron_holography.rst` & `holospy-0.2/doc/user_guide/electron_holography.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 Electron Holography
 *******************
 
 HoloSpy provides the user with a signal class which can be used to process
 (off-axis) electron holography data:
 
-* :py:class:`~.signals.hologram_image.HologramImage`
+* :py:class:`~.signals.HologramImage`
 
-It inherits from :external+hyperspy:py:class:`hyperspy._signals.signal2d.Signal2D` class and thus can
+It inherits from :external+hyperspy:py:class:`hyperspy.api.signals.Signal2D` class and thus can
 use all of its functionality. The usage of the class is explained in the
 following sections.
 
-To transform a :external+hyperspy:py:class:`hyperspy._signals.signal2d.Signal2D` (or subclass) into a
-:py:class:`~.signals.hologram_image.HologramImage` use:
+To transform a :external+hyperspy:py:class:`hyperspy.api.signals.Signal2D` (or subclass) into a
+:py:class:`~.signals.HologramImage` use:
 
 .. code-block:: python
 
     >>> im.set_signal_type('hologram')
 
 
 Reconstruction of holograms
@@ -26,18 +26,18 @@
 can be found in literature :ref:`[Gabor1948] <Gabor1948>`,
 :ref:`[Tonomura1999] <Tonomura1999>`,
 :ref:`[McCartney2007] <McCartney2007>`,
 and :ref:`[Joy1993] <Joy1993>`.
 Fourier based reconstruction of off-axis holograms (includes
 finding a side band in FFT, isolating and filtering it, recenter and
 calculate inverse Fourier transform) can be performed using the
-:py:meth:`~.signals.hologram_image.HologramImage.reconstruct_phase` method
-which returns a :external+hyperspy:py:class:`hyperspy._signals.complex_signal2d.ComplexSignal2D` class,
+:py:meth:`~.signals.HologramImage.reconstruct_phase` method
+which returns a :external+hyperspy:py:class:`hyperspy.api.signals.ComplexSignal2D` class,
 containing the reconstructed electron wave.
-The :py:meth:`~.signals.hologram_image.HologramImage.reconstruct_phase` method
+The :py:meth:`~.signals.HologramImage.reconstruct_phase` method
 takes sideband position and size as parameters:
 
 .. code-block:: python
 
     >>> import holospy as holo
     >>> im =  holo.datasets.Fe_needle_hologram()
     >>> wave_image = im.reconstruct_phase(sb_position=(<y>, <x>),
@@ -47,18 +47,18 @@
 
 .. code-block:: python
 
     >>> sb_position = im.estimate_sideband_position(ap_cb_radius=None,
     ...                                             sb='lower')
     >>> sb_size = im.estimate_sideband_size(sb_position)
 
-:py:meth:`~.signals.hologram_image.HologramImage.estimate_sideband_position`
+:py:meth:`~.signals.HologramImage.estimate_sideband_position`
 method searches for maximum of intensity in upper or lower part of FFT pattern
 (parameter ``sb``) excluding the middle area defined by ``ap_cb_radius``.
-:py:meth:`~._signals.hologram_image.HologramImage.estimate_sideband_size` method
+:py:meth:`~.signals.HologramImage.estimate_sideband_size` method
 calculates the radius of the sideband filter as half of the distance to the
 central band which is commonly used for strong phase objects. Alternatively,
 the sideband filter radius can be recalculate as 1/3 of the distance
 (often used for weak phase objects) for example:
 
 .. code-block:: python
 
@@ -75,15 +75,15 @@
     >>> wave_image = im.reconstruct_phase(reference_hologram,
     ...                                   sb_position=sb_position,
     ...                                   sb_size=sb_size)
 
 Using the reconstructed wave, one can access its amplitude and phase (also
 unwrapped phase) using
 ``amplitude`` and ``phase`` properties
-(also the :external+hyperspy:py:meth:`hyperspy._signals.complex_signal.ComplexSignal.unwrapped_phase`
+(also the :external+hyperspy:meth:`hyperspy.api.signals.ComplexSignal.unwrapped_phase`
 method):
 
 .. code-block:: python
 
     >>> wave_image.unwrapped_phase().plot()
 
 .. figure:: images/holography_unwrapped_phase.png
@@ -101,15 +101,15 @@
 
 .. code-block:: python
 
     >>> wave_image = im.reconstruct_phase(reference_hologram,
     ...                                   sb_position=sb_position, sb_size=30,
     ...                                   sb_smoothness=0.05*30,sb_unit='mrad')
 
-Also the :py:meth:`~.signals.hologram_image.HologramImage.reconstruct_phase`
+Also the :py:meth:`~.signals.HologramImage.reconstruct_phase`
 method can output wave images with desired size (shape). By default the shape
 of the original hologram is preserved. Though this leads to oversampling of the
 output wave images, since the information is limited by the size of the
 sideband filter. To avoid oversampling the output shape can be set to the
 diameter of the sideband as follows:
 
 .. code-block:: python
@@ -117,19 +117,19 @@
     >>> out_size = int(2*sb_size.data)
     >>> wave_image = im.reconstruct_phase(reference_hologram,
     ...                                   sb_position=sb_position,
     ...                                   sb_size=sb_size,
     ...                                   output_shape=(out_size, out_size))
 
 Note that the
-:py:meth:`~.signals.hologram_image.HologramImage.reconstruct_phase`
+:py:meth:`~.signals.HologramImage.reconstruct_phase`
 method can be called without parameters, which will cause their automatic
 assignment by
-:py:meth:`~.signals.hologram_image.HologramImage.estimate_sideband_position`
-and :py:meth:`~.signals.hologram_image.HologramImage.estimate_sideband_size`
+:py:meth:`~.signals.HologramImage.estimate_sideband_position`
+and :py:meth:`~.signals.HologramImage.estimate_sideband_size`
 methods. This, however, is not recommended for not experienced users.
 
 .. _holography.stats-label:
 
 Further processing of complex wave and phase
 --------------------------------------------
 Once the complex electron wave reconstructed it :ref:`can be processed the same way as any other complex signal
@@ -147,15 +147,15 @@
   :align: center
 
   Argand diagram of the reconstructed complex wave.
 
 Getting hologram statistics
 ---------------------------
 There are many reasons to have an access to some parameters of holograms which describe the quality of the data.
-:meth:`~.signals.hologram_image.HologramImage.statistics` can be used to calculate carrier frequency,
+:meth:`~.signals.HologramImage.statistics` can be used to calculate carrier frequency,
 fringe spacing and estimate fringe contrast. The method outputs dictionary with the values listed above calculated also
 in different units. In particular fringe spacing is calculated in pixels (fringe sampling) as well as in
 calibrated units. Carrier frequency is calculated in inverse pixels or calibrated units as well as radians.
 Estimation of fringe contrast is either performed by division of standard deviation by mean value of hologram or
 in Fourier space as twice the fraction of amplitude of sideband centre and amplitude of center band (i.e. FFT origin).
 The first method is default and using it requires the fringe field to cover entire field of view; the method is
 highly sensitive to any artifacts in holograms like dud pixels,
@@ -182,8 +182,8 @@
 
 The estimation of fringe spacing using ``'fourier'`` method applies apodization in real space prior calculating FFT.
 By default ``apodization`` parameter is set to ``hanning`` which applies Hanning window. Other options are using either
 ``None`` or ``hamming`` for no apodization or Hamming window. Please note that for experimental conditions
 especially with extreme sampling of fringes and strong contrast variation due to Fresnel effects
 the calculated fringe contrast provides only an estimate and the values may differ strongly depending on apodization.
 
-For further information see documentation of :meth:`~.signals.hologram_image.HologramImage.statistics`.
+For further information see documentation of :meth:`~.signals.HologramImage.statistics`.
```

### Comparing `holospy-0.1.1/doc/user_guide/images/holography_argand_diagram.png` & `holospy-0.2/doc/user_guide/images/holography_argand_diagram.png`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/doc/user_guide/images/holography_unwrapped_phase.png` & `holospy-0.2/doc/user_guide/images/holography_unwrapped_phase.png`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/doc/user_guide/installation.rst` & `holospy-0.2/doc/user_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/doc/user_guide/metadata_structure.rst` & `holospy-0.2/doc/user_guide/metadata_structure.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 HoloSpy metadata structure
 **************************
 
 HoloSpy extends the :external+hyperspy:ref:`HyperSpy metadata structure
 <metadata_structure>`
 with conventions for metadata specific to its signal types. Refer to the
-:external+hyperspy:doc:`HyperSpy metadata documentation <user_guide/metadata_structure>`
+:external+hyperspy:ref:`HyperSpy metadata documentation <metadata_structure>`
 for general metadata fields.
 
 The metadata of any **signal objects** is stored in the `metadata` attribute,
 which has a tree structure. By convention, the node labels are capitalized and
 the ones for leaves are not capitalized. When a leaf contains a quantity that
 is not dimensionless, the units can be given in an extra leaf with the same
 label followed by the ``_units`` suffix.
@@ -45,35 +45,34 @@
                 ├── position
                 └── voltage (V)
 
 
 General
 =======
 
-See `HyperSpy-Metadata-General
-<https://hyperspy.org/hyperspy-doc/current/user_guide/metadata_structure.html#general>`_.
+See :external+hyperspy:ref:`HyperSpy-Metadata-General
+<general-metadata>`.
 
 Sample
 ======
 
-See `HyperSpy-Metadata-Sample
-<https://hyperspy.org/hyperspy-doc/current/user_guide/metadata_structure.html#sample>`_.
+See :external+hyperspy:ref:`HyperSpy-Metadata-Sample
+<sample-metadata>`.
 
 Signal
 ======
 
 signal_type
     type: string
 
     String that describes the type of signal. Currently, the only HoloSpy
     specific signal class is ``hologram``.
 
-See `HyperSpy-Metadata-Signal
-<https://hyperspy.org/hyperspy-doc/current/user_guide/metadata_structure.html#signal>`__
-for additional fields.
+See :external+hyperspy:ref:`HyperSpy-Metadata-Signal <signal-metadata>` for
+additional fields.
 
 Acquisition Instrument
 ======================
 
 TEM
 ===
 
@@ -94,9 +93,8 @@
     plane
 
 voltage
     type: Float
 
     Voltage of electrostatic biprism in volts
 
-See `HyperSpy-Metadata-TEM <https://hyperspy.org/hyperspy-doc/current/user_guide/metadata_structure.html#tem>`_
-	for additional fields.
+See :external+exspy:ref:`eXSpy TEM metadata <source-metadata>` for additional fields.
```

### Comparing `holospy-0.1.1/holospy/__init__.py` & `holospy-0.2/holospy/__init__.py`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/holospy/conftest.py` & `holospy-0.2/holospy/conftest.py`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5` & `holospy-0.2/holospy/data/00_ref_Vbp_130V_0V_bin2_crop.hdf5`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5` & `holospy-0.2/holospy/data/01_holo_Vbp_130V_0V_bin2_crop.hdf5`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/holospy/data/__init__.py` & `holospy-0.2/holospy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/holospy/reconstruct.py` & `holospy-0.2/holospy/reconstruct.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,49 +21,50 @@
 import matplotlib.pyplot as plt
 import logging
 
 _logger = logging.getLogger(__name__)
 
 
 def estimate_sideband_position(
-    holo_data, holo_sampling, central_band_mask_radius=None, sb="lower", high_cf=True
+    data, sampling, central_band_mask_radius=None, sb="lower", high_cf=True
 ):
     """
     Finds the position of the sideband and returns its position.
 
     Parameters
     ----------
-    holo_data: ndarray
+    data : numpy.ndarray
         The data of the hologram.
-    holo_sampling: tuple
+    sampling : tuple
         The sampling rate in both image directions.
-    central_band_mask_radius: float, optional
+    central_band_mask_radius : float, optional
         The aperture radius used to mask out the centerband.
     sb : str, optional
         Chooses which sideband is taken. 'lower', 'upper', 'left', or 'right'.
     high_cf : bool, optional
         If False, the highest carrier frequency allowed for the sideband location is equal to
         half of the Nyquist frequency (Default: True).
 
     Returns
     -------
-    Tuple of the sideband position (y, x), referred to the unshifted FFT.
+    tuple
+        The sideband position (y, x), referred to the unshifted FFT.
     """
     sb_position = (0, 0)
-    f_freq = freq_array(holo_data.shape, holo_sampling)
+    f_freq = freq_array(data.shape, sampling)
     # If aperture radius of centerband is not given, it will be set to 5 % of
     # the Nyquist frequ.:
     if central_band_mask_radius is None:
         central_band_mask_radius = 0.05 * np.max(f_freq)
     # A small aperture masking out the centerband.
     ap_cb = 1.0 - aperture_function(f_freq, central_band_mask_radius, 1e-6)
     if not high_cf:  # Cut out higher frequencies, if necessary:
         ap_cb *= aperture_function(f_freq, np.max(f_freq) / (2 * np.sqrt(2)), 1e-6)
     # Imitates 0:
-    fft_holo = fft2(holo_data) / np.prod(holo_data.shape)
+    fft_holo = fft2(data) / np.prod(data.shape)
     fft_filtered = fft_holo * ap_cb
     # Sideband position in pixels referred to unshifted FFT
     cb_position = (
         fft_filtered.shape[0] // 2,
         fft_filtered.shape[1] // 2,
     )  # cb: center band
     if sb == "lower":
@@ -80,89 +81,89 @@
         fft_sb = abs(fft_filtered[:, cb_position[1] :])
         sb_position = np.unravel_index(fft_sb.argmax(), fft_sb.shape)
         sb_position = np.asarray(np.add(sb_position, (0, cb_position[1])))
     # Return sideband position:
     return sb_position
 
 
-def estimate_sideband_size(sb_position, holo_shape, sb_size_ratio=0.5):
+def estimate_sideband_size(sb_position, shape, sb_size_ratio=0.5):
     """
     Estimates the size of sideband filter
 
     Parameters
     ----------
-    holo_shape : array_like
+    shape : array_like
             Holographic data array
     sb_position : tuple
         The sideband position (y, x), referred to the non-shifted FFT.
     sb_size_ratio : float, optional
         Size of sideband as a fraction of the distance to central band
 
     Returns
     -------
-    sb_size : float
+    float
         Size of sideband filter
 
     """
 
     h = (
         np.array(
             (
                 np.asarray(sb_position) - np.asarray([0, 0]),
-                np.asarray(sb_position) - np.asarray([0, holo_shape[1]]),
-                np.asarray(sb_position) - np.asarray([holo_shape[0], 0]),
-                np.asarray(sb_position) - np.asarray(holo_shape),
+                np.asarray(sb_position) - np.asarray([0, shape[1]]),
+                np.asarray(sb_position) - np.asarray([shape[0], 0]),
+                np.asarray(sb_position) - np.asarray(shape),
             )
         )
         * sb_size_ratio
     )
     return np.min(np.linalg.norm(h, axis=1))
 
 
 def reconstruct(
-    holo_data,
-    holo_sampling,
+    data,
+    sampling,
     sb_size,
     sb_position,
     sb_smoothness,
     output_shape=None,
     plotting=False,
 ):
     """Core function for holographic reconstruction.
 
     Parameters
     ----------
-    holo_data : array_like
+    data : array_like
         Holographic data array
-    holo_sampling : tuple
+    sampling : tuple
         Sampling rate of the hologram in y and x direction.
     sb_size : float
         Size of the sideband filter in pixel.
     sb_position : tuple
         Sideband position in pixel.
-    sb_smoothness: float
+    sb_smoothness : float
         Smoothness of the aperture in pixel.
-    output_shape: tuple, optional
+    output_shape : tuple, optional
         New output shape.
     plotting : bool
         Plots the masked sideband used for reconstruction.
 
     Returns
     -------
-        wav : nparray
-            Reconstructed electron wave
+    numpy.ndarray
+        Reconstructed electron wave
 
     """
 
-    holo_size = holo_data.shape
-    f_sampling = np.divide(1, [a * b for a, b in zip(holo_size, holo_sampling)])
+    holo_size = data.shape
+    f_sampling = np.divide(1, [a * b for a, b in zip(holo_size, sampling)])
 
-    fft_exp = fft2(holo_data) / np.prod(holo_size)
+    fft_exp = fft2(data) / np.prod(holo_size)
 
-    f_freq = freq_array(holo_data.shape, holo_sampling)
+    f_freq = freq_array(data.shape, sampling)
 
     sb_size *= np.mean(f_sampling)
     sb_smoothness *= np.mean(f_sampling)
     aperture = aperture_function(f_freq, sb_size, sb_smoothness)
 
     fft_shifted = np.roll(fft_exp, sb_position[0], axis=0)
     fft_shifted = np.roll(fft_shifted, sb_position[1], axis=1)
@@ -177,25 +178,24 @@
             int(holo_size[0] / 2) - sb_size / np.mean(f_sampling),
             int(holo_size[0] / 2) + sb_size / np.mean(f_sampling),
         )
         axs.set_ylim(
             int(holo_size[1] / 2) - sb_size / np.mean(f_sampling),
             int(holo_size[1] / 2) + sb_size / np.mean(f_sampling),
         )
-        plt.show()
 
     if output_shape is not None:
         y_min = int(holo_size[0] / 2 - output_shape[0] / 2)
         y_max = int(holo_size[0] / 2 + output_shape[0] / 2)
         x_min = int(holo_size[1] / 2 - output_shape[1] / 2)
         x_max = int(holo_size[1] / 2 + output_shape[1] / 2)
 
         fft_aperture = fftshift(fftshift(fft_aperture)[y_min:y_max, x_min:x_max])
 
-    wav = ifft2(fft_aperture) * np.prod(holo_data.shape)
+    wav = ifft2(fft_aperture) * np.prod(data.shape)
 
     return wav
 
 
 def aperture_function(r, apradius, rsmooth):
     """
     A smooth aperture function that decays from apradius-rsmooth to apradius+rsmooth.
@@ -204,33 +204,38 @@
     ----------
     r : ndarray
         Array of input data (e.g. frequencies)
     apradius : float
         Radius (center) of the smooth aperture. Decay starts at apradius - rsmooth.
     rsmooth : float
         Smoothness in halfwidth. rsmooth = 1 will cause a decay from 1 to 0 over 2 pixel.
+
+    Returns
+    -------
+    numpy.ndarray
     """
 
     return 0.5 * (1.0 - np.tanh((abs(r) - apradius) / (0.5 * rsmooth)))
 
 
 def freq_array(shape, sampling):
     """
     Makes up a frequency array.
 
     Parameters
     ----------
     shape : tuple
         The shape of the array.
-    sampling: tuple
+    sampling : tuple
         The sampling rates of the array.
 
     Returns
     -------
-    Array of the frequencies.
+    numpy.ndarray
+        Frequencies
     """
     f_freq_1d_y = np.fft.fftfreq(shape[0], sampling[0])
     f_freq_1d_x = np.fft.fftfreq(shape[1], sampling[1])
     f_freq_mesh = np.meshgrid(f_freq_1d_x, f_freq_1d_y)
     f_freq = np.hypot(f_freq_mesh[0], f_freq_mesh[1])
 
     return f_freq
```

### Comparing `holospy-0.1.1/holospy/signals/__init__.py` & `holospy-0.2/holospy/signals/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with holospy.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Signals to be operated on. The basic unit of data"""
+"""
+Modules containing the HoloSpy signals and their lazy counterparts.
+
+HologramImage
+    For holography data
+LazyHologramImage
+    For holography data processed lazily
+
+"""
 
 from .hologram_image import HologramImage, LazyHologramImage
 
 
 __all__ = [
     "HologramImage",
     "LazyHologramImage",
```

### Comparing `holospy-0.1.1/holospy/signals/hologram_image.py` & `holospy-0.2/holospy/signals/hologram_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,57 +119,57 @@
         if sb_size.axes_manager.navigation_size:
             raise ValueError(
                 "Sideband size dimensions do not match "
                 "neither reference nor hologram dimensions."
             )
         # sb_position navdim=0, therefore map function should not iterate:
         else:
-            sb_size_temp = float(sb_size.data)
+            sb_size_temp = float(sb_size.data[0])
     else:
         sb_size_temp = sb_size.deepcopy()
     return sb_size, sb_size_temp
 
 
-def _estimate_fringe_contrast_statistical(holo):
+def _estimate_fringe_contrast_statistical(signal):
     """
     Estimates average fringe contrast of a hologram using statistical definition:
     V = STD / MEAN.
 
     Parameters
     ----------
-    holo_data: ndarray
-        The data of the hologram.
+    signal : HologramImage
+        The hologram signal.
 
     Returns
     -------
-    Fringe contrast as a float
+    HologramImage
+        Fringe contrast as a float
     """
 
-    axes = holo.axes_manager.signal_axes
+    axes = signal.axes_manager.signal_axes
 
-    return holo.std(axes) / holo.mean(axes)
+    return signal.std(axes) / signal.mean(axes)
 
 
 class HologramImage(Signal2D):
-
     """Signal class for holograms acquired via off-axis electron holography."""
 
     _signal_type = "hologram"
 
     def set_microscope_parameters(
         self, beam_energy=None, biprism_voltage=None, tilt_stage=None
     ):
         """Set the microscope parameters.
 
         If no arguments are given, raises an interactive mode to fill
         the values.
 
         Parameters
         ----------
-        beam_energy: float
+        beam_energy : float
             The energy of the electron beam in keV
         biprism_voltage : float
             In volts
         tilt_stage : float
             In degrees
 
         Examples
@@ -201,27 +201,28 @@
         num_workers=None,
     ):
         """
         Estimates the position of the sideband and returns its position.
 
         Parameters
         ----------
-        ap_cb_radius: float, None
+        ap_cb_radius : float, None
             The aperture radius used to mask out the centerband.
         sb : str, optional
             Chooses which sideband is taken. ``'lower'`` or ``'upper'``
         high_cf : bool, optional
             If False, the highest carrier frequency allowed for the sideband location is equal to
             half of the Nyquist frequency (Default: True).
         %s
         %s
 
         Returns
         -------
-        Signal1D instance of sideband positions (y, x), referred to the unshifted FFT.
+        hyperspy.api.signals.Signal1D
+            Sideband positions (y, x), referred to the unshifted FFT.
 
         Raises
         ------
         NotImplementedError
             If the signal axes are non-uniform axes.
 
         Examples
@@ -237,15 +238,15 @@
             if not axis.is_uniform:
                 raise NotImplementedError(
                     "This operation is not yet implemented for non-uniform energy axes."
                 )
 
         sb_position = self.map(
             estimate_sideband_position,
-            holo_sampling=(
+            sampling=(
                 self.axes_manager.signal_axes[0].scale,
                 self.axes_manager.signal_axes[1].scale,
             ),
             central_band_mask_radius=ap_cb_radius,
             sb=sb,
             high_cf=high_cf,
             show_progressbar=show_progressbar,
@@ -268,22 +269,22 @@
         num_workers=None,
     ):
         """
         Estimates the size of the sideband and returns its size.
 
         Parameters
         ----------
-        sb_position : BaseSignal
+        sb_position : hyperspy.api.signals.BaseSignal
             The sideband position (y, x), referred to the non-shifted FFT.
         %s
         %s
 
         Returns
         -------
-        sb_size : Signal1D
+        hyperspy.api.signals.Signal1D
             Sideband size referred to the unshifted FFT.
 
         Raises
         ------
         NotImplementedError
             If the signal axes are non-uniform axes.
 
@@ -300,15 +301,15 @@
             if not axis.is_uniform:
                 raise NotImplementedError(
                     "This operation is not yet implemented for non-uniform energy axes."
                 )
 
         sb_size = sb_position.map(
             estimate_sideband_size,
-            holo_shape=self.axes_manager.signal_shape[::-1],
+            shape=self.axes_manager.signal_shape[::-1],
             show_progressbar=show_progressbar,
             inplace=False,
             num_workers=num_workers,
             ragged=False,
         )
 
         return sb_size
@@ -332,40 +333,40 @@
         store_parameters=True,
         show_progressbar=False,
         num_workers=None,
     ):
         """Reconstruct electron holograms. Operates on multidimensional
         hyperspy signals. There are several usage schemes:
 
-         * Reconstruct 1d or Nd hologram without reference
-         * Reconstruct 1d or Nd hologram using single reference hologram
-         * Reconstruct Nd hologram using Nd reference hologram (applies each
-           reference to each hologram in Nd stack)
+        * Reconstruct 1d or Nd hologram without reference
+        * Reconstruct 1d or Nd hologram using single reference hologram
+        * Reconstruct Nd hologram using Nd reference hologram (applies each
+          reference to each hologram in Nd stack)
 
         The reconstruction parameters (sb_position, sb_size, sb_smoothness)
         have to be 1d or to have same dimensionality as the hologram.
 
         Parameters
         ----------
-        reference : ndarray, Signal2D, None
+        reference : ndarray, hyperspy.api.signals.Signal2D, None
             Vacuum reference hologram.
-        sb_size : float, ndarray, BaseSignal, None
+        sb_size : float, ndarray, hyperspy.api.signals.BaseSignal, None
             Sideband radius of the aperture in corresponding unit (see
             'sb_unit'). If None, the radius of the aperture is set to 1/3 of
             the distance between sideband and center band.
-        sb_smoothness : float, ndarray, BaseSignal, None
+        sb_smoothness : float, ndarray, hyperspy.api.signals.BaseSignal, None
             Smoothness of the aperture in the same unit as sb_size.
         sb_unit : str, None
             Unit of the two sideband parameters 'sb_size' and 'sb_smoothness'.
             Default: None - Sideband size given in pixels
             'nm': Size and smoothness of the aperture are given in 1/nm.
             'mrad': Size and smoothness of the aperture are given in mrad.
         sb : str, None
             Select which sideband is selected. 'upper' or 'lower'.
-        sb_position : tuple, Signal1D, None
+        sb_position : tuple, hyperspy.api.signals.Signal1D, None
             The sideband position (y, x), referred to the non-shifted FFT. If
             None, sideband is determined automatically from FFT.
         high_cf : bool, optional
             If False, the highest carrier frequency allowed for the sideband
             location is equal to half of the Nyquist frequency (Default: True).
         output_shape: tuple, None
             Choose a new output shape. Default is the shape of the input
@@ -376,15 +377,15 @@
         store_parameters : bool
             Store reconstruction parameters in metadata
         %s
         %s
 
         Returns
         -------
-        wave : ComplexSignal2D
+        hyperspy.api.signals.ComplexSignal2D
             Reconstructed electron wave. By default object wave is divided by
             reference wave.
 
         Raises
         ------
         NotImplementedError
             If the signal axes are non-uniform axes.
@@ -499,15 +500,15 @@
                     "Sideband smoothness dimensions do not match"
                     " neither reference nor hologram "
                     "dimensions."
                 )
             # sb_position navdim=0, therefore map function should not iterate
             # it:
             else:
-                sb_smoothness_temp = float(sb_smoothness.data)
+                sb_smoothness_temp = float(sb_smoothness.data[0])
         else:
             sb_smoothness_temp = sb_smoothness.deepcopy()
 
         # Convert sideband size from 1/nm or mrad to pixels
         if sb_unit == "nm":
             f_sampling = np.divide(
                 1,
@@ -584,15 +585,15 @@
 
         # Reconstructing object electron wave:
 
         # Checking if reference is a single image, which requires sideband
         # parameters as a nparray to avoid iteration trough those:
         wave_object = self.map(
             reconstruct,
-            holo_sampling=(
+            sampling=(
                 self.axes_manager.signal_axes[0].scale,
                 self.axes_manager.signal_axes[1].scale,
             ),
             sb_size=sb_size_temp,
             sb_position=sb_position_temp,
             sb_smoothness=sb_smoothness_temp,
             output_shape=output_shape,
@@ -638,15 +639,15 @@
                 sb_smoothness_ref = float(_first_nav_pixel_data(sb_smoothness_temp))
             else:
                 sb_smoothness_ref = sb_smoothness_temp
             #
 
             wave_reference = reference.map(
                 reconstruct,
-                holo_sampling=(
+                sampling=(
                     self.axes_manager.signal_axes[0].scale,
                     self.axes_manager.signal_axes[1].scale,
                 ),
                 sb_size=sb_size_ref,
                 sb_position=sb_position_ref,
                 sb_smoothness=sb_smoothness_ref,
                 output_shape=output_shape,
@@ -656,15 +657,15 @@
                 num_workers=num_workers,
                 ragged=False,
             )
 
         else:
             wave_reference = reference.map(
                 reconstruct,
-                holo_sampling=(
+                sampling=(
                     self.axes_manager.signal_axes[0].scale,
                     self.axes_manager.signal_axes[1].scale,
                 ),
                 sb_size=sb_size_temp,
                 sb_position=sb_position_temp,
                 sb_smoothness=sb_smoothness_temp,
                 output_shape=output_shape,
@@ -732,50 +733,50 @@
         Fourier space approach (see description of `fringe_contrast_algorithm` parameter)
         2. Fringe sampling (in pixels)
         3. Fringe spacing (in calibrated units)
         4. Carrier frequency (in calibrated units, radians and 1/px)
 
         Parameters
         ----------
-        sb_position : tuple, Signal1D, None
+        sb_position : tuple, hyperspy.api.signals.Signal1D, None
             The sideband position (y, x), referred to the non-shifted FFT.
             It has to be tuple or to have the same dimensionality as the hologram.
             If None, sideband is determined automatically from FFT.
         sb : str, None
             Select which sideband is selected. 'upper', 'lower', 'left' or 'right'.
         high_cf : bool, optional
             If False, the highest carrier frequency allowed for the sideband location is equal to
             half of the Nyquist frequency (Default: False).
         fringe_contrast_algorithm : str
             Select fringe contrast algorithm between:
 
-            * 'fourier': fringe contrast is estimated as 2 * <I(k_0)> / <I(0)>,
+            * ``'fourier'``: fringe contrast is estimated as 2 * <I(k_0)> / <I(0)>,
               where I(k_0) is intensity of sideband and I(0) is the intensity of central band (FFT origin).
               This method delivers also reasonable estimation if the
               interference pattern do not cover full field of view.
-            * 'statistical': fringe contrast is estimated by dividing the
+            * ``'statistical'``: fringe contrast is estimated by dividing the
               standard deviation by the mean of the hologram intensity in real
               space. This algorithm relies on regularly spaced fringes and
               covering the entire field of view.
 
             (Default: 'statistical')
-        apodization: str or None, optional
-            Used with `fringe_contrast_algorithm='fourier'`. If 'hanning' or 'hamming' apodization window
+        apodization : str or None, optional
+            Used with ``fringe_contrast_algorithm='fourier'``. If ``'hanning'`` or ``'hamming'`` apodization window
             will be applied in real space before FFT for estimation of fringe contrast.
             Apodization is typically needed to suppress striking  due to sharp edges of the image,
             which often results in underestimation of the fringe contrast. (Default: 'hanning')
         single_values : bool, optional
             If True calculates statistics only for the first navigation pixels and
             returns the values as single floats (Default: True)
         %s
         %s
 
         Returns
         -------
-        statistics_dict :
+        dict
             Dictionary with the statistics
 
         Raises
         ------
         NotImplementedError
             If the signal axes are non-uniform axes.
 
@@ -933,14 +934,15 @@
             "Carrier frequency (mrad)": carrier_freq_mrad,
         }
 
     statistics.__doc__ %= (SHOW_PROGRESSBAR_ARG, NUM_WORKERS_ARG)
 
 
 class LazyHologramImage(LazySignal, HologramImage):
-
     """
     Lazy signal class for holograms acquired via off-axis electron
     holography.
     """
 
-    __doc__ += LAZYSIGNAL_DOC.replace("__BASECLASS__", "HologramImage")
+    __doc__ += LAZYSIGNAL_DOC.replace("__BASECLASS__", "HologramImage").replace(
+        "hs", "holospy"
+    )
```

### Comparing `holospy-0.1.1/holospy/tests/signals/test_hologram_image.py` & `holospy-0.2/holospy/tests/signals/test_hologram_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     phase_ref_crop = phase_ref[X_START:X_STOP, X_START:X_STOP]
     np.testing.assert_allclose(phase_new_crop, phase_ref_crop, atol=0.02)
 
 
 @pytest.mark.parametrize("lazy", [True, False])
 def test_reconstruct_phase_nonstandard(lazy):
     """Testing reconstruction with non-standard output size for stacked images"""
-    if lazy == True:
+    if lazy:
         pytest.skip("Dask array flags not supported")
     gc.collect()
     x2, z2, y2 = np.meshgrid(LS, np.array([0, 1]), LS)
     phase_ref2 = calc_phaseref(x2, y2, z2, img_size / 2.2, img_size / 2.2)
     holo2 = calc_holo(x2, y2, phase_ref2, FRINGE_SPACING, FRINGE_DIRECTION)
     ref2 = calc_holo(x2, y2, 0, FRINGE_SPACING, FRINGE_DIRECTION)
     holo_image2 = HologramImage(holo2)
@@ -167,16 +167,16 @@
         sb="right",
     )
     np.testing.assert_allclose(sb_position2, sb_position2_left)
     np.testing.assert_allclose(sb_position2_lower, sb_position2_right)
 
     sb_size2 = ref_image2.estimate_sideband_size(sb_position2)
     output_shape = (
-        int(sb_size2.inav[0].data * 2),
-        int(sb_size2.inav[0].data * 2),
+        int(sb_size2.inav[0].data[0] * 2),
+        int(sb_size2.inav[0].data[0] * 2),
     )
 
     wave_image2 = holo_image2.reconstruct_phase(
         reference=ref_image2,
         sb_position=sb_position2,
         sb_size=sb_size2,
         sb_smoothness=sb_size2 * 0.05,
@@ -225,15 +225,15 @@
     phase_ref_crop1 = phase_ref2[1, X_START:X_STOP, X_START:X_STOP]
     np.testing.assert_allclose(phase_new_crop0, phase_ref_crop0, atol=0.05)
     np.testing.assert_allclose(phase_new_crop1, phase_ref_crop1, atol=0.04)
 
 
 @pytest.mark.parametrize("lazy", [True, False])
 def test_reconstruct_phase_multi(lazy):
-    if lazy == True:
+    if lazy:
         pytest.skip("Dask array flags not supported")
     x3, z3, y3 = np.meshgrid(
         np.linspace(-IMG_SIZE3X / 2, IMG_SIZE3X / 2, IMG_SIZE3X),
         np.arange(6),
         np.linspace(-IMG_SIZE3Y / 2, IMG_SIZE3Y / 2, IMG_SIZE3Y),
     )
     phase_ref3 = calc_phaseref(x3, y3, z3 / 6, IMG_SIZE3X * 2, IMG_SIZE3Y * 2)
```

### Comparing `holospy-0.1.1/holospy/tests/signals/test_hologram_image_statistics.py` & `holospy-0.2/holospy/tests/signals/test_hologram_image_statistics.py`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/holospy/tests/test_non-uniform_not-implemented.py` & `holospy-0.2/holospy/tests/test_non-uniform_not-implemented.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with HyperSpy. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 import pytest
 
-from holospy import __version__
 from holospy.signals import HologramImage
 
 
 def test_hologram_image():
     s = HologramImage([[10, 10], [10, 10]])
     s.axes_manager[0].convert_to_non_uniform_axis()
     s.axes_manager[1].convert_to_non_uniform_axis()
```

### Comparing `holospy-0.1.1/holospy/tools.py` & `holospy-0.2/holospy/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,76 +19,78 @@
 import numpy as np
 from scipy.fftpack import fft2
 import logging
 
 _logger = logging.getLogger(__name__)
 
 
-def calculate_carrier_frequency(holo_data, sb_position, scale):
+def calculate_carrier_frequency(data, sb_position, scale):
     """
     Calculates fringe carrier frequency of a hologram
 
     Parameters
     ----------
-    holo_data: ndarray
+    data : numpy.ndarray
         The data of the hologram.
-    sb_position: tuple
+    sb_position : tuple
         Position of the sideband with the reference to non-shifted FFT
-    scale: tuple
+    scale : tuple
         Scale of the axes that will be used for the calculation.
 
     Returns
     -------
-    Carrier frequency
+    numpy.ndarray
+        Carrier frequency
     """
 
-    shape = holo_data.shape
+    shape = data.shape
     origins = [
         np.array((0, 0)),
         np.array((0, shape[1])),
         np.array((shape[0], shape[1])),
         np.array((shape[0], 0)),
     ]
     origin_index = np.argmin(
         [np.linalg.norm(origin - sb_position) for origin in origins]
     )
     return np.linalg.norm(np.multiply(origins[origin_index] - sb_position, scale))
 
 
-def estimate_fringe_contrast_fourier(holo_data, sb_position, apodization="hanning"):
+def estimate_fringe_contrast_fourier(data, sb_position, apodization="hanning"):
     """
     Estimates average fringe contrast of a hologram  by dividing amplitude
     of maximum pixel of sideband by amplitude of FFT's origin.
 
     Parameters
     ----------
-    holo_data: ndarray
+    data : numpy.ndarray
         The data of the hologram.
-    sb_position: tuple
+    sb_position : tuple
         Position of the sideband with the reference to non-shifted FFT
-    apodization: string, None
+    apodization : string, None
         Use 'hanning', 'hamming' or None to apply apodization window in real space before FFT
         Apodization is typically needed to suppress the striking  due to sharp edges
         of the which often results in underestimation of the fringe contrast. (Default: 'hanning')
 
     Returns
     -------
-    Fringe contrast as a float
+    numpy.ndarray
+        Fringe contrast as a float
     """
 
-    holo_shape = holo_data.shape
+    shape = data.shape
 
     if apodization:
         if apodization == "hanning":
-            window_x = np.hanning(holo_shape[0])
-            window_y = np.hanning(holo_shape[1])
+            window_x = np.hanning(shape[0])
+            window_y = np.hanning(shape[1])
         elif apodization == "hamming":
-            window_x = np.hamming(holo_shape[0])
-            window_y = np.hamming(holo_shape[1])
+            window_x = np.hamming(shape[0])
+            window_y = np.hamming(shape[1])
         window_2d = np.sqrt(np.outer(window_x, window_y))
-        data = holo_data * window_2d
+        data = data * window_2d
     else:
-        data = holo_data
+        data = data
 
     fft_exp = fft2(data)
 
     return 2 * abs(fft_exp[tuple(sb_position)]) / abs(fft_exp[0, 0])
```

### Comparing `holospy-0.1.1/holospy.egg-info/PKG-INFO` & `holospy-0.2/holospy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: holospy
-Version: 0.1.1
-Summary: Analysis of (off-axis) holography data with HyperSpy.
+Version: 0.2
+Summary: Analysis of (off-axis) electron holography data with HyperSpy.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -676,57 +676,57 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <http://www.gnu.org/philosophy/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://hyperspy.org/holospy
 Project-URL: Bug Reports, https://github.com/hyperspy/holospy/issues
 Project-URL: Source, https://github.com/hyperspy/holospy
-Keywords: data analysis,microscopy,electron microscopy,Off-axis holography
+Keywords: python,hyperspy,data analysis,microscopy,electron microscopy,electron holography,Off-axis holography,STEM,TEM
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hyperspy>=2.0rc0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.5.0
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: setuptools-scm; extra == "tests"
 Provides-Extra: doc
 Requires-Dist: numpydoc; extra == "doc"
 Requires-Dist: pydata-sphinx-theme>=0.13; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-favicon; extra == "doc"
 Requires-Dist: sphinxcontrib-towncrier; extra == "doc"
 Requires-Dist: towncrier; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: holospy[doc]; extra == "dev"
 Requires-Dist: holospy[tests]; extra == "dev"
 
 
 [![Tests](https://github.com/hyperspy/holospy/actions/workflows/tests.yml/badge.svg)](https://github.com/hyperspy/holospy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/hyperspy/holospy/graph/badge.svg?token=XB1QDTXQ86)](https://codecov.io/gh/hyperspy/holospy)
 [![Docs](https://readthedocs.org/projects/holospy/badge/?version=latest)](https://holospy.readthedocs.io/en/latest/?badge=latest)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![DOI](https://zenodo.org/badge/2233998.svg)](https://zenodo.org/badge/latestdoi/2233998)
 
 **HoloSpy** is a Python package extending the functionality for multi-dimensional
 data analysis provided by the [HyperSpy](https://hyperspy.org) library. It is
 aimed at helping with the analysis of (off-axis) electron holography data.
 
 Go to the documentation for instructions on how to install HoloSpy and start an
 analysis: [Read the docs](https://holospy.readthedocs.io).
```

### Comparing `holospy-0.1.1/holospy.egg-info/SOURCES.txt` & `holospy-0.2/holospy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 CONTRIBUTING.rst
 LICENSE
 README.md
 prepare_release.py
 pyproject.toml
 releasing_guide.md
 .github/PULL_REQUEST_TEMPLATE.md
+.github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/custom.md
 .github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/black.yml
 .github/workflows/doc.yml
 .github/workflows/package_and_test.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 doc/Makefile
 doc/changes.rst
-doc/citing.rst
 doc/conf.py
 doc/contributing.rst
 doc/index.rst
-doc/license.rst
+doc/intro.rst
 doc/make.bat
-doc/_static/hyperspy_logo.png
+doc/_static/holospy-banner-dark.svg
+doc/_static/holospy-banner-light.svg
+doc/_static/holospy-icon.svg
+doc/_static/holospy.ico
 doc/api/data.rst
 doc/api/index.rst
 doc/api/reconstruct.rst
 doc/api/signals.rst
 doc/api/tools.rst
 doc/user_guide/bibliography.rst
 doc/user_guide/electron_holography.rst
@@ -54,8 +56,9 @@
 holospy/data/__init__.py
 holospy/signals/__init__.py
 holospy/signals/hologram_image.py
 holospy/tests/__init__.py
 holospy/tests/test_non-uniform_not-implemented.py
 holospy/tests/signals/__init__.py
 holospy/tests/signals/test_hologram_image.py
-holospy/tests/signals/test_hologram_image_statistics.py
+holospy/tests/signals/test_hologram_image_statistics.py
+upcoming_changes/README.rst
```

### Comparing `holospy-0.1.1/prepare_release.py` & `holospy-0.2/prepare_release.py`

 * *Files identical despite different names*

### Comparing `holospy-0.1.1/pyproject.toml` & `holospy-0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm>=8", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "holospy"
-description = "Analysis of (off-axis) holography data with HyperSpy."
+description = "Analysis of (off-axis) electron holography data with HyperSpy."
 requires-python = ">=3.8"
 readme = "README.md"
 keywords=[
+    "python",
+    "hyperspy",
     "data analysis",
     "microscopy",
     "electron microscopy",
+    "electron holography",
     "Off-axis holography",
+    "STEM",
+    "TEM",
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Topic :: Software Development :: Libraries",
   "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Physics",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+  "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
-  "Operating System :: Microsoft :: Windows",
-  "Operating System :: POSIX",
-  "Operating System :: Unix",
-  "Operating System :: MacOS",
 ]
 dependencies = [
   "hyperspy>=2.0rc0",
   "numpy>=1.20.0",
   "scipy>=1.5.0",
 ]
 dynamic = ["version"]
@@ -49,14 +52,15 @@
   "pytest-cov",
   "setuptools-scm",
 ]
 doc = [
   "numpydoc",
   "pydata-sphinx-theme>=0.13",
   "sphinx",
+  "sphinx-design",
   "sphinx-favicon",
   "sphinxcontrib-towncrier",
   "towncrier",
 ]
 dev = [
   "black",
   "holospy[doc]",
@@ -95,50 +99,24 @@
   "*hdf5",
   "*.yaml"
   ]
 
 [tool.setuptools_scm]
 # Presence enables setuptools_scm, the version will be determine at build time from git
 # The version will be updated by the `prepare_release.py` script
-fallback_version = "0.2.dev0"
+fallback_version = "0.3.dev0"
 
 [tool.towncrier]
-package_dir = "holospy"
-filename = "CHANGES.rst"
 directory = "upcoming_changes/"
-title_format = "{version} ({project_date})"
+filename = "CHANGES.rst"
 issue_format = "`#{issue} <https://github.com/hyperspy/holospy/issues/{issue}>`_"
-
-  [[tool.towncrier.type]]
-  directory = "new"
-  name = "New features"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "bugfix"
-  name = "Bug Fixes"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "doc"
-  name = "Improved Documentation"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "deprecation"
-  name = "Deprecations"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "enhancements"
-  name = "Enhancements"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "api"
-  name = "API changes"
-  showcontent = true
-
-  [[tool.towncrier.type]]
-  directory = "maintenance"
-  name = "Maintenance"
-  showcontent = true
+title_format = "{version} ({project_date})"
+package_dir = "holospy"
+type = [
+    { directory = "new", name = "New features", showcontent = true },
+    { directory = "enhancements", name = "Enhancements", showcontent = true },
+    { directory = "bugfix", name = "Bug Fixes", showcontent = true },
+    { directory = "api", name = "API changes", showcontent = true },
+    { directory = "deprecation", name = "Deprecations", showcontent = true },
+    { directory = "doc", name = "Improved Documentation", showcontent = true },
+    { directory = "maintenance", name = "Maintenance", showcontent = true },
+]
```

### Comparing `holospy-0.1.1/releasing_guide.md` & `holospy-0.2/releasing_guide.md`

 * *Files identical despite different names*

