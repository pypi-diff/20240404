# Comparing `tmp/AlgBench-2.4.0.tar.gz` & `tmp/AlgBench-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgBench-2.4.0.tar", last modified: Tue Nov 14 12:29:18 2023, max compression
+gzip compressed data, was "AlgBench-2.4.1.tar", last modified: Thu Apr  4 16:34:31 2024, max compression
```

## Comparing `AlgBench-2.4.0.tar` & `AlgBench-2.4.1.tar`

### file list

```diff
@@ -1,79 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.694502 AlgBench-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-14 12:29:09.000000 AlgBench-2.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.682502 AlgBench-2.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.686502 AlgBench-2.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-11-14 12:29:09.000000 AlgBench-2.4.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-11-14 12:29:09.000000 AlgBench-2.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2023-11-14 12:29:09.000000 AlgBench-2.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-11-14 12:29:09.000000 AlgBench-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-11-14 12:29:09.000000 AlgBench-2.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-14 12:29:09.000000 AlgBench-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2023-11-14 12:29:18.694502 AlgBench-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24652 2023-11-14 12:29:09.000000 AlgBench-2.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.686502 AlgBench-2.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/algbench.db.rst
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/algbench.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/algbench.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-14 12:29:09.000000 AlgBench-2.4.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.682502 AlgBench-2.4.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/examples/graph_coloring/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/00_generate_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/01_instances.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/02_run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/algbench.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/env_info/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/results/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
--rw-r--r--   0 runner    (1001) docker     (127)    36423 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/04_check_results.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/05_process_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/06_simplified_results.json.zip
--rw-r--r--   0 runner    (1001) docker     (127)    15837 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/07_analyze_mean.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1072992 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/08_analyze_runtime.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   397345 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/09_analyze_quality.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/examples/graph_coloring/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-14 12:29:09.000000 AlgBench-2.4.0/examples/graph_coloring/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2023-11-14 12:29:09.000000 AlgBench-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-14 12:29:09.000000 AlgBench-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 12:29:18.694502 AlgBench-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.682502 AlgBench-2.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/src/AlgBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2023-11-14 12:29:18.000000 AlgBench-2.4.0/src/AlgBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-11-14 12:29:18.000000 AlgBench-2.4.0/src/AlgBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 12:29:18.000000 AlgBench-2.4.0/src/AlgBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-14 12:29:18.000000 AlgBench-2.4.0/src/AlgBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-14 12:29:18.000000 AlgBench-2.4.0/src/AlgBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.690502 AlgBench-2.4.0/src/algbench/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/_stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/benchmark_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.694502 AlgBench-2.4.0/src/algbench/db/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/db/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/db/nfs_json_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/db/nfs_json_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/db/nfs_json_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.694502 AlgBench-2.4.0/src/algbench/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2023-11-14 12:29:09.000000 AlgBench-2.4.0/src/algbench/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 12:29:18.694502 AlgBench-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-11-14 12:29:09.000000 AlgBench-2.4.0/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-11-14 12:29:09.000000 AlgBench-2.4.0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-14 12:29:09.000000 AlgBench-2.4.0/tests/test_extensive.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-14 12:29:09.000000 AlgBench-2.4.0/tests/test_file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-14 12:29:09.000000 AlgBench-2.4.0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.135091 AlgBench-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 16:34:23.000000 AlgBench-2.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.119091 AlgBench-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.123091 AlgBench-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-04 16:34:23.000000 AlgBench-2.4.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 16:34:23.000000 AlgBench-2.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-04 16:34:23.000000 AlgBench-2.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-04 16:34:23.000000 AlgBench-2.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-04 16:34:23.000000 AlgBench-2.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 16:34:23.000000 AlgBench-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25326 2024-04-04 16:34:31.135091 AlgBench-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24699 2024-04-04 16:34:23.000000 AlgBench-2.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.123091 AlgBench-2.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/algbench.db.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/algbench.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/algbench.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 16:34:23.000000 AlgBench-2.4.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.119091 AlgBench-2.4.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.127091 AlgBench-2.4.1/examples/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/00_generate_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/01_instances.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/02_run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.127091 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/algbench.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.127091 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.127091 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/env_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.127091 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    36423 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/04_check_results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/05_process_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/06_simplified_results.json.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    15837 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/07_analyze_mean.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1072992 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/08_analyze_runtime.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   397345 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/09_analyze_quality.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.127091 AlgBench-2.4.1/examples/graph_coloring/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/graph_coloring/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.131091 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/run_evaluation_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/run_evaluation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/run_evaluation_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/run_evaluation_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-04 16:34:23.000000 AlgBench-2.4.1/examples/gurobi_tsp_with_slurminade/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-04 16:34:23.000000 AlgBench-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 16:34:23.000000 AlgBench-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:34:31.135091 AlgBench-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.119091 AlgBench-2.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.135091 AlgBench-2.4.1/src/AlgBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25326 2024-04-04 16:34:31.000000 AlgBench-2.4.1/src/AlgBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-04 16:34:31.000000 AlgBench-2.4.1/src/AlgBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:34:31.000000 AlgBench-2.4.1/src/AlgBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 16:34:31.000000 AlgBench-2.4.1/src/AlgBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 16:34:31.000000 AlgBench-2.4.1/src/AlgBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.131091 AlgBench-2.4.1/src/algbench/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/benchmark_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.131091 AlgBench-2.4.1/src/algbench/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/db/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/db/nfs_json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/db/nfs_json_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/db/nfs_json_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.131091 AlgBench-2.4.1/src/algbench/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-04 16:34:23.000000 AlgBench-2.4.1/src/algbench/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:34:31.135091 AlgBench-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-04 16:34:23.000000 AlgBench-2.4.1/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-04 16:34:23.000000 AlgBench-2.4.1/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 16:34:23.000000 AlgBench-2.4.1/tests/test_extensive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-04 16:34:23.000000 AlgBench-2.4.1/tests/test_file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-04 16:34:23.000000 AlgBench-2.4.1/tests/test_fingerprinting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-04 16:34:23.000000 AlgBench-2.4.1/tests/test_logger.py
```

### Comparing `AlgBench-2.4.0/.github/workflows/pytest.yml` & `AlgBench-2.4.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/.github/workflows/release.yml` & `AlgBench-2.4.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/.gitignore` & `AlgBench-2.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/.pre-commit-config.yaml` & `AlgBench-2.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/LICENSE` & `AlgBench-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/PKG-INFO` & `AlgBench-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 2.4.0
+Version: 2.4.1
 Summary: Util for benchmarking algorithms.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/AlgBench
 Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -641,14 +641,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.4.1** Fixes bug when path ends with `/`.
 - **2.4.0** Removing information on installed packages due to deprecated ``pkg_resources``. New apply-function.
 - **2.2.2** Fixing problem with Jupyter notebooks, because they may not have a ``__file__`` attribute.
 - **2.2.1** Should be able to deal with corrupt zip files now.
 - **2.2.0** Allowing to skip entries in ``read_as_pandas`` by returning a None for the row.
 - **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
```

### Comparing `AlgBench-2.4.0/README.rst` & `AlgBench-2.4.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -624,14 +624,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.4.1** Fixes bug when path ends with `/`.
 - **2.4.0** Removing information on installed packages due to deprecated ``pkg_resources``. New apply-function.
 - **2.2.2** Fixing problem with Jupyter notebooks, because they may not have a ``__file__`` attribute.
 - **2.2.1** Should be able to deal with corrupt zip files now.
 - **2.2.0** Allowing to skip entries in ``read_as_pandas`` by returning a None for the row.
 - **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
```

### Comparing `AlgBench-2.4.0/docs/Makefile` & `AlgBench-2.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/docs/algbench.db.rst` & `AlgBench-2.4.1/docs/algbench.db.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/docs/algbench.rst` & `AlgBench-2.4.1/docs/algbench.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/docs/conf.py` & `AlgBench-2.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/docs/make.bat` & `AlgBench-2.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/00_generate_instances.py` & `AlgBench-2.4.1/examples/graph_coloring/00_generate_instances.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/02_run_benchmark.py` & `AlgBench-2.4.1/examples/graph_coloring/02_run_benchmark.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py` & `AlgBench-2.4.1/examples/graph_coloring/02b_run_benchmark_with_slurminade.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/04_check_results.ipynb` & `AlgBench-2.4.1/examples/graph_coloring/04_check_results.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/05_process_results.py` & `AlgBench-2.4.1/examples/graph_coloring/05_process_results.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/07_analyze_mean.ipynb` & `AlgBench-2.4.1/examples/graph_coloring/07_analyze_mean.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/08_analyze_runtime.ipynb` & `AlgBench-2.4.1/examples/graph_coloring/08_analyze_runtime.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/09_analyze_quality.ipynb` & `AlgBench-2.4.1/examples/graph_coloring/09_analyze_quality.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/README.md` & `AlgBench-2.4.1/examples/graph_coloring/README.md`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/examples/graph_coloring/_utils/__init__.py` & `AlgBench-2.4.1/examples/graph_coloring/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/pyproject.toml` & `AlgBench-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/src/AlgBench.egg-info/PKG-INFO` & `AlgBench-2.4.1/src/AlgBench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 2.4.0
+Version: 2.4.1
 Summary: Util for benchmarking algorithms.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/AlgBench
 Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -641,14 +641,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.4.1** Fixes bug when path ends with `/`.
 - **2.4.0** Removing information on installed packages due to deprecated ``pkg_resources``. New apply-function.
 - **2.2.2** Fixing problem with Jupyter notebooks, because they may not have a ``__file__`` attribute.
 - **2.2.1** Should be able to deal with corrupt zip files now.
 - **2.2.0** Allowing to skip entries in ``read_as_pandas`` by returning a None for the row.
 - **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
```

### Comparing `AlgBench-2.4.0/src/AlgBench.egg-info/SOURCES.txt` & `AlgBench-2.4.1/src/AlgBench.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docs/algbench.db.rst
 docs/algbench.rst
 docs/algbench.utils.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/modules.rst
+docs/requirements.txt
 examples/graph_coloring/00_generate_instances.py
 examples/graph_coloring/01_instances.zip
 examples/graph_coloring/02_run_benchmark.py
 examples/graph_coloring/02b_run_benchmark_with_slurminade.py
 examples/graph_coloring/04_check_results.ipynb
 examples/graph_coloring/05_process_results.py
 examples/graph_coloring/06_simplified_results.json.zip
@@ -29,14 +30,21 @@
 examples/graph_coloring/README.md
 examples/graph_coloring/requirements.txt
 examples/graph_coloring/03_benchmark_data/algbench.json
 examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
 examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
 examples/graph_coloring/03_benchmark_data/results/_compressed.zip
 examples/graph_coloring/_utils/__init__.py
+examples/gurobi_tsp_with_slurminade/README.md
+examples/gurobi_tsp_with_slurminade/instances.py
+examples/gurobi_tsp_with_slurminade/run_evaluation_v0.py
+examples/gurobi_tsp_with_slurminade/run_evaluation_v1.py
+examples/gurobi_tsp_with_slurminade/run_evaluation_v2.py
+examples/gurobi_tsp_with_slurminade/run_evaluation_v3.py
+examples/gurobi_tsp_with_slurminade/solver.py
 src/AlgBench.egg-info/PKG-INFO
 src/AlgBench.egg-info/SOURCES.txt
 src/AlgBench.egg-info/dependency_links.txt
 src/AlgBench.egg-info/requires.txt
 src/AlgBench.egg-info/top_level.txt
 src/algbench/__init__.py
 src/algbench/_stream_utils.py
@@ -53,8 +61,9 @@
 src/algbench/db/nfs_json_set.py
 src/algbench/utils/__init__.py
 src/algbench/utils/timer.py
 tests/test_apply.py
 tests/test_basics.py
 tests/test_extensive.py
 tests/test_file_splitting.py
+tests/test_fingerprinting.py
 tests/test_logger.py
```

### Comparing `AlgBench-2.4.0/src/algbench/__init__.py` & `AlgBench-2.4.1/src/algbench/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/src/algbench/_stream_utils.py` & `AlgBench-2.4.1/src/algbench/_stream_utils.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/src/algbench/benchmark.py` & `AlgBench-2.4.1/src/algbench/benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import inspect
 import logging
 import sys
 import traceback
 import typing
 import os
 from contextlib import ExitStack, redirect_stderr, redirect_stdout
-
+from pathlib import Path
 import yaml
 
 from ._stream_utils import NotSavingIO, PrintingStringIO, StreamWithTime
 from .benchmark_db import BenchmarkDb
 from .db.json_serializer import to_json
 from .fingerprint import fingerprint
 from .log_capture import JsonLogCapture, JsonLogHandler
@@ -270,15 +270,15 @@
         NOT THREAD-SAFE!
         """
         self._db.clear()
 
     def delete_if(self, condition: typing.Callable[[typing.Dict], bool]):
         """
         Delete entries if a specific condition is met (return True).
-        Recreates the internal 'results' folder for this porpose. 
+        Recreates the internal 'results' folder for this porpose.
         Use `front` to get a preview on how an entry that is
         passed to the condition looks like.
 
         NOT THREAD-SAFE!
         """
 
         def func(entry) -> typing.Optional[typing.Dict]:
@@ -287,34 +287,34 @@
                 return None
             return entry
 
         self.apply(func)
 
     def apply(self, func: typing.Callable[[typing.Dict], typing.Optional[typing.Dict]]):
         """
-        Allows to modify all entries (in place !) inside this benchmark, 
+        Allows to modify all entries (in place !) inside this benchmark,
         based on the provided callable. It is being called for every
-        entry inside the database, and the returned entry will be stored 
+        entry inside the database, and the returned entry will be stored
         instead. If None is returned, the provided entry will be deleted
-        from the database. 
+        from the database.
 
         NOT THREAD-SAFE, execute this while no other instance is accessing
-        the file system. 
+        the file system.
         """
         old_db = self._db
-        original_path = old_db.path
+        original_path = Path(old_db.path)
 
         timestamp = datetime.datetime.now().strftime("%Y%m%d%H%M")
         i = 0
-        new_path = f"{original_path}{timestamp}-{i}"
+        new_path = original_path.parent/f"{timestamp}-{i}"
         while os.path.exists(new_path):
-            i+=1
-            new_path = f"{original_path}{timestamp}-{i}"
-        
-        old_db.move_database(new_path)
+            i += 1
+            new_path = original_path.parent/f"{timestamp}-{i}"
+
+        old_db.move_database(str(new_path))
         self._db = BenchmarkDb(original_path)
 
         for entry in old_db:
             new_entry = func(entry)
             if new_entry:
                 self.insert(new_entry)
 
@@ -326,13 +326,24 @@
         Return the number of fingerprints in the database.
         It is possible that this does not correspond to the
         number of entries. Use `__iter__` to iterate over
         all entries and count them to get the number of entries.
         However, this is not recommended, as it is slow.
         """
         return self._db.__len__()
-    
+
     def empty(self):
         """
         Return True if the database is empty, False otherwise.
         """
         return len(self) == 0
+
+    def fingerprint(self):
+        """
+        Returns a fingerprint over all data contained in this benchmark.
+        Two fingerprints should be matching exactly if the benchmark contains the same
+        data, including timestamps etc., no matter the internal structure like order
+        of entries and possible compression.
+        """
+        hashes = [fingerprint(entry) for entry in self]
+        hashes.sort()
+        return fingerprint(hashes)
```

### Comparing `AlgBench-2.4.0/src/algbench/benchmark_db.py` & `AlgBench-2.4.1/src/algbench/benchmark_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,40 +78,42 @@
     def _create_entry_with_env(self, entry):
         entry = entry.copy()
         try:
             entry["env"] = self.get_env_info(entry["env_fingerprint"])
             return entry
         except KeyError:
             return None
-        
+
     def __iter__(self):
         for entry in self._data:
             entry_with_env = self._create_entry_with_env(entry)
             if entry_with_env:
                 yield entry_with_env
 
     def front(self) -> typing.Optional[typing.Dict]:
         try:
             return next(self.__iter__())
         except StopIteration:
             return None
 
     def __len__(self):
         return len(self._arg_fingerprints)
-    
+
     def move_database(self, new_path: str):
         """
-        Moves the entire database to a new directory, keeping all entries. 
-        THIS OPERATION IS NOT THREAD-SAFE, especially not regarding other 
+        Moves the entire database to a new directory, keeping all entries.
+        THIS OPERATION IS NOT THREAD-SAFE, especially not regarding other
         nodes or instances of this script. Other instances will not be notified
-        that the base directory has changed! 
+        that the base directory has changed!
         """
 
         if os.path.exists(new_path) or os.path.isfile(new_path):
             msg = f"Error while moving database to {new_path}: There exists an equally named file or folder"
             raise RuntimeError(msg)
         shutil.move(self.path, new_path)
 
         self.path = new_path
-        self._arg_fingerprints.set_new_directory(os.path.join(new_path, "arg_fingerprints"))
+        self._arg_fingerprints.set_new_directory(
+            os.path.join(new_path, "arg_fingerprints")
+        )
         self._data.set_new_directory(os.path.join(new_path, "results"))
-        self._env_data.set_new_directory(os.path.join(new_path, "env_info"))
+        self._env_data.set_new_directory(os.path.join(new_path, "env_info"))
```

### Comparing `AlgBench-2.4.0/src/algbench/db/json_serializer.py` & `AlgBench-2.4.1/src/algbench/db/json_serializer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/src/algbench/db/nfs_json_dict.py` & `AlgBench-2.4.1/src/algbench/db/nfs_json_dict.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,10 +58,10 @@
 
     def delete(self):
         self._db.delete()
 
     def set_new_directory(self, new_path: str):
         """
         NOT THREAD-SAFE! Does not check the new path, just
-        silently continues working in the new given directory. 
+        silently continues working in the new given directory.
         """
-        self._db.set_new_directory(new_path)
+        self._db.set_new_directory(new_path)
```

### Comparing `AlgBench-2.4.0/src/algbench/db/nfs_json_list.py` & `AlgBench-2.4.1/src/algbench/db/nfs_json_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 import os.path
 import pathlib
 import random
 import shutil
 import socket
 import typing
 import zipfile
-from zipfile import ZipFile, BadZipFile
+from zipfile import BadZipFile, ZipFile
 
 from .json_serializer import to_json
 
 _log = logging.getLogger("AlgBench")
 
 
 class NfsJsonList:
     """
     A simple database to dump data (dictionaries) into. Should be reasonably threadsafe
     even for slurm pools with NFS.
     """
 
-    def __init__(self, path: typing.Union[str, pathlib.Path], file_split_mb: float=30):
+    def __init__(
+        self, path: typing.Union[str, pathlib.Path], file_split_mb: float = 30
+    ):
         self.path: typing.Union[str, pathlib.Path] = path
         if not os.path.exists(path):
             # Could fail in very few unlucky cases on an NFS (parallel creations)
             os.makedirs(path, exist_ok=True)
             _log.info(f"Created new database '{path}'.")
         if os.path.isfile(path):
             msg = f"Cannot create database {path} because there exists an equally named file."
@@ -68,14 +70,15 @@
                 if os.path.getsize(path) <= 0:
                     _log.warning(f"Skipping '{path}' due to zero size.")
                     continue
                 _log.info(f"Compressing '{file_name}' of size {os.path.getsize(path)}.")
                 z.write(path, file_name)
                 os.remove(path)
         _log.info(f"Compressed database has size {os.path.getsize(compr_path)}.")
+        self._new_data_file()
 
     def extend(self, entries: typing.List, flush=True):
         _log.info(f"Adding {len(entries)} items to database.")
         serialized_data = [to_json(e) for e in entries]
         self._cache += serialized_data
         if flush:
             self.flush()
@@ -96,24 +99,30 @@
                 self._filesize += len(data)
             if os.path.getsize(path) <= 0:
                 msg = "Could not write to disk. Resulting file has zero size."
                 raise RuntimeError(msg)
             if not os.path.isfile(path):
                 msg = "Could not write to disk for unknown reasons."
                 raise RuntimeError(msg)
-            
+
             if self._filesize > self._file_split_size:
-                new_unique_name = self._get_unique_name()
-                _log.info(f"File {self._subfile_path} exceeds {self._file_split_size} MB, starting new file {new_unique_name}.")
-                self._subfile_path = new_unique_name
-                self._filesize = 0
-            
+                _log.info(
+                    f"File {self._subfile_path} exceeds {self._file_split_size} MB."
+                )
+                self._new_data_file()
+
         _log.info(f"Wrote {len(self._cache)} entries to disk.")
         self._cache.clear()
 
+    def _new_data_file(self):
+        new_unique_name = self._get_unique_name()
+        _log.info(f"Start writing into new file {new_unique_name}.")
+        self._subfile_path = new_unique_name
+        self._filesize = 0
+
     def iter_cache(self):
         yield from self._cache
 
     def iter_compressed(self):
         """
         Iterate over all entries in the compressed database.
         This may not represent the whole database if the database is not completely compressed.
@@ -188,13 +197,13 @@
 
     def delete(self):
         self._cache.clear()
         shutil.rmtree(self.path)
 
     def set_new_directory(self, new_path: str):
         """
-        Not thread safe. Does not check the new path 
-        and does not move any folders on its own. It is expected 
-        that this step has already been performed. 
+        Not thread safe. Does not check the new path
+        and does not move any folders on its own. It is expected
+        that this step has already been performed.
         """
         _log.info(f"New database path being set to {new_path} (was {self.path}).")
-        self.path = new_path
+        self.path = new_path
```

### Comparing `AlgBench-2.4.0/src/algbench/db/nfs_json_set.py` & `AlgBench-2.4.1/src/algbench/db/nfs_json_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
 
     def __len__(self):
         return len(self._values)
 
     def set_new_directory(self, new_path: str):
         """
         NOT THREAD-SAFE. Does not check the new path, just
-        silently continues working in the new given directory. 
+        silently continues working in the new given directory.
         """
-        self._db.set_new_directory(new_path)
+        self._db.set_new_directory(new_path)
```

### Comparing `AlgBench-2.4.0/src/algbench/environment.py` & `AlgBench-2.4.1/src/algbench/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             .strip()
             .decode("ascii")
         )
     except subprocess.CalledProcessError:
         label = None
     return label
 
+
 def get_python_file() -> typing.Optional[str]:
     """
     Return the path of the calling python file.
     """
     try:
         label = __main__.__file__
     except AttributeError:
@@ -51,19 +52,19 @@
     __cached = {
         "hostname": socket.gethostname(),
         "python_version": sys.version,
         "python": sys.executable,
         "cwd": Path.cwd(),
         # Unfortunately deprecated.
         # Looking for a replacement.
-        #"environment": [
+        # "environment": [
         #    {
         #        "name": str(pkg.project_name),
         #        "path": str(pkg.location),
         #        "version": str(pkg.parsed_version),
         #    }
         #    for pkg in pkg_resources.working_set
-        #],
+        # ],
         "git_revision": get_git_revision(),
         "python_file": get_python_file(),
     }
     return __cached
```

### Comparing `AlgBench-2.4.0/src/algbench/log_capture.py` & `AlgBench-2.4.1/src/algbench/log_capture.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/src/algbench/pandas.py` & `AlgBench-2.4.1/src/algbench/pandas.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/src/algbench/utils/timer.py` & `AlgBench-2.4.1/src/algbench/utils/timer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/tests/test_apply.py` & `AlgBench-2.4.1/tests/test_apply.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,78 @@
-import os
 import typing
+
 from algbench import Benchmark
 
-def test_apply():
 
+def test_apply():
     benchmark = Benchmark("./test_apply")
 
-    def generate_entry(args): 
-        return {"entry_index" : args["index"], "data" : f"Data for entry {args['index']}"}
+    def generate_entry(args):
+        return {"entry_index": args["index"], "data": f"Data for entry {args['index']}"}
+
     for i in range(20):
-        benchmark.add(generate_entry, {"index" : i})
-    
+        benchmark.add(generate_entry, {"index": i})
+
     benchmark.compress()
 
     def db_count_entries(b: Benchmark) -> int:
         return len([0 for _ in b])
 
     assert db_count_entries(benchmark) == 20
 
+    def func(entry: typing.Dict):
+        if entry["result"]["entry_index"] % 2 == 1:
+            return None
+        else:
+            del entry["timestamp"]
+            del entry["runtime"]
+            return entry
+
+    benchmark.apply(func)
+
+    assert db_count_entries(benchmark) == 10
+
+    for entry in benchmark:
+        assert "timestamp" not in entry
+        assert "result" in entry
+
+    benchmark.repair()  # implies both a delete_if() and apply() call
+    assert db_count_entries(benchmark) == 10
+
+    benchmark.delete()
+
+def test_apply_2():
+    benchmark = Benchmark("./test_apply_2/")
+
+    def generate_entry(args):
+        return {"entry_index": args["index"], "data": f"Data for entry {args['index']}"}
+
+    for i in range(20):
+        benchmark.add(generate_entry, {"index": i})
+
+    benchmark.compress()
+
+    def db_count_entries(b: Benchmark) -> int:
+        return len([0 for _ in b])
+
+    assert db_count_entries(benchmark) == 20
 
     def func(entry: typing.Dict):
         if entry["result"]["entry_index"] % 2 == 1:
             return None
         else:
             del entry["timestamp"]
             del entry["runtime"]
             return entry
+
     benchmark.apply(func)
 
     assert db_count_entries(benchmark) == 10
 
     for entry in benchmark:
         assert "timestamp" not in entry
         assert "result" in entry
 
-    benchmark.repair() # implies both a delete_if() and apply() call
+    benchmark.repair()  # implies both a delete_if() and apply() call
     assert db_count_entries(benchmark) == 10
 
-    benchmark.delete()
+    benchmark.delete()
```

### Comparing `AlgBench-2.4.0/tests/test_basics.py` & `AlgBench-2.4.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.4.0/tests/test_extensive.py` & `AlgBench-2.4.1/tests/test_extensive.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     benchmark = Benchmark("./extensive_benchmark")
     benchmark.clear()
     assert benchmark.empty()
 
     def f(x, _test=2, default="default"):
         print(x)
         return {"r1": x, "r2": "test"}
-    
+
     for x in range(500):
         benchmark.add(f, x, _test=None)
 
     assert len(benchmark) == 500
     for x, entry in enumerate(benchmark):
         assert entry["result"]["r1"] == x
     benchmark.compress()
@@ -28,9 +28,10 @@
     assert len(benchmark_) == 250
     for x, entry in enumerate(benchmark_):
         assert entry["result"]["r1"] == x * 2 + 1
     benchmark_.compress()
     assert len(benchmark_) == 250
     benchmark.delete()
 
+
 if __name__ == "__main__":
-    test_extensive_use_case()
+    test_extensive_use_case()
```

### Comparing `AlgBench-2.4.0/tests/test_file_splitting.py` & `AlgBench-2.4.1/tests/test_file_splitting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import os
+
 from algbench import Benchmark
 
-def test_file_splitting():
 
+def test_file_splitting():
     benchmark = Benchmark("./test_file_split_benchmark")
 
     # random data generation taken from https://stackoverflow.com/questions/16308989/
-    def generate_one_mb_results(args): 
-        offset = ord(b'A')
+    def generate_one_mb_results(args):
+        offset = ord(b"A")
         rand_bytes = os.urandom(1024 * 1024)
         array = bytearray(rand_bytes)
         for i, bt in enumerate(array):
             array[i] = offset + bt % 26
-        return {str(args["index"]) : bytes(array).decode()}
-        
+        return {str(args["index"]): bytes(array).decode()}
+
     for i in range(100):
-        benchmark.add(generate_one_mb_results, {"index" : i})
+        benchmark.add(generate_one_mb_results, {"index": i})
 
-    # Hardcoded for now. The file splits are hardcoded in nfs_json_list to be made at 30 MB. 
-    # For the 100MB + some curly brackets and environments, this should produce 4 files. 
-    assert len(os.listdir("./test_file_split_benchmark/results")) == 4 
+    # Hardcoded for now. The file splits are hardcoded in nfs_json_list to be made at 30 MB.
+    # For the 100MB + some curly brackets and environments, this should produce 4 files.
+    assert len(os.listdir("./test_file_split_benchmark/results")) == 4
 
-    benchmark.delete()
+    benchmark.delete()
```

### Comparing `AlgBench-2.4.0/tests/test_logger.py` & `AlgBench-2.4.1/tests/test_logger.py`

 * *Files identical despite different names*

