# Comparing `tmp/cace-2.1.8.tar.gz` & `tmp/cace-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cace-2.1.8.tar", last modified: Fri Mar 15 15:53:08 2024, max compression
+gzip compressed data, was "cace-2.1.9.tar", last modified: Fri Mar 15 16:00:12 2024, max compression
```

## Comparing `cace-2.1.8.tar` & `cace-2.1.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.453106 cace-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.441106 cace-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.441106 cace-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-15 15:52:44.000000 cace-2.1.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-15 15:52:44.000000 cace-2.1.8/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-15 15:52:44.000000 cace-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-15 15:52:44.000000 cace-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-15 15:52:44.000000 cace-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-15 15:52:44.000000 cace-2.1.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-15 15:53:08.453106 cace-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-03-15 15:52:44.000000 cace-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.445106 cace-2.1.8/cace/
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-03-15 15:52:44.000000 cace-2.1.8/cace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-15 15:52:44.000000 cace-2.1.8/cace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-15 15:52:44.000000 cace-2.1.8/cace/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24829 2024-03-15 15:52:44.000000 cace-2.1.8/cace/cace_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    80400 2024-03-15 15:52:44.000000 cace-2.1.8/cace/cace_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.449106 cace-2.1.8/cace/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_calculate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_collate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26066 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_gensim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14386 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_launch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14647 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_makeplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_measure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10773 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47778 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_regenerate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8701 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_simulate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_unused.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    52969 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/cace_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/layout_estimate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/netlist_precheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/safe_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-03-15 15:52:44.000000 cace-2.1.8/cace/common/spiceunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.449106 cace-2.1.8/cace/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-03-15 15:52:44.000000 cace-2.1.8/cace/doc/characterize_help.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25405 2024-03-15 15:52:44.000000 cace-2.1.8/cace/doc/format.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.449106 cace-2.1.8/cace/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1879 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/consoletext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29537 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/editparam.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27947 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/failreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9775 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/helpwindow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5747 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16358 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/simhints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/textreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/tksimpledialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-03-15 15:52:44.000000 cace-2.1.8/cace/gui/tooltip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.453106 cace-2.1.8/cace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-15 15:53:08.000000 cace-2.1.8/cace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-15 15:53:08.000000 cace-2.1.8/cace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:53:08.000000 cace-2.1.8/cace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-15 15:53:08.000000 cace-2.1.8/cace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 15:53:08.000000 cace-2.1.8/cace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 15:53:08.000000 cace-2.1.8/cace.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.449106 cace-2.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-15 15:52:44.000000 cace-2.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-15 15:52:44.000000 cace-2.1.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.449106 cace-2.1.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.449106 cace-2.1.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/_static/cace_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/characterization.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.453106 cace-2.1.8/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/dev/codebase.md
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/dev/coding_style.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/dev/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.453106 cace-2.1.8/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (127)    22353 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/formats/format_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/formats/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/formats/schematic_description.md
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.453106 cace-2.1.8/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/usage/cace_cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/usage/cace_gui.md
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-15 15:52:44.000000 cace-2.1.8/docs/source/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-15 15:52:44.000000 cace-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 15:52:44.000000 cace-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-15 15:52:44.000000 cace-2.1.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-15 15:52:44.000000 cace-2.1.8/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 15:53:08.453106 cace-2.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:53:08.453106 cace-2.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-15 15:52:44.000000 cace-2.1.8/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 15:52:44.000000 cace-2.1.8/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.073902 cace-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.077902 cace-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-15 15:59:50.000000 cace-2.1.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-15 15:59:50.000000 cace-2.1.9/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-15 15:59:50.000000 cace-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-15 15:59:50.000000 cace-2.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-15 15:59:50.000000 cace-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-15 15:59:50.000000 cace-2.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-15 16:00:12.089902 cace-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-03-15 15:59:50.000000 cace-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.077902 cace-2.1.9/cace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-03-15 15:59:50.000000 cace-2.1.9/cace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-15 15:59:50.000000 cace-2.1.9/cace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-15 15:59:50.000000 cace-2.1.9/cace/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24829 2024-03-15 15:59:50.000000 cace-2.1.9/cace/cace_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    80400 2024-03-15 15:59:50.000000 cace-2.1.9/cace/cace_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.081902 cace-2.1.9/cace/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_calculate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_collate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26066 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_gensim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14386 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14647 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_makeplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_measure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10773 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47991 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_regenerate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8701 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_simulate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_unused.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    52969 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/cace_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/layout_estimate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/netlist_precheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/safe_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-03-15 15:59:50.000000 cace-2.1.9/cace/common/spiceunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.081902 cace-2.1.9/cace/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-03-15 15:59:50.000000 cace-2.1.9/cace/doc/characterize_help.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25405 2024-03-15 15:59:50.000000 cace-2.1.9/cace/doc/format.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/cace/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1879 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/consoletext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29537 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/editparam.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27947 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/failreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9775 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/helpwindow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5747 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16358 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/simhints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/textreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/tksimpledialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-03-15 15:59:50.000000 cace-2.1.9/cace/gui/tooltip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/cace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 16:00:12.000000 cace-2.1.9/cace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-15 15:59:50.000000 cace-2.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-15 15:59:50.000000 cace-2.1.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/_static/cace_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/characterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.085902 cace-2.1.9/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/dev/codebase.md
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/dev/coding_style.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/dev/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)    22353 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/formats/format_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/formats/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/formats/schematic_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/cace_cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/cace_gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-15 15:59:50.000000 cace-2.1.9/docs/source/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-15 15:59:50.000000 cace-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-15 15:59:50.000000 cace-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-15 15:59:50.000000 cace-2.1.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-15 15:59:50.000000 cace-2.1.9/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 16:00:12.089902 cace-2.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:00:12.089902 cace-2.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-15 15:59:50.000000 cace-2.1.9/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-15 15:59:50.000000 cace-2.1.9/tests/test1.py
```

### Comparing `cace-2.1.8/.github/workflows/ci.yaml` & `cace-2.1.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/.github/workflows/pypi.yaml` & `cace-2.1.9/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/.readthedocs.yaml` & `cace-2.1.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/LICENSE` & `cace-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/Makefile` & `cace-2.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/PKG-INFO` & `cace-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.1.8
+Version: 2.1.9
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.1.8 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.1.9 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.1.8/README.md` & `cace-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/__init__.py` & `cace-2.1.9/cace/__init__.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/__main__.py` & `cace-2.1.9/cace/__main__.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/__version__.py` & `cace-2.1.9/cace/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '2.1.8'
+__version__ = '2.1.9'
 
 if __name__ == '__main__':
     print(__version__, end='')
```

### Comparing `cace-2.1.8/cace/cace_cli.py` & `cace-2.1.9/cace/cace_cli.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/cace_gui.py` & `cace-2.1.9/cace/cace_gui.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_calculate.py` & `cace-2.1.9/cace/common/cace_calculate.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_collate.py` & `cace-2.1.9/cace/common/cace_collate.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_compat.py` & `cace-2.1.9/cace/common/cace_compat.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_evaluate.py` & `cace-2.1.9/cace/common/cace_evaluate.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_gensim.py` & `cace-2.1.9/cace/common/cace_gensim.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_launch.py` & `cace-2.1.9/cace/common/cace_launch.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_makeplot.py` & `cace-2.1.9/cace/common/cace_makeplot.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_measure.py` & `cace-2.1.9/cace/common/cace_measure.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_read.py` & `cace-2.1.9/cace/common/cace_read.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_regenerate.py` & `cace-2.1.9/cace/common/cace_regenerate.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,15 +859,15 @@
 # 	a primitive, and rely on an include file to pull in the
 # 	netlist (either schematic or layout) from the appropriate
 # 	netlist directory.
 #
 # -----------------------------------------------------------------------
 
 
-def set_xschem_paths(dsheet, tclstr=None):
+def set_xschem_paths(dsheet, symbolpath, tclstr=None):
     paths = dsheet['paths']
 
     # Root path
     if 'root' in paths:
         root_path = paths['root']
     else:
         root_path = '.'
@@ -881,18 +881,19 @@
 
     # Add the root path to the search path (may not be necessary but covers
     # cases where schematics have been specified from the project root for
     # either the testbench or schematic directories, or both).
 
     tcllist.append('append XSCHEM_LIBRARY_PATH :' + os.path.abspath(root_path))
 
-    # Add the schematic path to the search path
-    if 'schematic' in paths:
-        schempath = os.path.join(root_path, paths['schematic'])
-        tcllist.append('append XSCHEM_LIBRARY_PATH :' + schempath)
+    # Add the path with the DUT symbol to the search path.  Note that testbenches
+    # use a version of the DUT symbol that is marked as "primitive" so that it
+    # does not get added to the netlist directly.  The netlist is included by a
+    # ".include" statement in the testbenches.
+    tcllist.append('append XSCHEM_LIBRARY_PATH :' + symbolpath)
 
     # If dependencies are declared, then pull in their locations
     # and add them to the search path as well.
 
     # NOTE:  This depends on the setup of the dependent repository.
     # The code below assumes that there is a subdirectory 'xschem'
     # in the repository.  There needs to be a routine that recursively
@@ -1031,15 +1032,17 @@
 
         newenv = os.environ.copy()
         if pdk_root and 'PDK_ROOT' not in newenv:
             newenv['PDK_ROOT'] = pdk_root
         if pdk and 'PDK' not in newenv:
             newenv['PDK'] = pdk
 
-        tclstr = set_xschem_paths(dsheet, 'set lvs_netlist 1')
+        tclstr = set_xschem_paths(
+            dsheet, schem_netlist_path, 'set lvs_netlist 1'
+        )
 
         # Xschem arguments:
         # -n:  Generate a netlist
         # -s:  Netlist type is SPICE
         # -r:  Bypass readline (because stdin/stdout are piped)
         # -x:  No X11 / No GUI window
         # -q:  Quit after processing command line
@@ -1179,15 +1182,15 @@
 
     newenv = os.environ.copy()
     if pdk_root and 'PDK_ROOT' not in newenv:
         newenv['PDK_ROOT'] = pdk_root
     if pdk and 'PDK' not in newenv:
         newenv['PDK'] = pdk
 
-    tclstr = set_xschem_paths(dsheet, '')
+    tclstr = set_xschem_paths(dsheet, testbenchpath, '')
     xschemargs = ['xschem', '-n', '-s', '-r', '-x', '-q', '--tcl', tclstr]
 
     # Use the PDK xschemrc file for xschem startup
     xschemrcfile = os.path.join(
         pdk_root, pdk, 'libs.tech', 'xschem', 'xschemrc'
     )
     if os.path.isfile(xschemrcfile):
```

### Comparing `cace-2.1.8/cace/common/cace_simulate.py` & `cace-2.1.9/cace/common/cace_simulate.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_unused.txt` & `cace-2.1.9/cace/common/cace_unused.txt`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/cace_write.py` & `cace-2.1.9/cace/common/cace_write.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/layout_estimate.py` & `cace-2.1.9/cace/common/layout_estimate.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/netlist_precheck.py` & `cace-2.1.9/cace/common/netlist_precheck.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/safe_eval.py` & `cace-2.1.9/cace/common/safe_eval.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/common/spiceunits.py` & `cace-2.1.9/cace/common/spiceunits.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/doc/characterize_help.txt` & `cace-2.1.9/cace/doc/characterize_help.txt`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/doc/format.txt` & `cace-2.1.9/cace/doc/format.txt`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/consoletext.py` & `cace-2.1.9/cace/gui/consoletext.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/editparam.py` & `cace-2.1.9/cace/gui/editparam.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/failreport.py` & `cace-2.1.9/cace/gui/failreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/helpwindow.py` & `cace-2.1.9/cace/gui/helpwindow.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/settings.py` & `cace-2.1.9/cace/gui/settings.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/simhints.py` & `cace-2.1.9/cace/gui/simhints.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/textreport.py` & `cace-2.1.9/cace/gui/textreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/tksimpledialog.py` & `cace-2.1.9/cace/gui/tksimpledialog.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace/gui/tooltip.py` & `cace-2.1.9/cace/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/cace.egg-info/PKG-INFO` & `cace-2.1.9/cace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.1.8
+Version: 2.1.9
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.1.8 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.1.9 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.1.8/cace.egg-info/SOURCES.txt` & `cace-2.1.9/cace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/Makefile` & `cace-2.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/make.bat` & `cace-2.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/_static/cace_screenshot.png` & `cace-2.1.9/docs/source/_static/cace_screenshot.png`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/characterization.md` & `cace-2.1.9/docs/source/characterization.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/conf.py` & `cace-2.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/formats/format_description.md` & `cace-2.1.9/docs/source/formats/format_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/formats/schematic_description.md` & `cace-2.1.9/docs/source/formats/schematic_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/index.md` & `cace-2.1.9/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/usage/cace_cli.md` & `cace-2.1.9/docs/source/usage/cace_cli.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/usage/cace_gui.md` & `cace-2.1.9/docs/source/usage/cace_gui.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/docs/source/usage/getting_started.md` & `cace-2.1.9/docs/source/usage/getting_started.md`

 * *Files identical despite different names*

### Comparing `cace-2.1.8/pyproject.toml` & `cace-2.1.9/pyproject.toml`

 * *Files identical despite different names*

