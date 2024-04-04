# Comparing `tmp/swebench-1.0.2.tar.gz` & `tmp/swebench-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.2.tar", last modified: Tue Apr  2 13:57:35 2024, max compression
+gzip compressed data, was "swebench-1.0.3.tar", last modified: Thu Apr  4 17:24:17 2024, max compression
```

## Comparing `swebench-1.0.2.tar` & `swebench-1.0.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.986966 swebench-1.0.2/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.2/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-02 13:57:35.986887 swebench-1.0.2/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5270 2024-04-02 05:49:19.000000 swebench-1.0.2/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.977476 swebench-1.0.2/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.978031 swebench-1.0.2/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.979527 swebench-1.0.2/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.2/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.2/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.2/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-02 13:57:35.987229 swebench-1.0.2/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.2/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.979815 swebench-1.0.2/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-02 13:57:17.000000 swebench-1.0.2/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.982137 swebench-1.0.2/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.983705 swebench-1.0.2/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18925 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    30156 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.2/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14820 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.985262 swebench-1.0.2/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.2/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     5746 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.2/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.986306 swebench-1.0.2/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.986581 swebench-1.0.2/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.756102 swebench-1.0.3/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.3/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-04 17:24:17.756030 swebench-1.0.3/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5270 2024-04-02 05:49:19.000000 swebench-1.0.3/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.745527 swebench-1.0.3/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.746246 swebench-1.0.3/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.748621 swebench-1.0.3/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.3/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.3/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.3/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.3/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.3/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-04 17:24:17.756307 swebench-1.0.3/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.3/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.748975 swebench-1.0.3/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-04 17:24:01.000000 swebench-1.0.3/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.750956 swebench-1.0.3/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.753171 swebench-1.0.3/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18925 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    30128 2024-04-04 17:22:05.000000 swebench-1.0.3/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.3/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14820 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.754709 swebench-1.0.3/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.3/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5932 2024-04-04 17:22:14.000000 swebench-1.0.3/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.3/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.755612 swebench-1.0.3/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.3/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-04 17:24:17.755793 swebench-1.0.3/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-04 17:24:17.000000 swebench-1.0.3/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.2/LICENSE` & `swebench-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/PKG-INFO` & `swebench-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.2
+Version: 1.0.3
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.2 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.3 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.2/README.md` & `swebench-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/llamao/distributed_attention.py` & `swebench-1.0.3/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/llamao/modeling_flash_llama.py` & `swebench-1.0.3/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/make_datasets/bm25_retrieval.py` & `swebench-1.0.3/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/make_datasets/create_instance.py` & `swebench-1.0.3/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/make_datasets/create_text_dataset.py` & `swebench-1.0.3/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/make_datasets/eval_retrieval.py` & `swebench-1.0.3/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/make_datasets/tokenize_dataset.py` & `swebench-1.0.3/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/make_datasets/utils.py` & `swebench-1.0.3/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/run_api.py` & `swebench-1.0.3/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/run_live.py` & `swebench-1.0.3/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/inference/run_llama.py` & `swebench-1.0.3/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/setup.py` & `swebench-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/__init__.py` & `swebench-1.0.3/swebench/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.0.2/swebench/collect/build_dataset.py` & `swebench-1.0.3/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/collect/build_dataset_ft.py` & `swebench-1.0.3/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/collect/get_tasks_pipeline.py` & `swebench-1.0.3/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/collect/get_top_pypi.py` & `swebench-1.0.3/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/collect/print_pulls.py` & `swebench-1.0.3/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/collect/utils.py` & `swebench-1.0.3/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/harness/constants.py` & `swebench-1.0.3/swebench/harness/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/harness/context_manager.py` & `swebench-1.0.3/swebench/harness/context_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging, os, platform, subprocess
 
+from logging import DEBUG, INFO, WARNING, ERROR, CRITICAL
 from swebench.harness.constants import (
     APPLY_PATCH_FAIL,
     APPLY_PATCH_PASS,
     DEFAULT_CONDA_LINK,
     INSTALL_FAIL,
     INSTALL_PASS,
     INSTALL_TIMEOUT,
@@ -25,41 +26,65 @@
     get_environment_yml,
     get_requirements,
     get_test_directives,
 )
 from tempfile import TemporaryDirectory
 from traceback import format_exc
 
-logging.basicConfig(
-    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
-)
+logging.basicConfig(format="%(asctime)s - %(levelname)s - %(message)s")
 logger_testbed = logging.getLogger("testbed_context_manager")
 
 
+class LogWrapper:
+    def __init__(
+        self,
+        log_file: str,
+        logger: logging.Logger = None,
+        prefix: str = None,
+    ):
+        self.log_file = log_file
+        self.logger = logger
+        self.prefix = prefix
+
+    def write(
+            self,
+            message: str,
+            mode: str = "a",
+            level: int = INFO):
+        with open(self.log_file, mode) as f:
+            log = f"{self.prefix} {message} \n" if self.prefix \
+                is not None else f"{message} \n"
+            f.write(log)
+        if self.logger is not None:
+            self.logger.log(level, message)
+
+
 class ExecWrapper:
     def __init__(
         self,
         subprocess_args: dict = None,
+        logger: logging.Logger = None,
     ):
+        self.logger = logger
         if subprocess_args is None:
             self.subprocess_args = {}
         else:
             self.subprocess_args = subprocess_args
 
     def __call__(self, cmd, raise_error=True, **kwargs):
         try:
             combined_args = {**self.subprocess_args, **kwargs}
             output = subprocess.run(cmd, **combined_args)
             return output
         except subprocess.CalledProcessError as e:
-            if raise_error:
-                logger_testbed.error(f"Error: {e}")
-                logger_testbed.error(f"Error stdout: {e.stdout}")
-                logger_testbed.error(f"Error stderr: {e.stderr}")
-                logger_testbed.error(f"Error traceback: {format_exc()}")
+            if raise_error and self.logger is not None:
+                self.logger.error(f"Error: {e}")
+                self.logger.error(f"Error stdout: {e.stdout}")
+                self.logger.error(f"Error stderr: {e.stderr}")
+                self.logger.error(f"Error traceback: {format_exc()}")
                 raise e
 
 
 class TestbedContextManager:
     def __init__(
         self,
         task_instances: list,
@@ -81,58 +106,40 @@
             conda_link(str): URL to conda installation to use
             path_conda (str): Path to conda installation
             testbed (str): Path to testbed directory
             verbose (bool): Whether to show logs
             timeout (int): Timeout for actions
             temp_dir (str): Path to temporary directory
         """
-        logger_testbed.propagate = verbose
+        if verbose:
+            logger_testbed.setLevel(logging.INFO)
         self.conda_link = conda_link
         self.log_dir = os.path.abspath(log_dir)
         self.old_dir = os.getcwd()
         self.timeout = timeout
         self.verbose = verbose
         self.exec = ExecWrapper(
             subprocess_args={
                 "check": True,
                 "shell": False,
                 "capture_output": True,
                 "text": True,
-            }
+            },
+            logger=logger_testbed,
         )
 
         # Create log, temp directories if they don't exist
         if not os.path.exists(self.log_dir):
             logger_testbed.info(f"[Testbed] Creating log directory {self.log_dir}")
             os.makedirs(self.log_dir, exist_ok=True)
         if temp_dir is not None and not os.path.exists(temp_dir):
             logger_testbed.info(f"[Testbed] Creating temp directory {temp_dir}")
             os.makedirs(temp_dir, exist_ok=True)
         temp_dir = os.path.abspath(temp_dir) if temp_dir is not None else None
 
-        # Set up conda path, create in temp directory if None
-        if path_conda is not None:
-            self.temp_dir_conda = None
-            self.path_conda = os.path.abspath(path_conda)
-        else:
-            self.temp_dir_conda = TemporaryDirectory(dir=temp_dir)
-            self.path_conda = self.temp_dir_conda.name
-        logger_testbed.info(f"[Testbed] Using conda path {self.path_conda}")
-
-        # Set up testbed path, create in temp directory if None
-        if testbed is not None:
-            self.temp_dir_work = None
-            self.testbed = os.path.abspath(testbed)
-        else:
-            self.temp_dir_work = TemporaryDirectory(dir=temp_dir)
-            self.testbed = self.temp_dir_work.name
-        logger_testbed.info(
-            f"[Testbed] Using working directory {self.testbed} for testbed"
-        )
-
         # Sort task instances by created_at
         self.task_instances = sorted(
             task_instances, key=lambda x: x["created_at"], reverse=True
         )
 
         # Group repos by repo, then version
         self.task_instances_grouped = {}
@@ -146,30 +153,66 @@
             repo = instance["repo"]
             version = instance["version"] if "version" in instance else None
             if repo not in self.task_instances_grouped:
                 self.task_instances_grouped[repo] = {}
             if version not in self.task_instances_grouped[repo]:
                 self.task_instances_grouped[repo][version] = []
             self.task_instances_grouped[repo][version].append(instance)
+        
+        # Check if instances are from single repo/version
+        self.is_single_repo_version = len(self.task_instances_grouped) == 1 and \
+            len(self.task_instances_grouped) == 1 and \
+            len(list(self.task_instances_grouped.values())[0]) == 1
+        
+        # Create log file for testbed
+        log_file_name = "testbed"
+        if self.is_single_repo_version:
+            key, versions = list(self.task_instances_grouped.items())[0]
+            _, repo = key.split("/")
+            version = list(versions.keys())[0]
+            log_file_name += f"_{repo}_{version}.log"
+        else:
+            # TODO: Make log file name more intelligible, random 4 digit number for now
+            # This random naming is necessary due to parallelized execution
+            log_file_name += f"_{os.urandom(24).hex()}.log"
+
+        self.log_file = os.path.join(self.log_dir, log_file_name)
+        self.log = LogWrapper(self.log_file, logger=logger_testbed, prefix="[Testbed]")
+        self.log.write(f"Created log file {self.log_file}", mode="w")
 
-        # Log grouped task instances to be run
+        # Get reference set up instances for each repo/version
         self.setup_refs = {}
         for repo, map_version_to_instances in self.task_instances_grouped.items():
-            logger_testbed.info(
-                f"[Testbed] Repo {repo}: {len(map_version_to_instances)} versions"
-            )
+            self.log.write(f"Repo {repo}: {len(map_version_to_instances)} versions")
 
             # Determine instances to use for environment installation
             self.setup_refs[repo] = {}
             for version, instances in map_version_to_instances.items():
-                logger_testbed.info(
-                    f"[Testbed] \tVersion {version}: {len(instances)} instances"
-                )
+                self.log.write(f"\tVersion {version}: {len(instances)} instances")
+                # Use the first instance as set up for each version
                 self.setup_refs[repo][version] = instances[0]
 
+        # Set up conda path, create in temp directory if None
+        if path_conda is not None:
+            self.temp_dir_conda = None
+            self.path_conda = os.path.abspath(path_conda)
+        else:
+            self.temp_dir_conda = TemporaryDirectory(dir=temp_dir)
+            self.path_conda = self.temp_dir_conda.name
+        self.log.write(f"Using conda path {self.path_conda}")
+
+        # Set up testbed path, create in temp directory if None
+        if testbed is not None:
+            self.temp_dir_work = None
+            self.testbed = os.path.abspath(testbed)
+        else:
+            self.temp_dir_work = TemporaryDirectory(dir=temp_dir)
+            self.testbed = self.temp_dir_work.name
+        self.log.write(f"Using working directory {self.testbed} for testbed")
+
         # Remove None versions, versions not in MAP_VERSION_TO_INSTALL
         self._custom_restraints()
 
     def __enter__(self):
         """
         Set up testbed (conda environments, git repositories)
         """
@@ -178,36 +221,34 @@
         if platform.system() == "Darwin" and platform.machine() == "arm64":
             is_osx_64 = True
         if self.temp_dir_conda is not None:
             # Set up the paths for Miniconda
             self.path_conda = os.path.join(self.path_conda, "miniconda3")
             os.mkdir(self.path_conda)
             miniconda_sh = os.path.join(self.path_conda, "miniconda.sh")
-            logger_testbed.info(
-                f"No conda path provided, creating temporary install in {self.path_conda}..."
-            )
+            self.log.write(f"No conda path provided, creating temporary install in {self.path_conda}...")
 
             # Download Miniconda installer
             if self.conda_link is not None:
                 cmd_line_install_link = self.conda_link
             else:
                 cmd_line_install_link = "https://repo.anaconda.com/miniconda/Miniconda3-"
 
                 # Adjust version for evaluation by repo/version
-                key, versions = list(self.setup_refs.items())[0]
-                if len(self.setup_refs) == 1 and len(versions) == 1:
+                if self.is_single_repo_version:
+                    key, versions = list(self.setup_refs.items())[0]
                     owner, repo = key.split("/")
                     version = list(versions.keys())[0]
-                    logger_testbed.info(f"[Testbed] {repo}/{version} instances in a single process")
+                    self.log.write(f"{repo}/{version} instances in a single process")
                     conda_id = MAP_REPO_VERSION_TO_CONDA_LINK.get(repo, {}).get(version, DEFAULT_CONDA_LINK)
                     cmd_line_install_link += conda_id
-                    logger_testbed.info(f"[Testbed] {repo}/{version} using Miniconda link: {cmd_line_install_link}")
+                    self.log.write(f"{repo}/{version} using Miniconda link: {cmd_line_install_link}")
                 else:
                     cmd_line_install_link += DEFAULT_CONDA_LINK
-                    logger_testbed.info(f"[Testbed] Multiple repos/versions; using Miniconda link: {cmd_line_install_link}")
+                    self.log.write(f"Multiple repos/versions; using Miniconda link: {cmd_line_install_link}")
 
                 if platform.system() == "Darwin":
                     if is_osx_64:
                         cmd_line_install_link += "-MacOSX-arm64.sh"
                     else:
                         cmd_line_install_link += "-MacOSX-x86_64.sh"
                 elif platform.system() == "Linux":
@@ -232,147 +273,123 @@
             if is_osx_64:
                 condabin = os.path.join(self.path_conda, "bin", "conda")
                 config_cmd = [condabin, "config", "--env", "--set", "subdir", "osx-64"]
                 self.exec(config_cmd)
 
             # Clean up the installer
             os.remove(miniconda_sh)
-        logger_testbed.info(f"[Testbed] Using conda path {self.path_conda}")
+        self.log.write(f"Using conda path {self.path_conda}")
 
         # Set up conda executables, get existing environments
         self.path_conda = os.path.abspath(self.path_conda)
-        conda_bin_path = os.path.join(self.path_conda, "bin")
-
         path_activate = os.path.join(self.path_conda, "bin", "activate")
         exec_cmd = os.path.join(self.path_conda, "bin", "conda")
         env_list = get_conda_env_names(exec_cmd)
 
         # Set up testbed (environment, github repo) for each repo
         for repo, version_to_setup_ref in self.setup_refs.items():
             repo_prefix = repo.replace("/", "__")
 
             # Run any repo-level installation commands if provided
             if repo in MAP_REPO_TO_INSTALL:
                 install_cmd = MAP_REPO_TO_INSTALL[repo]
-                logger_testbed.info(
-                    f"[Testbed] Running custom install command for {repo}: {install_cmd}"
-                )
+                self.log.write(f"Running custom install command for {repo}: {install_cmd}")
                 self.exec(install_cmd)
 
             # Create conda environment per version of the repo
             for version, install in MAP_VERSION_TO_INSTALL[repo].items():
                 # Skip if none of the task instances are for this version
                 if version not in version_to_setup_ref:
                     continue
 
                 # Name for both environment and github repo
                 env_name = f"{repo_prefix}__{version}"
-                logger_testbed.info(f"[Testbed] Setting up testbed for {env_name}")
+                self.log.write(f"Setting up testbed for {env_name}")
 
                 # Clone github per repo/version
                 repo_path = os.path.join(self.testbed, env_name)
                 if not os.path.exists(repo_path):
                     clone_repo(repo, repo_path)
-                    logger_testbed.info(f"[Testbed] Cloned {repo} to {repo_path}")
+                    self.log.write(f"Cloned {repo} to {repo_path}")
                 else:
-                    logger_testbed.info(
-                        f"[Testbed] Repo for {repo_prefix} version {version} exists: {repo_path}; skipping"
-                    )
+                    self.log.write(f"Repo for {repo_prefix} version {version} exists: {repo_path}; skipping")
 
                 # Skip if conda environment already exists
                 if env_name in env_list:
-                    logger_testbed.info(
-                        f"[Testbed] Environment {env_name} already exists; skipping"
-                    )
+                    self.log.write(f"Environment {env_name} already exists; skipping")
                     continue
 
                 # Get setup reference instance
                 setup_ref_instance = version_to_setup_ref[version]
 
                 # Create conda environment according to install instructinos
                 pkgs = install["packages"] if "packages" in install else ""
                 if pkgs == "requirements.txt":
                     # Create environment
                     cmd = (
                         f"{exec_cmd} create -n {env_name} python={install['python']} -y"
                     )
-                    logger_testbed.info(
-                        f"[Testbed] Creating environment {env_name}; Command: {cmd}"
-                    )
+                    self.log.write(f"Creating environment {env_name}; Command: {cmd}")
                     self.exec(cmd.split(" "))
 
                     # Install dependencies
                     path_to_reqs = get_requirements(setup_ref_instance, self.testbed)
                     cmd = f". {path_activate} {env_name} && echo 'activate successful' && pip install -r {path_to_reqs}"
-                    logger_testbed.info(
-                        f"[Testbed] Installing dependencies for {env_name}; Command: {cmd}"
-                    )
+                    self.log.write(f"Installing dependencies for {env_name}; Command: {cmd}")
                     self.exec(cmd, shell=True)
                     os.remove(path_to_reqs)
                 elif pkgs == "environment.yml":
                     if "no_use_env" in install and install["no_use_env"]:
                         # Create environment from yml
                         path_to_reqs = get_environment_yml(
                             setup_ref_instance, env_name,
                             save_path=self.testbed
                         )
 
                         # `conda create` based installation
                         cmd = f"{exec_cmd} create -c conda-forge -n {env_name} python={install['python']} -y"
-                        logger_testbed.info(
-                            f"[Testbed] Creating environment {env_name}; Command: {cmd}"
-                        )
+                        self.log.write(f"Creating environment {env_name}; Command: {cmd}")
                         self.exec(cmd.split(" "))
 
                         # Install dependencies
                         cmd = f"{exec_cmd} env update -f {path_to_reqs}"
-                        logger_testbed.info(
-                            f"[Testbed] Installing dependencies for {env_name}; Command: {cmd}"
-                        )
+                        self.log.write(f"Installing dependencies for {env_name}; Command: {cmd}")
                         self.exec(cmd.split(" "))
                     else:
                         # Create environment from yml
                         path_to_reqs = get_environment_yml(
                             setup_ref_instance, env_name,
                             save_path=self.testbed,
                             python_version=install["python"]
                         )
 
                         # `conda env create` based installation
                         cmd = f"{exec_cmd} env create --file {path_to_reqs}"
-                        logger_testbed.info(
-                            f"[Testbed] Creating environment {env_name}; Command: {cmd}"
-                        )
+                        self.log.write(f"Creating environment {env_name}; Command: {cmd}")
                         self.exec(cmd.split(" "))
 
                     # Remove environment.yml
                     os.remove(path_to_reqs)
                 else:
                     # Create environment + install dependencies
                     cmd = f"{exec_cmd} create -n {env_name} python={install['python']} {pkgs} -y"
-                    logger_testbed.info(
-                        f"[Testbed] Creating environment {env_name}; Command: {cmd}"
-                    )
+                    self.log.write(f"Creating environment {env_name}; Command: {cmd}")
                     self.exec(cmd.split(" "))
                 
                 arch = platform.machine()
                 arch_specific_packages = install.get("arch_specific_packages", {}).get(arch, "")
                 if arch_specific_packages:
                     cmd = f". {path_activate} {env_name} && conda install {arch_specific_packages} -y"
-                    logger_testbed.info(
-                        f"[Testbed] Installing arch-specific packages for {env_name}; Command: {cmd}"
-                    )
+                    self.log.write(f"Installing arch-specific packages for {env_name}; Command: {cmd}")
                     self.exec(cmd, shell=True)
 
                 # Install additional packages if specified
                 if "pip_packages" in install:
                     cmd = f". {path_activate} {env_name} && pip install {install['pip_packages']}"
-                    logger_testbed.info(
-                        f"[Testbed] Installing pip packages for {env_name}; Command: {cmd}"
-                    )
+                    self.log.write(f"Installing pip packages for {env_name}; Command: {cmd}")
                     self.exec(cmd, shell=True)
 
         return self
 
     def get_distributed_tasks(self) -> list:
         """
         Create task group (instances + keywords) for each repo/version
@@ -401,22 +418,23 @@
 
     def _custom_restraints(self):
         """
         Custom restraints per repo
         """
         for repo, group in self.task_instances_grouped.items():
             if None in group:
-                logger_testbed.info(f"[Testbed] Removed None version from repo {repo}")
+                self.log.write(f"Removed None version from repo {repo}")
                 del group[None]
             versions = list(group.keys())
             for version in versions:
                 if version not in MAP_VERSION_TO_INSTALL[repo]:
-                    logger_testbed.info(
-                        f"[Testbed] Removed {version} version from repo {repo} (Install instructions not given)"
-                    )
+                    self.log.write((
+                        f"Removed {version} version from repo "
+                        f"{repo} (Install instructions not given)"
+                    ))
                     del group[version]
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         if self.temp_dir_work is not None:
             self.temp_dir_work.cleanup()
         if self.temp_dir_conda is not None:
             self.temp_dir_conda.cleanup()
@@ -448,15 +466,16 @@
             log_dir (str): Path to log directory
             conda_path (str): Path to conda installation
             verbose (bool): Whether to show logs
             timeout (int): Timeout for actions
             is_eval (bool): Whether this is for evaluating a model on SWE Bench
                 (Mainly for logging purposes)
         """
-        logger_taskenv.propagate = verbose
+        if verbose:
+            logger_taskenv.setLevel(logging.INFO)
         self.instance = instance
         self.conda_path = conda_path
         self.conda_cache_dir = os.path.join(self.conda_path, "cache")
         self.cwd = os.getcwd()
         self.is_eval = is_eval
         self.testbed = testbed
         self.testbed_name = testbed.split("/")[-1]
@@ -471,42 +490,49 @@
         if log_suffix is not None:
             log_file_name = (
                 f"{instance[KEY_INSTANCE_ID]}.{instance[KEY_MODEL]}.{log_suffix}.eval.log"
                 if self.is_eval
                 else f"{instance[KEY_INSTANCE_ID]}.{log_suffix}.log"
             )
         self.log_file = os.path.join(log_dir, log_file_name)
+        self.log = LogWrapper(
+            self.log_file, logger=logger_taskenv,
+            prefix=f"[{self.testbed_name}] [{self.instance[KEY_INSTANCE_ID]}]")
 
         self.cmd_activate = (
             f". {os.path.join(self.conda_path, 'bin', 'activate')} "
             + f"{self.venv} && echo 'activate successful'"
         )
         self.timeout = timeout
 
         self.exec = ExecWrapper(
             subprocess_args={
                 "check": True,
                 "shell": False,
                 "capture_output": True,
                 "text": True,
                 "env": {"CONDA_PKGS_DIRS": self.conda_cache_dir},
-            }
+            },
+            logger=logger_taskenv,
         )
 
     def __enter__(self):
         """
         Enter task environment, set up log file
         """
         os.chdir(self.testbed)
-        with open(self.log_file, "w") as f:
-            f.write(
-                f"Task Metadata:\n\t- Instance ID: {self.instance[KEY_INSTANCE_ID]}\n\t- Testbed: {self.testbed}\n\t- Virtual Env.: {self.venv}\n"
-            )
-            if self.is_eval:
-                f.write(f"\t- Evaluation Model: {self.instance[KEY_MODEL]}\n")
+        enter_msg = (
+            f"Task Metadata:\n\t- "
+            f"Instance ID: {self.instance[KEY_INSTANCE_ID]}\n\t- "
+            f"Testbed: {self.testbed}\n\t- "
+            f"Virtual Env.: {self.venv}"
+        )
+        if self.is_eval:
+            enter_msg += f"\n\t- Evaluation Model: {self.instance[KEY_MODEL]}"
+        self.log.write(enter_msg, mode="w")
         return self
 
     def reset_task_env(self, instance: dict):
         """
         Reset task environment + testbed and checkout base commit of given task instance
 
         Args:
@@ -527,21 +553,19 @@
             self.exec("git reset HEAD .".split(" "))
             self.exec("git clean -fdx".split(" "))
             self.exec(
                 f"git -c advice.detachedHead=false checkout {instance['base_commit']}".split(
                     " "
                 )
             )
-            logger_taskenv.info(
-                f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Reset task environment to {instance['base_commit']}"
-            )
+            self.log.write(f"Reset task environment to {instance['base_commit']}")
             return True
         except Exception as e:
             err_msg = f"{RESET_FAILED}; Failed to reset task environment to {instance['base_commit']}: {e}"
-            logger_taskenv.error(f"[{self.testbed_name}] {err_msg}")
+            self.log.write(err_msg, level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(err_msg)
             return False
 
     def run_install_task(self, instance: dict) -> bool:
         """
         Run installation for task instance
@@ -554,79 +578,65 @@
         # Get installation instructions by repo/version
         specifications = MAP_VERSION_TO_INSTALL[instance["repo"]][instance["version"]]
 
         # Run pre-install set up if provided
         if "pre_install" in specifications:
             for pre_install in specifications["pre_install"]:
                 cmd_pre_install = f"{self.cmd_activate} && {pre_install}"
-                logger_taskenv.info(
-                    f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Running pre-install setup command: {cmd_pre_install}"
-                )
+                self.log.write(f"Running pre-install setup command: {cmd_pre_install}")
                 out_pre_install = self.exec(
                     cmd_pre_install, timeout=self.timeout, shell=True
                 )
                 with open(self.log_file, "a") as f:
                     f.write(f"Pre-installation Command: {cmd_pre_install}\n")
                     f.write(f"Std. Output: {out_pre_install.stdout}\n")
                     f.write(f"Std. Error: {out_pre_install.stderr}\n")
                 if out_pre_install.returncode != 0:
-                    logger_taskenv.error(
-                        f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Pre-install setup failed"
-                    )
+                    self.log.write(f"Pre-install setup failed", level=ERROR)
                     with open(self.log_file, "a") as f:
                         f.write(f"\n{INSTALL_FAIL}\n")
                     return False
 
         # Skip installation if no instructions provided
         if "install" not in specifications:
             return True
 
         cmd_install = f"{self.cmd_activate} && {specifications['install']}"
-        logger_taskenv.info(
-            f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Installing with command: {cmd_install}"
-        )
+        self.log.write(f"Running installation command: {cmd_install}")
         try:
             # Run installation command
             out_install = self.exec(cmd_install, timeout=self.timeout, shell=True)
 
             # Write installation logs to log file
             with open(self.log_file, "a") as f:
                 f.write(f"Installation Command: {cmd_install}\n")
                 f.write(f"Std. Output: {out_install.stdout}\n")
                 f.write(f"Std. Error: {out_install.stderr}\n")
 
             if out_install.returncode != 0:
                 # Installation failed
-                logger_taskenv.error(
-                    f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Installation failed"
-                )
+                self.log.write(f"Installation failed", level=ERROR)
                 with open(self.log_file, "a") as f:
                     f.write(f"\n{INSTALL_FAIL}\n")
                 return False
 
             # Installation successful
-            logger_taskenv.info(
-                f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Installation successful"
-            )
+            self.log.write(f"Installation successful")
             with open(self.log_file, "a") as f:
                 f.write(f"\n{INSTALL_PASS}\n")
             return True
         except subprocess.TimeoutExpired:
             # Installation timed out
-            logger_taskenv.error(
-                f"[{self.testbed_name}] [{self.instance[KEY_INSTANCE_ID]}] Installation timed out"
-            )
+            self.log.write(f"Installation timed out", level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(f"\n{INSTALL_TIMEOUT}\n")
             return False
         except Exception as e:
             # Installation failed
-            logger_taskenv.error(
-                f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Installation failed"
-            )
+            self.log.write(f"Installation failed", level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(f"\n{INSTALL_FAIL}: {e}\n")
             return False
 
     def apply_patch(
         self, patch: str, patch_type: str = "", revert: bool = False
     ) -> bool:
@@ -637,17 +647,15 @@
             patch (str): Plaintext of patch to apply
             patch_type (str): Type of patch (e.g. "eval", "test")
         Returns:
             bool: True if patch applied successfully, False otherwise
         """
         # If patch is `None`, indicate in log and skip
         if patch is None:
-            logger_taskenv.error(
-                f"[{self.testbed_name}] [{self.instance[KEY_INSTANCE_ID]}] Patch is `None` ({patch_type})"
-            )
+            self.log.write(f"Patch is `None` ({patch_type})")
             with open(self.log_file, "a") as f:
                 f.write(f"{APPLY_PATCH_FAIL}; Prediction patch is `None`")
             return False
 
         # Write patch to temporary patch file in parent directory
         patch_path = os.path.join(
             os.path.dirname(self.testbed.rstrip("/")),
@@ -662,27 +670,23 @@
         )
         out_patch = self.exec(apply_cmd.split(" "), raise_error=False, check=False)
         os.remove(patch_path)
 
         log_cmd = "Revert" if revert else "Apply"
         if out_patch.returncode != 0:
             # Patch apply failed
-            logger_taskenv.error(
-                f"[{self.testbed_name}] [{self.instance[KEY_INSTANCE_ID]}] {log_cmd} patch failed ({patch_type})"
-            )
+            self.log.write(f"{log_cmd} patch failed ({patch_type})", level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(f"{APPLY_PATCH_FAIL}; ({patch_type})\nOutput:\n")
                 f.write(out_patch.stdout)
                 f.write(out_patch.stderr)
             return False
 
         # Patch apply succeeded
-        logger_taskenv.info(
-            f"[{self.testbed_name}] [{self.instance[KEY_INSTANCE_ID]}] {log_cmd} patch successful ({patch_type})"
-        )
+        self.log.write(f"{log_cmd} patch successful ({patch_type})")
         with open(self.log_file, "a") as f:
             f.write(f"{APPLY_PATCH_PASS} ({patch_type})\n")
         return True
 
     def run_tests_task(self, instance: dict):
         """
         Run tests for task instance
@@ -707,30 +711,24 @@
                 f.write(out_test.stdout)
                 f.write(out_test.stderr)
                 if out_test.returncode != 0:
                     f.write(f"\n{TESTS_FAILED}\n")
                 else:
                     f.write(f"\n{TESTS_PASSED}\n")
 
-            logger_taskenv.info(
-                f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Test script run successful"
-            )
+            self.log.write(f"Test script run successful")
             return True
         except subprocess.TimeoutExpired:
             # Test command run timed out
-            logger_taskenv.error(
-                f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Test script run time out {self.timeout}"
-            )
+            self.log.write("Test script run timed out", level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(f"{TESTS_TIMEOUT} after {self.timeout} seconds\n")
             return False
         except Exception as e:
             # Test command run failed
-            logger_taskenv.error(
-                f"[{self.testbed_name}] [{instance[KEY_INSTANCE_ID]}] Test script run failed"
-            )
+            self.log.write(f"Test script run failed", level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(f"{TESTS_ERROR}: {e}")
             return False
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         os.chdir(self.cwd)
```

### Comparing `swebench-1.0.2/swebench/harness/engine_evaluation.py` & `swebench-1.0.3/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/harness/engine_validation.py` & `swebench-1.0.3/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/harness/run_evaluation.py` & `swebench-1.0.3/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/harness/utils.py` & `swebench-1.0.3/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/metrics/constants.py` & `swebench-1.0.3/swebench/metrics/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/metrics/conversion.py` & `swebench-1.0.3/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/metrics/getters.py` & `swebench-1.0.3/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/metrics/log_parsers.py` & `swebench-1.0.3/swebench/metrics/log_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,18 @@
             test_case = line.split()[1]
             test_status_map[test_case] = TestStatus.FAILED.value
         elif f" {TestStatus.PASSED.value} " in line:
             parts = line.split()
             if parts[1] == TestStatus.PASSED.value:
                 test_case = parts[0]
                 test_status_map[test_case] = TestStatus.PASSED.value
+        elif line.startswith(TestStatus.PASSED.value):
+            parts = line.split()
+            test_case = parts[1]
+            test_status_map[test_case] = TestStatus.PASSED.value
     return test_status_map
 
 
 def parse_log_sympy(log):
     """
     Parser for test logs generated with Sympy framework
```

### Comparing `swebench-1.0.2/swebench/metrics/metrics.py` & `swebench-1.0.3/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/metrics/monitor.py` & `swebench-1.0.3/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/metrics/report.py` & `swebench-1.0.3/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/versioning/constants.py` & `swebench-1.0.3/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/versioning/get_versions.py` & `swebench-1.0.3/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench/versioning/utils.py` & `swebench-1.0.3/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.2/swebench.egg-info/PKG-INFO` & `swebench-1.0.3/swebench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.2
+Version: 1.0.3
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.2 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.3 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.2/swebench.egg-info/SOURCES.txt` & `swebench-1.0.3/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

