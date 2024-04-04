# Comparing `tmp/arkindex-base-worker-0.3.7rc6.tar.gz` & `tmp/arkindex-base-worker-0.3.7rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.7rc6.tar", last modified: Wed Mar 20 14:54:24 2024, max compression
+gzip compressed data, was "arkindex-base-worker-0.3.7rc7.tar", last modified: Thu Apr  4 13:32:10 2024, max compression
```

## Comparing `arkindex-base-worker-0.3.7rc6.tar` & `arkindex-base-worker-0.3.7rc7.tar`

### file list

```diff
@@ -1,55 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:54:24.389160 arkindex-base-worker-0.3.7rc6/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3389 2024-03-20 14:54:24.389160 arkindex-base-worker-0.3.7rc6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:54:24.389160 arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3389 2024-03-20 14:54:24.000000 arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1484 2024-03-20 14:54:24.000000 arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 14:54:24.000000 arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      288 2024-03-20 14:54:24.000000 arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-20 14:54:24.000000 arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:54:24.385160 arkindex-base-worker-0.3.7rc6/arkindex_worker/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11248 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    14166 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/image.py
--rw-rw-rw-   0 root         (0) root         (0)     9526 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6900 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:54:24.385160 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/
--rw-rw-rw-   0 root         (0) root         (0)    19498 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19934 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10328 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     3228 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    33848 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/element.py
--rw-rw-rw-   0 root         (0) root         (0)    14630 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6669 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/task.py
--rw-rw-rw-   0 root         (0) root         (0)    10235 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/training.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/transcription.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/version.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/docs-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2349 2024-03-20 14:50:36.000000 arkindex-base-worker-0.3.7rc6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 14:54:24.389160 arkindex-base-worker-0.3.7rc6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:54:24.385160 arkindex-base-worker-0.3.7rc6/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 14:54:05.000000 arkindex-base-worker-0.3.7rc6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22004 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    24512 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_base_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    10640 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    28273 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_dataset_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    13181 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:54:24.389160 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26417 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    13475 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    84971 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_elements.py
--rw-rw-rw-   0 root         (0) root         (0)    34557 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    18672 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6312 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8414 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)    73468 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_transcriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17163 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    16262 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     8331 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-03-20 14:46:26.000000 arkindex-base-worker-0.3.7rc6/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.146465 arkindex-base-worker-0.3.7rc7/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3359 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3359 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1633 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-04 13:32:10.000000 arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.134466 arkindex-base-worker-0.3.7rc7/arkindex_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9844 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6900 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.138466 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/
+-rw-rw-rw-   0 root         (0) root         (0)    18575 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19585 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10328 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    33848 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/element.py
+-rw-rw-rw-   0 root         (0) root         (0)    14714 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/training.py
+-rw-rw-rw-   0 root         (0) root         (0)    20464 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/transcription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/docs-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.138466 arkindex-base-worker-0.3.7rc7/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/hooks/pre_gen_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     2405 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 13:32:10.146465 arkindex-base-worker-0.3.7rc7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.138466 arkindex-base-worker-0.3.7rc7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 13:31:52.000000 arkindex-base-worker-0.3.7rc7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22134 2024-04-04 13:28:53.000000 arkindex-base-worker-0.3.7rc7/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    24512 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_base_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10640 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    23728 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_dataset_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    13181 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26417 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11777 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    84971 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    34557 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18756 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8414 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)    73468 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_transcriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17163 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    16262 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8331 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-04 13:28:54.000000 arkindex-base-worker-0.3.7rc7/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.134466 arkindex-base-worker-0.3.7rc7/worker-demo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/worker-demo/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/tests/test_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:32:10.142465 arkindex-base-worker-0.3.7rc7/worker-demo/worker_demo/
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/worker_demo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-04 13:29:16.000000 arkindex-base-worker-0.3.7rc7/worker-demo/worker_demo/worker.py
```

### Comparing `arkindex-base-worker-0.3.7rc6/LICENSE` & `arkindex-base-worker-0.3.7rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/PKG-INFO` & `arkindex-base-worker-0.3.7rc7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-base-worker
-Version: 0.3.7rc6
+Version: 0.3.7rc7
 Summary: Base Worker to easily build Arkindex ML workflows
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 Teklia
         
@@ -37,21 +37,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: arkindex-client==1.0.15
 Requires-Dist: peewee==3.17.0
 Requires-Dist: Pillow==10.2.0
 Requires-Dist: pymdown-extensions==10.7
 Requires-Dist: python-gnupg==0.5.2
 Requires-Dist: shapely==2.0.3
-Requires-Dist: tenacity==8.2.3
+Requires-Dist: teklia-toolbox==0.1.4rc3
 Requires-Dist: zstandard==0.22.0
 Provides-Extra: docs
 Requires-Dist: black==24.2.0; extra == "docs"
 Requires-Dist: doc8==1.1.1; extra == "docs"
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.10; extra == "docs"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs"
```

### Comparing `arkindex-base-worker-0.3.7rc6/README.md` & `arkindex-base-worker-0.3.7rc7/README.md`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/PKG-INFO` & `arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-base-worker
-Version: 0.3.7rc6
+Version: 0.3.7rc7
 Summary: Base Worker to easily build Arkindex ML workflows
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 Teklia
         
@@ -37,21 +37,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: arkindex-client==1.0.15
 Requires-Dist: peewee==3.17.0
 Requires-Dist: Pillow==10.2.0
 Requires-Dist: pymdown-extensions==10.7
 Requires-Dist: python-gnupg==0.5.2
 Requires-Dist: shapely==2.0.3
-Requires-Dist: tenacity==8.2.3
+Requires-Dist: teklia-toolbox==0.1.4rc3
 Requires-Dist: zstandard==0.22.0
 Provides-Extra: docs
 Requires-Dist: black==24.2.0; extra == "docs"
 Requires-Dist: doc8==1.1.1; extra == "docs"
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.10; extra == "docs"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs"
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_base_worker.egg-info/SOURCES.txt` & `arkindex-base-worker-0.3.7rc7/arkindex_base_worker.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 docs-requirements.txt
 pyproject.toml
 requirements.txt
-setup.py
 arkindex_base_worker.egg-info/PKG-INFO
 arkindex_base_worker.egg-info/SOURCES.txt
 arkindex_base_worker.egg-info/dependency_links.txt
 arkindex_base_worker.egg-info/requires.txt
 arkindex_base_worker.egg-info/top_level.txt
 arkindex_worker/__init__.py
 arkindex_worker/cache.py
@@ -21,14 +20,15 @@
 arkindex_worker/worker/element.py
 arkindex_worker/worker/entity.py
 arkindex_worker/worker/metadata.py
 arkindex_worker/worker/task.py
 arkindex_worker/worker/training.py
 arkindex_worker/worker/transcription.py
 arkindex_worker/worker/version.py
+hooks/pre_gen_project.py
 tests/__init__.py
 tests/conftest.py
 tests/test_base_worker.py
 tests/test_cache.py
 tests/test_dataset_worker.py
 tests/test_element.py
 tests/test_image.py
@@ -40,8 +40,12 @@
 tests/test_elements_worker/test_dataset.py
 tests/test_elements_worker/test_elements.py
 tests/test_elements_worker/test_entities.py
 tests/test_elements_worker/test_metadata.py
 tests/test_elements_worker/test_task.py
 tests/test_elements_worker/test_training.py
 tests/test_elements_worker/test_transcriptions.py
-tests/test_elements_worker/test_worker.py
+tests/test_elements_worker/test_worker.py
+worker-demo/tests/conftest.py
+worker-demo/tests/test_worker.py
+worker-demo/worker_demo/__init__.py
+worker-demo/worker_demo/worker.py
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/cache.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/image.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
 from arkindex_worker import logger
+from teklia_toolbox.requests import should_verify_cert
 
 # Avoid circular imports error when type checking
 if TYPE_CHECKING:
     from arkindex_worker.cache import CachedElement
     from arkindex_worker.models import Element
 
 # See http://docs.python-requests.org/en/master/user/advanced/#timeouts
@@ -171,15 +172,17 @@
     stop=stop_after_attempt(3),
     wait=wait_exponential(multiplier=2),
     retry=retry_if_exception_type(requests.RequestException),
     before_sleep=_retry_log,
     reraise=True,
 )
 def _retried_request(url, *args, method=requests.get, **kwargs):
-    resp = method(url, *args, timeout=DOWNLOAD_TIMEOUT, **kwargs)
+    resp = method(
+        url, *args, timeout=DOWNLOAD_TIMEOUT, verify=should_verify_cert(url), **kwargs
+    )
     resp.raise_for_status()
     return resp
 
 
 def download_tiles(url: str) -> Image:
     """
     Reconstruct a full IIIF image on servers that cannot serve the full-sized image, using tiles.
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/models.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     """
 
     def _magify(self, item):
         """
         Automagically convert lists and dicts to MagicDicts and lists of MagicDicts
         Allows for nested access: foo.bar.baz
         """
+        if isinstance(item, Dataset):
+            return item
         if isinstance(item, list):
             return list(map(self._magify, item))
         if isinstance(item, dict):
             return MagicDict(item)
         return item
 
     def __getitem__(self, item):
@@ -268,11 +270,21 @@
     def filepath(self) -> str:
         """
         Generic filepath to the Dataset compressed archive.
         """
         return f"{self.id}.tar.zst"
 
 
+class Set(MagicDict):
+    """
+    Describes an Arkindex dataset set.
+    """
+
+    def __str__(self):
+        # Not using ArkindexModel.__str__ as we do not retrieve the Set ID
+        return f"{self.__class__.__name__} ({self.name}) from {self.dataset}"
+
+
 class Artifact(ArkindexModel):
     """
     Describes an Arkindex artifact.
     """
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/utils.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/utils.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/__init__.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,34 +3,33 @@
 """
 
 import contextlib
 import json
 import os
 import sys
 import uuid
+from argparse import ArgumentTypeError
 from collections.abc import Iterable, Iterator
 from enum import Enum
-from itertools import groupby
-from operator import itemgetter
 from pathlib import Path
 
 from apistar.exceptions import ErrorResponse
 
 from arkindex_worker import logger
 from arkindex_worker.cache import CachedElement
-from arkindex_worker.models import Dataset, Element
+from arkindex_worker.models import Dataset, Element, Set
 from arkindex_worker.worker.base import BaseWorker
 from arkindex_worker.worker.classification import ClassificationMixin
 from arkindex_worker.worker.dataset import DatasetMixin, DatasetState
 from arkindex_worker.worker.element import ElementMixin
-from arkindex_worker.worker.entity import EntityMixin  # noqa: F401
+from arkindex_worker.worker.entity import EntityMixin
 from arkindex_worker.worker.metadata import MetaDataMixin, MetaType  # noqa: F401
 from arkindex_worker.worker.task import TaskMixin
 from arkindex_worker.worker.transcription import TranscriptionMixin
-from arkindex_worker.worker.version import WorkerVersionMixin  # noqa: F401
+from arkindex_worker.worker.version import WorkerVersionMixin
 
 
 class ActivityState(Enum):
     """
     Processing state of an element.
     """
 
@@ -156,14 +155,24 @@
 
         if self.is_read_only:
             super().configure_for_developers()
         else:
             super().configure()
             super().configure_cache()
 
+        # Retrieve the model configuration
+        if self.model_configuration:
+            self.config.update(self.model_configuration)
+            logger.info("Model version configuration retrieved")
+
+        # Retrieve the user configuration
+        if self.user_configuration:
+            self.config.update(self.user_configuration)
+            logger.info("User configuration retrieved")
+
     def run(self):
         """
         Implements an Arkindex worker that goes through each element returned by
         [list_elements][arkindex_worker.worker.ElementsWorker.list_elements].
         It calls [process_element][arkindex_worker.worker.ElementsWorker.process_element],
         catching exceptions, and handles saving WorkerActivity updates when enabled.
         """
@@ -297,219 +306,201 @@
             )
             raise e
 
         logger.debug(f"Updated activity of element {element_id} to {state}")
         return True
 
 
+def check_dataset_set(value: str) -> tuple[uuid.UUID, str]:
+    values = value.split(":")
+    if len(values) != 2:
+        raise ArgumentTypeError(
+            f"'{value}' is not in the correct format `<dataset_id>:<set_name>`"
+        )
+
+    dataset_id, set_name = values
+    try:
+        dataset_id = uuid.UUID(dataset_id)
+        return (dataset_id, set_name)
+    except (TypeError, ValueError) as e:
+        raise ArgumentTypeError(f"'{dataset_id}' should be a valid UUID") from e
+
+
 class MissingDatasetArchive(Exception):
     """
     Exception raised when the compressed archive associated to
     a dataset isn't found in its task artifacts.
     """
 
 
 class DatasetWorker(BaseWorker, DatasetMixin, TaskMixin):
     """
-    Base class for ML workers that operate on Arkindex datasets.
+    Base class for ML workers that operate on Arkindex dataset sets.
 
     This class inherits from numerous mixin classes found in other modules of
     ``arkindex.worker``, which provide helpers to read and write to the Arkindex API.
     """
 
     def __init__(
         self,
         description: str = "Arkindex Dataset Worker",
         support_cache: bool = False,
-        generator: bool = False,
     ):
         """
         :param description: The worker's description.
         :param support_cache: Whether the worker supports cache.
-        :param generator: Whether the worker generates the dataset archive artifact.
         """
         super().__init__(description, support_cache)
 
+        self.downloaded_artifact: Path | None = None
+
         self.parser.add_argument(
-            "--dataset",
-            type=uuid.UUID,
+            "--set",
+            type=check_dataset_set,
             nargs="+",
-            help="One or more Arkindex dataset ID",
+            help="""
+                One or more Arkindex dataset sets, format is <dataset_uuid>:<set_name>
+                (e.g.: "12341234-1234-1234-1234-123412341234:train")
+            """,
+            default=[],
         )
 
-        self.generator = generator
-
     def configure(self):
         """
         Setup the worker using CLI arguments and environment variables.
         """
         # CLI args are stored on the instance so that implementations can access them
         self.args = self.parser.parse_args()
 
         if self.is_read_only:
             super().configure_for_developers()
         else:
             super().configure()
             super().configure_cache()
 
-    def download_dataset_artifact(self, dataset: Dataset) -> Path:
+        # Retrieve the model configuration
+        if self.model_configuration:
+            self.config.update(self.model_configuration)
+            logger.info("Model version configuration retrieved")
+
+        # Retrieve the user configuration
+        if self.user_configuration:
+            self.config.update(self.user_configuration)
+            logger.info("User configuration retrieved")
+
+    def cleanup_downloaded_artifact(self) -> None:
+        """
+        Cleanup the downloaded artifact if any
+        """
+        if not self.downloaded_artifact:
+            return
+
+        self.downloaded_artifact.unlink(missing_ok=True)
+
+    def download_dataset_artifact(self, dataset: Dataset) -> None:
         """
         Find and download the compressed archive artifact describing a dataset using
         the [list_artifacts][arkindex_worker.worker.task.TaskMixin.list_artifacts] and
         [download_artifact][arkindex_worker.worker.task.TaskMixin.download_artifact] methods.
 
         :param dataset: The dataset to retrieve the compressed archive artifact for.
-        :returns: A path to the downloaded artifact.
         :raises MissingDatasetArchive: When the dataset artifact is not found.
         """
+        extra_dir = self.find_extras_directory()
+        archive = extra_dir / dataset.filepath
+        if archive.exists():
+            return
 
-        task_id = uuid.UUID(dataset.task_id)
+        # Cleanup the dataset artifact that was downloaded previously
+        self.cleanup_downloaded_artifact()
 
+        logger.info(f"Downloading artifact for {dataset}")
+        task_id = uuid.UUID(dataset.task_id)
         for artifact in self.list_artifacts(task_id):
             if artifact.path != dataset.filepath:
                 continue
 
-            extra_dir = self.find_extras_directory()
-            archive = extra_dir / dataset.filepath
             archive.write_bytes(self.download_artifact(task_id, artifact).read())
-            return archive
+            self.downloaded_artifact = archive
+            return
 
         raise MissingDatasetArchive(
             "The dataset compressed archive artifact was not found."
         )
 
-    def list_dataset_elements_per_split(
-        self, dataset: Dataset
-    ) -> Iterator[tuple[str, list[Element]]]:
-        """
-        List the elements in the dataset, grouped by split, using the
-        [list_dataset_elements][arkindex_worker.worker.dataset.DatasetMixin.list_dataset_elements] method.
-
-        :param dataset: The dataset to retrieve elements from.
-        :returns: An iterator of tuples containing the split name and the list of its elements.
-        """
-
-        def format_split(
-            split: tuple[str, Iterator[tuple[str, Element]]],
-        ) -> tuple[str, list[Element]]:
-            return (split[0], list(map(itemgetter(1), list(split[1]))))
-
-        return map(
-            format_split,
-            groupby(
-                sorted(self.list_dataset_elements(dataset), key=itemgetter(0)),
-                key=itemgetter(0),
-            ),
-        )
-
-    def process_dataset(self, dataset: Dataset):
+    def process_set(self, set: Set):
         """
-        Override this method to implement your worker and process a single Arkindex dataset at once.
+        Override this method to implement your worker and process a single Arkindex dataset set at once.
 
-        :param dataset: The dataset to process.
+        :param set: The set to process.
         """
 
-    def list_datasets(self) -> Iterator[Dataset] | Iterator[str]:
+    def list_sets(self) -> Iterator[Set]:
         """
-        List the datasets to be processed, either from the CLI arguments or using the
-        [list_process_datasets][arkindex_worker.worker.dataset.DatasetMixin.list_process_datasets] method.
+        List the sets to be processed, either from the CLI arguments or using the
+        [list_process_sets][arkindex_worker.worker.dataset.DatasetMixin.list_process_sets] method.
 
-        :returns: An iterator of strings if the worker is in read-only mode,
-        else an iterator of ``Dataset`` objects.
+        :returns: An iterator of ``Set`` objects.
         """
-        if self.is_read_only:
-            return map(str, self.args.dataset)
+        if not self.is_read_only:
+            yield from self.list_process_sets()
+
+        datasets: dict[uuid.UUID, Dataset] = {}
+        for dataset_id, set_name in self.args.set:
+            # Retrieving dataset information is not already cached
+            if dataset_id not in datasets:
+                datasets[dataset_id] = Dataset(
+                    **self.request("RetrieveDataset", id=dataset_id)
+                )
 
-        return self.list_process_datasets()
+            yield Set(name=set_name, dataset=datasets[dataset_id])
 
     def run(self):
         """
-        Implements an Arkindex worker that goes through each dataset returned by
-        [list_datasets][arkindex_worker.worker.DatasetWorker.list_datasets].
+        Implements an Arkindex worker that goes through each dataset set returned by
+        [list_sets][arkindex_worker.worker.DatasetWorker.list_sets].
 
-        It calls [process_dataset][arkindex_worker.worker.DatasetWorker.process_dataset],
-        catching exceptions, and handles updating the [DatasetState][arkindex_worker.worker.dataset.DatasetState]
-        when the worker is a generator.
+        It calls [process_set][arkindex_worker.worker.DatasetWorker.process_set],
+        catching exceptions.
         """
         self.configure()
 
-        datasets: list[Dataset] | list[str] = list(self.list_datasets())
-        if not datasets:
-            logger.warning("No datasets to process, stopping.")
+        dataset_sets: list[Set] = list(self.list_sets())
+        if not dataset_sets:
+            logger.warning("No sets to process, stopping.")
             sys.exit(1)
 
-        # Process every dataset
-        count = len(datasets)
+        # Process every set
+        count = len(dataset_sets)
         failed = 0
-        for i, item in enumerate(datasets, start=1):
-            dataset = None
-            dataset_artifact = None
-
+        for i, dataset_set in enumerate(dataset_sets, start=1):
             try:
-                if not self.is_read_only:
-                    # Just use the result of list_datasets as the dataset
-                    dataset = item
-                else:
-                    # Load dataset using the Arkindex API
-                    dataset = Dataset(**self.request("RetrieveDataset", id=item))
+                assert (
+                    dataset_set.dataset.state == DatasetState.Complete.value
+                ), "When processing a set, its dataset state should be Complete."
 
-                if self.generator:
-                    assert (
-                        dataset.state
-                        in [DatasetState.Open.value, DatasetState.Error.value]
-                    ), "When generating a new dataset, its state should be Open or Error."
-                else:
-                    assert (
-                        dataset.state == DatasetState.Complete.value
-                    ), "When processing an existing dataset, its state should be Complete."
-
-                logger.info(f"Processing {dataset} ({i}/{count})")
-
-                if self.generator:
-                    # Update the dataset state to Building
-                    logger.info(f"Building {dataset} ({i}/{count})")
-                    self.update_dataset_state(dataset, DatasetState.Building)
-                else:
-                    logger.info(f"Downloading data for {dataset} ({i}/{count})")
-                    dataset_artifact = self.download_dataset_artifact(dataset)
+                logger.info(f"Retrieving data for {dataset_set} ({i}/{count})")
+                self.download_dataset_artifact(dataset_set.dataset)
 
-                # Process the dataset
-                self.process_dataset(dataset)
-
-                if self.generator:
-                    # Update the dataset state to Complete
-                    logger.info(f"Completed {dataset} ({i}/{count})")
-                    self.update_dataset_state(dataset, DatasetState.Complete)
+                logger.info(f"Processing {dataset_set} ({i}/{count})")
+                self.process_set(dataset_set)
             except Exception as e:
-                # Handle errors occurring while retrieving, processing or patching the state for this dataset.
+                # Handle errors occurring while retrieving or processing this dataset set
                 failed += 1
 
-                # Handle the case where we failed retrieving the dataset
-                dataset_id = dataset.id if dataset else item
-
                 if isinstance(e, ErrorResponse):
-                    message = f"An API error occurred while processing dataset {dataset_id}: {e.title} - {e.content}"
+                    message = f"An API error occurred while processing {dataset_set}: {e.title} - {e.content}"
                 else:
-                    message = (
-                        f"Failed running worker on dataset {dataset_id}: {repr(e)}"
-                    )
+                    message = f"Failed running worker on {dataset_set}: {repr(e)}"
 
-                logger.warning(
-                    message,
-                    exc_info=e if self.args.verbose else None,
-                )
-                if dataset and self.generator:
-                    # Try to update the state to Error regardless of the response
-                    with contextlib.suppress(Exception):
-                        self.update_dataset_state(dataset, DatasetState.Error)
-            finally:
-                # Cleanup the dataset artifact if it was downloaded, no matter what
-                if dataset_artifact:
-                    dataset_artifact.unlink(missing_ok=True)
+                logger.warning(message, exc_info=e if self.args.verbose else None)
+
+        # Cleanup the latest downloaded dataset artifact
+        self.cleanup_downloaded_artifact()
 
-        message = f'Ran on {count} dataset{"s"[:count>1]}: {count - failed} completed, {failed} failed'
+        message = f'Ran on {count} set{"s"[:count>1]}: {count - failed} completed, {failed} failed'
         if failed:
             logger.error(message)
             if failed >= count:  # Everything failed!
                 sys.exit(1)
         else:
             logger.info(message)
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/base.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,36 +17,24 @@
     before_sleep_log,
     retry,
     retry_if_exception,
     stop_after_attempt,
     wait_exponential,
 )
 
-from arkindex import ArkindexClient, options_from_env
 from arkindex_worker import logger
 from arkindex_worker.cache import (
     check_version,
     create_tables,
     create_version_table,
     init_cache_db,
     merge_parents_cache,
 )
 from arkindex_worker.utils import close_delete_file, extract_tar_zst_archive
-
-
-def _is_500_error(exc: Exception) -> bool:
-    """
-    Check if an Arkindex API error has a HTTP 5xx error code.
-    Used to retry most API calls in [BaseWorker][arkindex_worker.worker.base.BaseWorker].
-    :param exc: Exception to check
-    """
-    if not isinstance(exc, ErrorResponse):
-        return False
-
-    return 500 <= exc.status_code < 600
+from teklia_toolbox.requests import _get_arkindex_client, _is_500_error
 
 
 class ExtrasDirNotFoundError(Exception):
     """
     Exception raised when the path towards the extras directory is invalid
     """
 
@@ -193,15 +181,15 @@
         raise DeprecationWarning("`worker_version_id` usage is deprecated")
 
     def setup_api_client(self):
         """
         Create an ArkindexClient to make API requests towards Arkindex instances.
         """
         # Build Arkindex API client from environment variables
-        self.api_client = ArkindexClient(**options_from_env())
+        self.api_client = _get_arkindex_client()
         logger.debug(f"Setup Arkindex API client on {self.api_client.document.url}")
 
     def configure_for_developers(self):
         """
         Setup the necessary configuration needed when working in `read_only` mode.
         This is the method called when running a worker locally.
         """
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/classification.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/classification.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/dataset.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from collections.abc import Iterator
 from enum import Enum
 
 from arkindex_worker import logger
 from arkindex_worker.cache import unsupported_cache
-from arkindex_worker.models import Dataset, Element
+from arkindex_worker.models import Dataset, Element, Set
 
 
 class DatasetState(Enum):
     """
     State of a dataset.
     """
 
@@ -33,57 +33,50 @@
     Error = "error"
     """
     The dataset is in error.
     """
 
 
 class DatasetMixin:
-    def list_process_datasets(self) -> Iterator[Dataset]:
+    def list_process_sets(self) -> Iterator[Set]:
         """
-        List datasets associated to the worker's process. This helper is not available in developer mode.
+        List dataset sets associated to the worker's process. This helper is not available in developer mode.
 
-        :returns: An iterator of ``Dataset`` objects built from the ``ListProcessDatasets`` API endpoint.
+        :returns: An iterator of ``Set`` objects built from the ``ListProcessSets`` API endpoint.
         """
         assert not self.is_read_only, "This helper is not available in read-only mode."
 
         results = self.api_client.paginate(
-            "ListProcessDatasets", id=self.process_information["id"]
+            "ListProcessSets", id=self.process_information["id"]
         )
 
         return map(
-            lambda result: Dataset(**result["dataset"], selected_sets=result["sets"]),
+            lambda result: Set(
+                name=result["set_name"], dataset=Dataset(**result["dataset"])
+            ),
             results,
         )
 
-    def list_dataset_elements(self, dataset: Dataset) -> Iterator[tuple[str, Element]]:
+    def list_set_elements(self, dataset_set: Set) -> Iterator[Element]:
         """
-        List elements in a dataset.
+        List elements in a dataset set.
 
-        :param dataset: Dataset to find elements in.
-        :returns: An iterator of tuples built from the ``ListDatasetElements`` API endpoint.
+        :param dataset_set: Set to find elements in.
+        :returns: An iterator of Element built from the ``ListDatasetElements`` API endpoint.
         """
-        assert dataset and isinstance(
-            dataset, Dataset
-        ), "dataset shouldn't be null and should be a Dataset"
-
-        if dataset.sets == dataset.selected_sets:
-            results = self.api_client.paginate("ListDatasetElements", id=dataset.id)
-        else:
-            results = iter(
-                element
-                for selected_set in dataset.selected_sets
-                for element in self.api_client.paginate(
-                    "ListDatasetElements", id=dataset.id, set=selected_set
-                )
-            )
+        assert dataset_set and isinstance(
+            dataset_set, Set
+        ), "dataset_set shouldn't be null and should be a Set"
 
-        return map(
-            lambda result: (result["set"], Element(**result["element"])), results
+        results = self.api_client.paginate(
+            "ListDatasetElements", id=dataset_set.dataset.id, set=dataset_set.name
         )
 
+        return map(lambda result: Element(**result["element"]), results)
+
     @unsupported_cache
     def update_dataset_state(self, dataset: Dataset, state: DatasetState) -> Dataset:
         """
         Partially updates a dataset state through the API.
 
         :param dataset: The dataset to update.
         :param state: State of the dataset.
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/element.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/entity.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,26 +376,28 @@
 
         self.entities = {
             entity["id"]: entity
             for entity in self.api_client.paginate(
                 "ListCorpusEntities", id=self.corpus_id, **query_params
             )
         }
+        count = len(self.entities)
         logger.info(
-            f"Loaded {len(self.entities)} entities in corpus ({self.corpus_id})"
+            f'Loaded {count} entit{"ies" if count > 1 else "y"} in corpus ({self.corpus_id})'
         )
 
     def list_corpus_entity_types(
         self,
     ):
         """
         Loads available entity types in corpus.
         """
         self.entity_types = {
             entity_type["name"]: entity_type["id"]
             for entity_type in self.api_client.paginate(
                 "ListCorpusEntityTypes", id=self.corpus_id
             )
         }
+        count = len(self.entity_types)
         logger.info(
-            f"Loaded {len(self.entity_types)} entity types in corpus ({self.corpus_id})."
+            f'Loaded {count} entity type{"s"[:count>1]} in corpus ({self.corpus_id}).'
         )
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/metadata.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,41 +104,41 @@
                 "worker_run_id": self.worker_run_id,
             },
         )
 
         return metadata["id"]
 
     @unsupported_cache
-    def create_metadatas(
+    def create_metadata_bulk(
         self,
         element: Element | CachedElement,
-        metadatas: list[dict[str, MetaType | str | int | float | None]],
+        metadata_list: list[dict[str, MetaType | str | int | float | None]],
     ) -> list[dict[str, str]]:
         """
         Create multiple metadata on an existing element.
         This method does not support cache.
 
         :param element: The element to create multiple metadata on.
-        :param metadatas: The list of dict whose keys are the following:
+        :param metadata_list: The list of dict whose keys are the following:
             - type: MetaType
             - name: str
             - value: str | int | float
             - entity_id: str | None
         """
         assert element and isinstance(
             element, Element | CachedElement
         ), "element shouldn't be null and should be of type Element or CachedElement"
 
-        assert metadatas and isinstance(
-            metadatas, list
-        ), "type shouldn't be null and should be of type list of Dict"
+        assert metadata_list and isinstance(
+            metadata_list, list
+        ), "metadata_list shouldn't be null and should be of type list of dict"
 
         # Make a copy to avoid modifying the metadata_list argument
         metas = []
-        for index, metadata in enumerate(metadatas):
+        for index, metadata in enumerate(metadata_list):
             assert isinstance(
                 metadata, dict
             ), f"Element at index {index} in metadata_list: Should be of type dict"
 
             assert metadata.get("type") and isinstance(
                 metadata.get("type"), MetaType
             ), "type shouldn't be null and should be of type MetaType"
```

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/task.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/task.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/training.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/transcription.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/transcription.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/arkindex_worker/worker/version.py` & `arkindex-base-worker-0.3.7rc7/arkindex_worker/worker/version.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/pyproject.toml` & `arkindex-base-worker-0.3.7rc7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arkindex-base-worker"
-version = "0.3.7rc6"
+version = "0.3.7rc7"
 description = "Base Worker to easily build Arkindex ML workflows"
 license = { file = "LICENSE" }
 dynamic = ["dependencies", "optional-dependencies"]
 authors = [
     { name = "Teklia", email = "contact@teklia.com" },
 ]
 maintainers = [
@@ -31,14 +31,17 @@
 [project.urls]
 Homepage = "https://workers.arkindex.org"
 Documentation = "https://workers.arkindex.org"
 Repository = "https://gitlab.teklia.com/workers/base-worker"
 "Bug Tracker" = "https://gitlab.teklia.com/workers/base-worker/issues"
 Authors = "https://teklia.com"
 
+[tool.setuptools.packages]
+find = {}
+
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 optional-dependencies = { docs = { file = ["docs-requirements.txt"] } }
 
 [tool.ruff]
 exclude = [".git", "__pycache__"]
 
@@ -71,15 +74,15 @@
 ]
 
 [tool.ruff.lint.per-file-ignores]
 # Ignore `pytest-composite-assertion` rules of `flake8-pytest-style` linter for non-test files
 "arkindex_worker/**/*.py" = ["PT018"]
 
 [tool.ruff.lint.isort]
-known-first-party = ["arkindex", "arkindex_common", "arkindex_worker"]
+known-first-party = ["arkindex", "arkindex_common", "arkindex_worker", "teklia_toolbox"]
 known-third-party = [
     "PIL",
     "apistar",
     "gnupg",
     "peewee",
     "playhouse",
     "pytest",
```

### Comparing `arkindex-base-worker-0.3.7rc6/tests/conftest.py` & `arkindex-base-worker-0.3.7rc7/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     CachedImage,
     CachedTranscription,
     Version,
     create_tables,
     create_version_table,
     init_cache_db,
 )
-from arkindex_worker.models import Artifact, Dataset
+from arkindex_worker.models import Artifact, Dataset, Set
 from arkindex_worker.worker import BaseWorker, DatasetWorker, ElementsWorker
 from arkindex_worker.worker.dataset import DatasetState
 from arkindex_worker.worker.transcription import TextOrientation
 
 FIXTURES_DIR = Path(__file__).resolve().parent / "data"
 SAMPLES_DIR = Path(__file__).resolve().parent / "samples"
 
@@ -593,31 +593,35 @@
 
     return out
 
 
 @pytest.fixture()
 def default_dataset():
     return Dataset(
-        **{
+        {
             "id": "dataset_id",
             "name": "My dataset",
             "description": "A super dataset built by me",
             "sets": ["set_1", "set_2", "set_3", "set_4"],
             "state": DatasetState.Open.value,
             "corpus_id": "corpus_id",
             "creator": "creator@teklia.com",
             "task_id": "11111111-1111-1111-1111-111111111111",
             "created": "2000-01-01T00:00:00Z",
             "updated": "2000-01-01T00:00:00Z",
-        },
-        selected_sets=["set_1", "set_2", "set_3"],
+        }
     )
 
 
 @pytest.fixture()
+def default_train_set(default_dataset):
+    return Set(name="train", dataset=default_dataset)
+
+
+@pytest.fixture()
 def mock_dataset_worker(monkeypatch, mocker, _mock_worker_run_api):
     monkeypatch.setenv("PONOS_TASK", "my_task")
     mocker.patch.object(sys, "argv", ["worker"])
 
     dataset_worker = DatasetWorker()
     dataset_worker.configure()
     dataset_worker.process_information = {"id": PROCESS_ID}
@@ -631,17 +635,18 @@
 def mock_dev_dataset_worker(mocker):
     mocker.patch.object(
         sys,
         "argv",
         [
             "worker",
             "--dev",
-            "--dataset",
-            "11111111-1111-1111-1111-111111111111",
-            "22222222-2222-2222-2222-222222222222",
+            "--set",
+            "11111111-1111-1111-1111-111111111111:train",
+            "11111111-1111-1111-1111-111111111111:val",
+            "22222222-2222-2222-2222-222222222222:my_set",
         ],
     )
 
     dataset_worker = DatasetWorker()
     dataset_worker.configure()
 
     assert dataset_worker.args.dev is True
```

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_base_worker.py` & `arkindex-base-worker-0.3.7rc7/tests/test_base_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_cache.py` & `arkindex-base-worker-0.3.7rc7/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_dataset_worker.py` & `arkindex-base-worker-0.3.7rc7/tests/test_dataset_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,63 @@
 import logging
+import uuid
+from argparse import ArgumentTypeError
 
 import pytest
 from apistar.exceptions import ErrorResponse
 
-from arkindex_worker.worker import MissingDatasetArchive
+from arkindex_worker.models import Dataset, Set
+from arkindex_worker.worker import MissingDatasetArchive, check_dataset_set
 from arkindex_worker.worker.dataset import DatasetState
 from tests.conftest import FIXTURES_DIR, PROCESS_ID
 from tests.test_elements_worker import BASE_API_CALLS
 
+RANDOM_UUID = uuid.uuid4()
+
+
+@pytest.fixture()
+def tmp_archive(tmp_path):
+    archive = tmp_path / "test_archive.tar.zst"
+    archive.touch()
+
+    yield archive
+
+    archive.unlink(missing_ok=True)
+
+
+@pytest.mark.parametrize(
+    ("value", "error"),
+    [("train", ""), (f"{RANDOM_UUID}:train:val", ""), ("not_uuid:train", "")],
+)
+def test_check_dataset_set_errors(value, error):
+    with pytest.raises(ArgumentTypeError, match=error):
+        check_dataset_set(value)
+
+
+def test_check_dataset_set():
+    assert check_dataset_set(f"{RANDOM_UUID}:train") == (RANDOM_UUID, "train")
+
+
+def test_cleanup_downloaded_artifact_no_download(mock_dataset_worker):
+    assert not mock_dataset_worker.downloaded_artifact
+    # Do nothing
+    mock_dataset_worker.cleanup_downloaded_artifact()
+
+
+def test_cleanup_downloaded_artifact(mock_dataset_worker, tmp_archive):
+    mock_dataset_worker.downloaded_artifact = tmp_archive
+
+    assert mock_dataset_worker.downloaded_artifact.exists()
+    # Unlink the downloaded archive
+    mock_dataset_worker.cleanup_downloaded_artifact()
+    assert not mock_dataset_worker.downloaded_artifact.exists()
+
+    # Unlinking again does not raise an error even if the archive no longer exists
+    mock_dataset_worker.cleanup_downloaded_artifact()
+
 
 def test_download_dataset_artifact_list_api_error(
     responses, mock_dataset_worker, default_dataset
 ):
     task_id = default_dataset.task_id
 
     responses.add(
@@ -123,16 +169,23 @@
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
         ("GET", f"http://testserver/api/v1/task/{task_id}/artifacts/"),
     ]
 
 
+@pytest.mark.parametrize("downloaded_cache", [False, True])
 def test_download_dataset_artifact(
-    mocker, tmp_path, responses, mock_dataset_worker, default_dataset
+    mocker,
+    tmp_path,
+    responses,
+    mock_dataset_worker,
+    default_dataset,
+    downloaded_cache,
+    tmp_archive,
 ):
     task_id = default_dataset.task_id
     archive_path = (
         FIXTURES_DIR
         / "extract_parent_archives"
         / "first_parent"
         / "arkindex_data.tar.zst"
@@ -172,383 +225,267 @@
         responses.GET,
         f"http://testserver/api/v1/task/{task_id}/artifact/dataset_id.tar.zst",
         status=200,
         body=archive_path.read_bytes(),
         content_type="application/zstd",
     )
 
-    archive = mock_dataset_worker.download_dataset_artifact(default_dataset)
-    assert archive == tmp_path / "dataset_id.tar.zst"
-    assert archive.read_bytes() == archive_path.read_bytes()
-    archive.unlink()
+    if downloaded_cache:
+        mock_dataset_worker.downloaded_artifact = tmp_archive
+    previous_artifact = mock_dataset_worker.downloaded_artifact
+
+    mock_dataset_worker.download_dataset_artifact(default_dataset)
+
+    # We removed the artifact that was downloaded previously
+    if previous_artifact:
+        assert not previous_artifact.exists()
+
+    assert mock_dataset_worker.downloaded_artifact == tmp_path / "dataset_id.tar.zst"
+    assert (
+        mock_dataset_worker.downloaded_artifact.read_bytes()
+        == archive_path.read_bytes()
+    )
+    mock_dataset_worker.downloaded_artifact.unlink()
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 2
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
         ("GET", f"http://testserver/api/v1/task/{task_id}/artifacts/"),
         ("GET", f"http://testserver/api/v1/task/{task_id}/artifact/dataset_id.tar.zst"),
     ]
 
 
-def test_list_dataset_elements_per_split_api_error(
-    responses, mock_dataset_worker, default_dataset
+def test_download_dataset_artifact_already_exists(
+    mocker, tmp_path, responses, mock_dataset_worker, default_dataset
 ):
-    responses.add(
-        responses.GET,
-        f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_1&with_count=true",
-        status=500,
+    mocker.patch(
+        "arkindex_worker.worker.base.BaseWorker.find_extras_directory",
+        return_value=tmp_path,
     )
+    already_downloaded = tmp_path / "dataset_id.tar.zst"
+    already_downloaded.write_bytes(b"Some content")
+    mock_dataset_worker.downloaded_artifact = already_downloaded
 
-    with pytest.raises(
-        Exception, match="Stopping pagination as data will be incomplete"
-    ):
-        mock_dataset_worker.list_dataset_elements_per_split(default_dataset)
-
-    assert len(responses.calls) == len(BASE_API_CALLS) + 5
-    assert [
-        (call.request.method, call.request.url) for call in responses.calls
-    ] == BASE_API_CALLS + [
-        # The API call is retried 5 times
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_1&with_count=true",
-        ),
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_1&with_count=true",
-        ),
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_1&with_count=true",
-        ),
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_1&with_count=true",
-        ),
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_1&with_count=true",
-        ),
-    ]
-
+    mock_dataset_worker.download_dataset_artifact(default_dataset)
 
-def test_list_dataset_elements_per_split(
-    responses, mock_dataset_worker, default_dataset
-):
-    expected_results = []
-    for selected_set in default_dataset.selected_sets:
-        index = selected_set[-1]
-        expected_results.append(
-            {
-                "set": selected_set,
-                "element": {
-                    "id": str(index) * 4,
-                    "type": "page",
-                    "name": f"Test {index}",
-                    "corpus": {},
-                    "thumbnail_url": None,
-                    "zone": {},
-                    "best_classes": None,
-                    "has_children": None,
-                    "worker_version_id": None,
-                    "worker_run_id": None,
-                },
-            }
-        )
-        responses.add(
-            responses.GET,
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set={selected_set}&with_count=true",
-            status=200,
-            json={
-                "count": 1,
-                "next": None,
-                "results": [expected_results[-1]],
-            },
-        )
+    assert mock_dataset_worker.downloaded_artifact == already_downloaded
+    already_downloaded.unlink()
 
-    assert list(
-        mock_dataset_worker.list_dataset_elements_per_split(default_dataset)
-    ) == [
-        ("set_1", [expected_results[0]["element"]]),
-        ("set_2", [expected_results[1]["element"]]),
-        ("set_3", [expected_results[2]["element"]]),
-    ]
-
-    assert len(responses.calls) == len(BASE_API_CALLS) + 3
+    assert len(responses.calls) == len(BASE_API_CALLS)
     assert [
         (call.request.method, call.request.url) for call in responses.calls
-    ] == BASE_API_CALLS + [
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_1&with_count=true",
-        ),
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_2&with_count=true",
-        ),
-        (
-            "GET",
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set=set_3&with_count=true",
-        ),
-    ]
-
-
-def test_list_datasets_read_only(mock_dev_dataset_worker):
-    assert list(mock_dev_dataset_worker.list_datasets()) == [
-        "11111111-1111-1111-1111-111111111111",
-        "22222222-2222-2222-2222-222222222222",
-    ]
+    ] == BASE_API_CALLS
 
 
-def test_list_datasets_api_error(responses, mock_dataset_worker):
+def test_list_sets_api_error(responses, mock_dataset_worker):
     responses.add(
         responses.GET,
-        f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/",
+        f"http://testserver/api/v1/process/{PROCESS_ID}/sets/",
         status=500,
     )
 
     with pytest.raises(
         Exception, match="Stopping pagination as data will be incomplete"
     ):
-        next(mock_dataset_worker.list_datasets())
+        next(mock_dataset_worker.list_sets())
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 5
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
         # The API call is retried 5 times
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
     ]
 
 
-def test_list_datasets(responses, mock_dataset_worker):
+def test_list_sets(responses, mock_dataset_worker):
     expected_results = [
         {
-            "id": "process_dataset_1",
+            "id": "set_1",
             "dataset": {
                 "id": "dataset_1",
                 "name": "Dataset 1",
                 "description": "My first great dataset",
-                "sets": ["train", "val", "test"],
+                "sets": [
+                    {"id": "set_1", "name": "train"},
+                    {"id": "set_2", "name": "val"},
+                ],
                 "state": "open",
                 "corpus_id": "corpus_id",
                 "creator": "test@teklia.com",
                 "task_id": "task_id_1",
             },
-            "sets": ["test"],
+            "set_name": "train",
         },
         {
-            "id": "process_dataset_2",
+            "id": "set_2",
             "dataset": {
-                "id": "dataset_2",
-                "name": "Dataset 2",
-                "description": "My second great dataset",
-                "sets": ["train", "val"],
-                "state": "complete",
+                "id": "dataset_1",
+                "name": "Dataset 1",
+                "description": "My first great dataset",
+                "sets": [
+                    {"id": "set_1", "name": "train"},
+                    {"id": "set_2", "name": "val"},
+                ],
+                "state": "open",
                 "corpus_id": "corpus_id",
                 "creator": "test@teklia.com",
-                "task_id": "task_id_2",
+                "task_id": "task_id_1",
             },
-            "sets": ["train", "val"],
+            "set_name": "val",
         },
         {
-            "id": "process_dataset_3",
+            "id": "set_3",
             "dataset": {
-                "id": "dataset_3",
-                "name": "Dataset 3 (TRASHME)",
-                "description": "My third dataset, in error",
-                "sets": ["nonsense", "random set"],
-                "state": "error",
+                "id": "dataset_2",
+                "name": "Dataset 2",
+                "description": "My second great dataset",
+                "sets": [{"id": "set_3", "name": "my_set"}],
+                "state": "complete",
                 "corpus_id": "corpus_id",
                 "creator": "test@teklia.com",
-                "task_id": "task_id_3",
+                "task_id": "task_id_2",
             },
-            "sets": ["random set"],
+            "set_name": "my_set",
         },
     ]
     responses.add(
         responses.GET,
-        f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/",
+        f"http://testserver/api/v1/process/{PROCESS_ID}/sets/",
         status=200,
         json={
             "count": 3,
             "next": None,
             "results": expected_results,
         },
     )
 
-    for idx, dataset in enumerate(mock_dataset_worker.list_process_datasets()):
-        assert dataset == {
-            **expected_results[idx]["dataset"],
-            "selected_sets": expected_results[idx]["sets"],
-        }
+    for idx, dataset_set in enumerate(mock_dataset_worker.list_process_sets()):
+        assert isinstance(dataset_set, Set)
+        assert dataset_set.name == expected_results[idx]["set_name"]
+
+        assert isinstance(dataset_set.dataset, Dataset)
+        assert dataset_set.dataset == expected_results[idx]["dataset"]
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 1
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
     ]
 
 
-@pytest.mark.parametrize("generator", [True, False])
-def test_run_no_datasets(mocker, caplog, mock_dataset_worker, generator):
-    mocker.patch("arkindex_worker.worker.DatasetWorker.list_datasets", return_value=[])
-    mock_dataset_worker.generator = generator
+def test_list_sets_retrieve_dataset_api_error(
+    responses, mock_dev_dataset_worker, default_dataset
+):
+    mock_dev_dataset_worker.args.set = [
+        (default_dataset.id, "train"),
+        (default_dataset.id, "val"),
+    ]
 
-    with pytest.raises(SystemExit):
-        mock_dataset_worker.run()
+    responses.add(
+        responses.GET,
+        f"http://testserver/api/v1/datasets/{default_dataset.id}/",
+        status=500,
+    )
 
-    assert [(level, message) for _, level, message in caplog.record_tuples] == [
-        (logging.INFO, "Loaded Worker Fake worker @ 123412 from API"),
-        (logging.WARNING, "No datasets to process, stopping."),
+    with pytest.raises(ErrorResponse):
+        next(mock_dev_dataset_worker.list_sets())
+
+    assert len(responses.calls) == 5
+    assert [(call.request.method, call.request.url) for call in responses.calls] == [
+        # The API call is retried 5 times
+        ("GET", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
+        ("GET", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
+        ("GET", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
+        ("GET", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
+        ("GET", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
     ]
 
 
-@pytest.mark.parametrize(
-    ("generator", "error"),
-    [
-        (True, "When generating a new dataset, its state should be Open or Error."),
-        (False, "When processing an existing dataset, its state should be Complete."),
-    ],
-)
-def test_run_initial_dataset_state_error(
-    mocker, responses, caplog, mock_dataset_worker, default_dataset, generator, error
-):
-    default_dataset.state = DatasetState.Building.value
-    mocker.patch(
-        "arkindex_worker.worker.DatasetWorker.list_datasets",
-        return_value=[default_dataset],
+def test_list_sets_read_only(responses, mock_dev_dataset_worker, default_dataset):
+    mock_dev_dataset_worker.args.set = [
+        (default_dataset.id, "train"),
+        (default_dataset.id, "val"),
+    ]
+
+    responses.add(
+        responses.GET,
+        f"http://testserver/api/v1/datasets/{default_dataset.id}/",
+        status=200,
+        json=default_dataset,
     )
-    mock_dataset_worker.generator = generator
 
-    extra_call = []
-    if generator:
-        responses.add(
-            responses.PATCH,
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/",
-            status=200,
-            json={},
-        )
-        extra_call = [
-            ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ]
+    assert list(mock_dev_dataset_worker.list_sets()) == [
+        Set(name="train", dataset=default_dataset),
+        Set(name="val", dataset=default_dataset),
+    ]
+
+    assert len(responses.calls) == 1
+    assert [(call.request.method, call.request.url) for call in responses.calls] == [
+        ("GET", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
+    ]
+
+
+def test_run_no_sets(mocker, caplog, mock_dataset_worker):
+    mocker.patch("arkindex_worker.worker.DatasetWorker.list_sets", return_value=[])
 
     with pytest.raises(SystemExit):
         mock_dataset_worker.run()
 
-    assert len(responses.calls) == len(BASE_API_CALLS) * 2 + len(extra_call)
-    assert [
-        (call.request.method, call.request.url) for call in responses.calls
-    ] == BASE_API_CALLS * 2 + extra_call
-
     assert [(level, message) for _, level, message in caplog.record_tuples] == [
         (logging.INFO, "Loaded Worker Fake worker @ 123412 from API"),
-        (
-            logging.WARNING,
-            f"Failed running worker on dataset dataset_id: AssertionError('{error}')",
-        ),
-    ] + (
-        [
-            (
-                logging.WARNING,
-                "This API helper `update_dataset_state` did not update the cache database",
-            )
-        ]
-        if generator
-        else []
-    ) + [
-        (logging.ERROR, "Ran on 1 dataset: 0 completed, 1 failed"),
+        (logging.WARNING, "No sets to process, stopping."),
     ]
 
 
-def test_run_update_dataset_state_api_error(
+def test_run_initial_dataset_state_error(
     mocker, responses, caplog, mock_dataset_worker, default_dataset
 ):
+    default_dataset.state = DatasetState.Building.value
     mocker.patch(
-        "arkindex_worker.worker.DatasetWorker.list_datasets",
-        return_value=[default_dataset],
-    )
-    mock_dataset_worker.generator = True
-
-    responses.add(
-        responses.PATCH,
-        f"http://testserver/api/v1/datasets/{default_dataset.id}/",
-        status=500,
+        "arkindex_worker.worker.DatasetWorker.list_sets",
+        return_value=[Set(name="train", dataset=default_dataset)],
     )
 
     with pytest.raises(SystemExit):
         mock_dataset_worker.run()
 
-    assert len(responses.calls) == len(BASE_API_CALLS) * 2 + 10
+    assert len(responses.calls) == len(BASE_API_CALLS) * 2
     assert [
         (call.request.method, call.request.url) for call in responses.calls
-    ] == BASE_API_CALLS * 2 + [
-        # We retry 5 times the API call to update the Dataset as Building
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        # We retry 5 times the API call to update the Dataset as in Error
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-    ]
+    ] == BASE_API_CALLS * 2
 
-    retries = [3.0, 4.0, 8.0, 16.0]
     assert [(level, message) for _, level, message in caplog.record_tuples] == [
         (logging.INFO, "Loaded Worker Fake worker @ 123412 from API"),
-        (logging.INFO, "Processing Dataset (dataset_id) (1/1)"),
-        (logging.INFO, "Building Dataset (dataset_id) (1/1)"),
-        *[
-            (
-                logging.INFO,
-                f"Retrying arkindex_worker.worker.base.BaseWorker.request in {retry} seconds as it raised ErrorResponse: .",
-            )
-            for retry in retries
-        ],
         (
             logging.WARNING,
-            "An API error occurred while processing dataset dataset_id: 500 Internal Server Error - None",
-        ),
-        *[
-            (
-                logging.INFO,
-                f"Retrying arkindex_worker.worker.base.BaseWorker.request in {retry} seconds as it raised ErrorResponse: .",
-            )
-            for retry in retries
-        ],
-        (
-            logging.ERROR,
-            "Ran on 1 dataset: 0 completed, 1 failed",
+            "Failed running worker on Set (train) from Dataset (dataset_id): AssertionError('When processing a set, its dataset state should be Complete.')",
         ),
+        (logging.ERROR, "Ran on 1 set: 0 completed, 1 failed"),
     ]
 
 
 def test_run_download_dataset_artifact_api_error(
     mocker,
     tmp_path,
     responses,
     caplog,
     mock_dataset_worker,
     default_dataset,
 ):
     default_dataset.state = DatasetState.Complete.value
-
     mocker.patch(
-        "arkindex_worker.worker.DatasetWorker.list_datasets",
-        return_value=[default_dataset],
+        "arkindex_worker.worker.DatasetWorker.list_sets",
+        return_value=[Set(name="train", dataset=default_dataset)],
     )
     mocker.patch(
         "arkindex_worker.worker.base.BaseWorker.find_extras_directory",
         return_value=tmp_path,
     )
 
     responses.add(
@@ -570,47 +507,49 @@
         ("GET", f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/"),
         ("GET", f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/"),
         ("GET", f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/"),
     ]
 
     assert [(level, message) for _, level, message in caplog.record_tuples] == [
         (logging.INFO, "Loaded Worker Fake worker @ 123412 from API"),
-        (logging.INFO, "Processing Dataset (dataset_id) (1/1)"),
-        (logging.INFO, "Downloading data for Dataset (dataset_id) (1/1)"),
+        (
+            logging.INFO,
+            "Retrieving data for Set (train) from Dataset (dataset_id) (1/1)",
+        ),
+        (logging.INFO, "Downloading artifact for Dataset (dataset_id)"),
         *[
             (
                 logging.INFO,
                 f"Retrying arkindex_worker.worker.base.BaseWorker.request in {retry} seconds as it raised ErrorResponse: .",
             )
             for retry in [3.0, 4.0, 8.0, 16.0]
         ],
         (
             logging.WARNING,
-            "An API error occurred while processing dataset dataset_id: 500 Internal Server Error - None",
+            "An API error occurred while processing Set (train) from Dataset (dataset_id): 500 Internal Server Error - None",
         ),
         (
             logging.ERROR,
-            "Ran on 1 dataset: 0 completed, 1 failed",
+            "Ran on 1 set: 0 completed, 1 failed",
         ),
     ]
 
 
 def test_run_no_downloaded_artifact_error(
     mocker,
     tmp_path,
     responses,
     caplog,
     mock_dataset_worker,
     default_dataset,
 ):
     default_dataset.state = DatasetState.Complete.value
-
     mocker.patch(
-        "arkindex_worker.worker.DatasetWorker.list_datasets",
-        return_value=[default_dataset],
+        "arkindex_worker.worker.DatasetWorker.list_sets",
+        return_value=[Set(name="train", dataset=default_dataset)],
     )
     mocker.patch(
         "arkindex_worker.worker.base.BaseWorker.find_extras_directory",
         return_value=tmp_path,
     )
 
     responses.add(
@@ -628,220 +567,159 @@
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS * 2 + [
         ("GET", f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/"),
     ]
 
     assert [(level, message) for _, level, message in caplog.record_tuples] == [
         (logging.INFO, "Loaded Worker Fake worker @ 123412 from API"),
-        (logging.INFO, "Processing Dataset (dataset_id) (1/1)"),
-        (logging.INFO, "Downloading data for Dataset (dataset_id) (1/1)"),
+        (
+            logging.INFO,
+            "Retrieving data for Set (train) from Dataset (dataset_id) (1/1)",
+        ),
+        (logging.INFO, "Downloading artifact for Dataset (dataset_id)"),
         (
             logging.WARNING,
-            "Failed running worker on dataset dataset_id: MissingDatasetArchive('The dataset compressed archive artifact was not found.')",
+            "Failed running worker on Set (train) from Dataset (dataset_id): MissingDatasetArchive('The dataset compressed archive artifact was not found.')",
         ),
         (
             logging.ERROR,
-            "Ran on 1 dataset: 0 completed, 1 failed",
+            "Ran on 1 set: 0 completed, 1 failed",
         ),
     ]
 
 
-@pytest.mark.parametrize(
-    ("generator", "state"), [(True, DatasetState.Open), (False, DatasetState.Complete)]
-)
 def test_run(
     mocker,
     tmp_path,
     responses,
     caplog,
     mock_dataset_worker,
     default_dataset,
     default_artifact,
-    generator,
-    state,
 ):
-    mock_dataset_worker.generator = generator
-    default_dataset.state = state.value
-
+    default_dataset.state = DatasetState.Complete.value
     mocker.patch(
-        "arkindex_worker.worker.DatasetWorker.list_datasets",
-        return_value=[default_dataset],
+        "arkindex_worker.worker.DatasetWorker.list_sets",
+        return_value=[Set(name="train", dataset=default_dataset)],
     )
     mocker.patch(
         "arkindex_worker.worker.base.BaseWorker.find_extras_directory",
         return_value=tmp_path,
     )
-    mock_process = mocker.patch("arkindex_worker.worker.DatasetWorker.process_dataset")
+    mock_process = mocker.patch("arkindex_worker.worker.DatasetWorker.process_set")
 
-    extra_calls = []
-    extra_logs = []
-    if generator:
-        responses.add(
-            responses.PATCH,
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/",
-            status=200,
-            json={},
-        )
-        extra_calls += [
-            ("PATCH", f"http://testserver/api/v1/datasets/{default_dataset.id}/"),
-        ] * 2
-        extra_logs += [
-            (logging.INFO, "Building Dataset (dataset_id) (1/1)"),
-            (
-                logging.WARNING,
-                "This API helper `update_dataset_state` did not update the cache database",
-            ),
-            (logging.INFO, "Completed Dataset (dataset_id) (1/1)"),
-            (
-                logging.WARNING,
-                "This API helper `update_dataset_state` did not update the cache database",
-            ),
-        ]
-    else:
-        archive_path = (
-            FIXTURES_DIR
-            / "extract_parent_archives"
-            / "first_parent"
-            / "arkindex_data.tar.zst"
-        )
-        responses.add(
-            responses.GET,
-            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
-            status=200,
-            json=[default_artifact],
-        )
-        responses.add(
-            responses.GET,
-            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
-            status=200,
-            body=archive_path.read_bytes(),
-            content_type="application/zstd",
-        )
-        extra_calls += [
-            (
-                "GET",
-                f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
-            ),
-            (
-                "GET",
-                f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
-            ),
-        ]
-        extra_logs += [
-            (logging.INFO, "Downloading data for Dataset (dataset_id) (1/1)"),
-        ]
+    archive_path = (
+        FIXTURES_DIR
+        / "extract_parent_archives"
+        / "first_parent"
+        / "arkindex_data.tar.zst"
+    )
+    responses.add(
+        responses.GET,
+        f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
+        status=200,
+        json=[default_artifact],
+    )
+    responses.add(
+        responses.GET,
+        f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
+        status=200,
+        body=archive_path.read_bytes(),
+        content_type="application/zstd",
+    )
 
     mock_dataset_worker.run()
 
     assert mock_process.call_count == 1
 
-    assert len(responses.calls) == len(BASE_API_CALLS) * 2 + len(extra_calls)
+    assert len(responses.calls) == len(BASE_API_CALLS) * 2 + 2
     assert [
         (call.request.method, call.request.url) for call in responses.calls
-    ] == BASE_API_CALLS * 2 + extra_calls
+    ] == BASE_API_CALLS * 2 + [
+        (
+            "GET",
+            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
+        ),
+        (
+            "GET",
+            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
+        ),
+    ]
 
     assert [(level, message) for _, level, message in caplog.record_tuples] == [
         (logging.INFO, "Loaded Worker Fake worker @ 123412 from API"),
-        (logging.INFO, "Processing Dataset (dataset_id) (1/1)"),
-        *extra_logs,
-        (logging.INFO, "Ran on 1 dataset: 1 completed, 0 failed"),
+        (
+            logging.INFO,
+            "Retrieving data for Set (train) from Dataset (dataset_id) (1/1)",
+        ),
+        (logging.INFO, "Downloading artifact for Dataset (dataset_id)"),
+        (logging.INFO, "Processing Set (train) from Dataset (dataset_id) (1/1)"),
+        (logging.INFO, "Ran on 1 set: 1 completed, 0 failed"),
     ]
 
 
-@pytest.mark.parametrize(
-    ("generator", "state"), [(True, DatasetState.Open), (False, DatasetState.Complete)]
-)
 def test_run_read_only(
     mocker,
     tmp_path,
     responses,
     caplog,
     mock_dev_dataset_worker,
     default_dataset,
     default_artifact,
-    generator,
-    state,
 ):
-    mock_dev_dataset_worker.generator = generator
-    default_dataset.state = state.value
-
+    default_dataset.state = DatasetState.Complete.value
     mocker.patch(
-        "arkindex_worker.worker.DatasetWorker.list_datasets",
-        return_value=[default_dataset.id],
+        "arkindex_worker.worker.DatasetWorker.list_sets",
+        return_value=[Set(name="train", dataset=default_dataset)],
     )
     mocker.patch(
         "arkindex_worker.worker.base.BaseWorker.find_extras_directory",
         return_value=tmp_path,
     )
-    mock_process = mocker.patch("arkindex_worker.worker.DatasetWorker.process_dataset")
+    mock_process = mocker.patch("arkindex_worker.worker.DatasetWorker.process_set")
 
+    archive_path = (
+        FIXTURES_DIR
+        / "extract_parent_archives"
+        / "first_parent"
+        / "arkindex_data.tar.zst"
+    )
     responses.add(
         responses.GET,
-        f"http://testserver/api/v1/datasets/{default_dataset.id}/",
+        f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
         status=200,
-        json=default_dataset,
+        json=[default_artifact],
+    )
+    responses.add(
+        responses.GET,
+        f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
+        status=200,
+        body=archive_path.read_bytes(),
+        content_type="application/zstd",
     )
-
-    extra_calls = []
-    extra_logs = []
-    if generator:
-        extra_logs += [
-            (logging.INFO, "Building Dataset (dataset_id) (1/1)"),
-            (
-                logging.WARNING,
-                "Cannot update dataset as this worker is in read-only mode",
-            ),
-            (logging.INFO, "Completed Dataset (dataset_id) (1/1)"),
-            (
-                logging.WARNING,
-                "Cannot update dataset as this worker is in read-only mode",
-            ),
-        ]
-    else:
-        archive_path = (
-            FIXTURES_DIR
-            / "extract_parent_archives"
-            / "first_parent"
-            / "arkindex_data.tar.zst"
-        )
-        responses.add(
-            responses.GET,
-            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
-            status=200,
-            json=[default_artifact],
-        )
-        responses.add(
-            responses.GET,
-            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
-            status=200,
-            body=archive_path.read_bytes(),
-            content_type="application/zstd",
-        )
-        extra_calls += [
-            (
-                "GET",
-                f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
-            ),
-            (
-                "GET",
-                f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
-            ),
-        ]
-        extra_logs += [
-            (logging.INFO, "Downloading data for Dataset (dataset_id) (1/1)"),
-        ]
 
     mock_dev_dataset_worker.run()
 
     assert mock_process.call_count == 1
 
-    assert len(responses.calls) == 1 + len(extra_calls)
+    assert len(responses.calls) == 2
     assert [(call.request.method, call.request.url) for call in responses.calls] == [
-        ("GET", f"http://testserver/api/v1/datasets/{default_dataset.id}/")
-    ] + extra_calls
+        (
+            "GET",
+            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifacts/",
+        ),
+        (
+            "GET",
+            f"http://testserver/api/v1/task/{default_dataset.task_id}/artifact/dataset_id.tar.zst",
+        ),
+    ]
 
     assert [(level, message) for _, level, message in caplog.record_tuples] == [
         (logging.WARNING, "Running without any extra configuration"),
-        (logging.INFO, "Processing Dataset (dataset_id) (1/1)"),
-        *extra_logs,
-        (logging.INFO, "Ran on 1 dataset: 1 completed, 0 failed"),
+        (
+            logging.INFO,
+            "Retrieving data for Set (train) from Dataset (dataset_id) (1/1)",
+        ),
+        (logging.INFO, "Downloading artifact for Dataset (dataset_id)"),
+        (logging.INFO, "Processing Set (train) from Dataset (dataset_id) (1/1)"),
+        (logging.INFO, "Ran on 1 set: 1 completed, 0 failed"),
     ]
```

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_element.py` & `arkindex-base-worker-0.3.7rc7/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_classifications.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_cli.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_dataset.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,168 @@
 import json
 import logging
 
 import pytest
 from apistar.exceptions import ErrorResponse
 
-from arkindex_worker.models import Dataset
+from arkindex_worker.models import Dataset, Element, Set
 from arkindex_worker.worker.dataset import DatasetState
 from tests.conftest import PROCESS_ID
 from tests.test_elements_worker import BASE_API_CALLS
 
 
-def test_list_process_datasets_readonly_error(mock_dataset_worker):
+def test_list_process_sets_readonly_error(mock_dataset_worker):
     # Set worker in read_only mode
     mock_dataset_worker.worker_run_id = None
     assert mock_dataset_worker.is_read_only
 
     with pytest.raises(
         AssertionError, match="This helper is not available in read-only mode."
     ):
-        mock_dataset_worker.list_process_datasets()
+        mock_dataset_worker.list_process_sets()
 
 
-def test_list_process_datasets_api_error(responses, mock_dataset_worker):
+def test_list_process_sets_api_error(responses, mock_dataset_worker):
     responses.add(
         responses.GET,
-        f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/",
+        f"http://testserver/api/v1/process/{PROCESS_ID}/sets/",
         status=500,
     )
 
     with pytest.raises(
         Exception, match="Stopping pagination as data will be incomplete"
     ):
-        next(mock_dataset_worker.list_process_datasets())
+        next(mock_dataset_worker.list_process_sets())
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 5
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
         # The API call is retried 5 times
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
     ]
 
 
-def test_list_process_datasets(
+def test_list_process_sets(
     responses,
     mock_dataset_worker,
 ):
     expected_results = [
         {
-            "id": "process_dataset_1",
+            "id": "set_1",
             "dataset": {
                 "id": "dataset_1",
                 "name": "Dataset 1",
                 "description": "My first great dataset",
-                "sets": ["train", "val", "test"],
+                "sets": [
+                    {"id": "set_1", "name": "train"},
+                    {"id": "set_2", "name": "val"},
+                ],
                 "state": "open",
                 "corpus_id": "corpus_id",
                 "creator": "test@teklia.com",
                 "task_id": "task_id_1",
             },
-            "sets": ["test"],
+            "set_name": "train",
         },
         {
-            "id": "process_dataset_2",
+            "id": "set_2",
             "dataset": {
-                "id": "dataset_2",
-                "name": "Dataset 2",
-                "description": "My second great dataset",
-                "sets": ["train", "val"],
-                "state": "complete",
+                "id": "dataset_1",
+                "name": "Dataset 1",
+                "description": "My first great dataset",
+                "sets": [
+                    {"id": "set_1", "name": "train"},
+                    {"id": "set_2", "name": "val"},
+                ],
+                "state": "open",
                 "corpus_id": "corpus_id",
                 "creator": "test@teklia.com",
-                "task_id": "task_id_2",
+                "task_id": "task_id_1",
             },
-            "sets": ["train", "val"],
+            "set_name": "val",
         },
         {
-            "id": "process_dataset_3",
+            "id": "set_3",
             "dataset": {
-                "id": "dataset_3",
-                "name": "Dataset 3 (TRASHME)",
-                "description": "My third dataset, in error",
-                "sets": ["nonsense", "random set"],
-                "state": "error",
+                "id": "dataset_2",
+                "name": "Dataset 2",
+                "description": "My second great dataset",
+                "sets": [{"id": "set_3", "name": "my_set"}],
+                "state": "complete",
                 "corpus_id": "corpus_id",
                 "creator": "test@teklia.com",
-                "task_id": "task_id_3",
+                "task_id": "task_id_2",
             },
-            "sets": ["random set"],
+            "set_name": "my_set",
         },
     ]
     responses.add(
         responses.GET,
-        f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/",
+        f"http://testserver/api/v1/process/{PROCESS_ID}/sets/",
         status=200,
         json={
             "count": 3,
             "next": None,
             "results": expected_results,
         },
     )
 
-    for idx, dataset in enumerate(mock_dataset_worker.list_process_datasets()):
-        assert isinstance(dataset, Dataset)
-        assert dataset == {
-            **expected_results[idx]["dataset"],
-            "selected_sets": expected_results[idx]["sets"],
-        }
+    for idx, dataset_set in enumerate(mock_dataset_worker.list_process_sets()):
+        assert isinstance(dataset_set, Set)
+        assert dataset_set.name == expected_results[idx]["set_name"]
+
+        assert isinstance(dataset_set.dataset, Dataset)
+        assert dataset_set.dataset == expected_results[idx]["dataset"]
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 1
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
-        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/datasets/"),
+        ("GET", f"http://testserver/api/v1/process/{PROCESS_ID}/sets/"),
     ]
 
 
 @pytest.mark.parametrize(
     ("payload", "error"),
     [
-        # Dataset
+        # Set
         (
-            {"dataset": None},
-            "dataset shouldn't be null and should be a Dataset",
+            {"dataset_set": None},
+            "dataset_set shouldn't be null and should be a Set",
         ),
         (
-            {"dataset": "not Dataset type"},
-            "dataset shouldn't be null and should be a Dataset",
+            {"dataset_set": "not Set type"},
+            "dataset_set shouldn't be null and should be a Set",
         ),
     ],
 )
-def test_list_dataset_elements_wrong_param_dataset(mock_dataset_worker, payload, error):
+def test_list_set_elements_wrong_param_dataset_set(mock_dataset_worker, payload, error):
     with pytest.raises(AssertionError, match=error):
-        mock_dataset_worker.list_dataset_elements(**payload)
+        mock_dataset_worker.list_set_elements(**payload)
 
 
-@pytest.mark.parametrize(
-    "sets",
-    [
-        ["set_1"],
-        ["set_1", "set_2", "set_3"],
-        ["set_1", "set_2", "set_3", "set_4"],
-    ],
-)
-def test_list_dataset_elements_api_error(
-    responses, mock_dataset_worker, sets, default_dataset
+def test_list_set_elements_api_error(
+    responses, mock_dataset_worker, default_dataset, default_train_set
 ):
-    default_dataset.selected_sets = sets
-    query_params = (
-        "?with_count=true"
-        if sets == default_dataset.sets
-        else "?set=set_1&with_count=true"
-    )
+    query_params = f"?set={default_train_set.name}&with_count=true"
     responses.add(
         responses.GET,
         f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/{query_params}",
         status=500,
     )
 
     with pytest.raises(
         Exception, match="Stopping pagination as data will be incomplete"
     ):
-        next(mock_dataset_worker.list_dataset_elements(dataset=default_dataset))
+        next(mock_dataset_worker.list_set_elements(dataset_set=default_train_set))
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 5
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
         # The API call is retried 5 times
         (
@@ -191,107 +184,68 @@
         (
             "GET",
             f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/{query_params}",
         ),
     ]
 
 
-@pytest.mark.parametrize(
-    "sets",
-    [
-        ["set_1"],
-        ["set_1", "set_2", "set_3"],
-        ["set_1", "set_2", "set_3", "set_4"],
-    ],
-)
-def test_list_dataset_elements(
+def test_list_set_elements(
     responses,
     mock_dataset_worker,
-    sets,
     default_dataset,
+    default_train_set,
 ):
-    default_dataset.selected_sets = sets
-
-    dataset_elements = []
-    for split in default_dataset.sets:
-        index = split[-1]
-        dataset_elements.append(
-            {
-                "set": split,
-                "element": {
-                    "id": str(index) * 4,
-                    "type": "page",
-                    "name": f"Test {index}",
-                    "corpus": {},
-                    "thumbnail_url": None,
-                    "zone": {},
-                    "best_classes": None,
-                    "has_children": None,
-                    "worker_version_id": None,
-                    "worker_run_id": None,
-                },
-            }
-        )
-        if split == "set_1":
-            dataset_elements.append({**dataset_elements[-1]})
-            dataset_elements[-1]["element"]["name"] = f"Test {index} (bis)"
-
-    # All sets are selected, we call the unfiltered endpoint once
-    if default_dataset.sets == default_dataset.selected_sets:
-        expected_results = dataset_elements
-        responses.add(
-            responses.GET,
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?with_count=true",
-            status=200,
-            json={
-                "count": len(expected_results),
-                "next": None,
-                "results": expected_results,
+    expected_results = [
+        {
+            "set": "train",
+            "element": {
+                "id": "element_1",
+                "type": "page",
+                "name": "1",
+                "corpus": {},
+                "thumbnail_url": None,
+                "zone": {},
+                "best_classes": None,
+                "has_children": None,
+                "worker_version_id": None,
+                "worker_run_id": None,
             },
-        )
-        expected_calls = [
-            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?with_count=true"
-        ]
-
-    # Not all sets are selected, we call the filtered endpoint multiple times, once per set
-    else:
-        expected_results, expected_calls = [], []
-        for selected_set in default_dataset.selected_sets:
-            partial_results = [
-                element
-                for element in dataset_elements
-                if element["set"] == selected_set
-            ]
-            expected_results += partial_results
-            responses.add(
-                responses.GET,
-                f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set={selected_set}&with_count=true",
-                status=200,
-                json={
-                    "count": len(partial_results),
-                    "next": None,
-                    "results": partial_results,
-                },
-            )
-            expected_calls += [
-                f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/?set={selected_set}&with_count=true"
-            ]
+        }
+    ]
+    expected_results.append({**expected_results[-1]})
+    expected_results[-1]["element"]["id"] = "element_2"
+    expected_results[-1]["element"]["name"] = "2"
+
+    query_params = f"?set={default_train_set.name}&with_count=true"
+    responses.add(
+        responses.GET,
+        f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/{query_params}",
+        status=200,
+        json={
+            "count": 2,
+            "next": None,
+            "results": expected_results,
+        },
+    )
 
     for idx, element in enumerate(
-        mock_dataset_worker.list_dataset_elements(dataset=default_dataset)
+        mock_dataset_worker.list_set_elements(dataset_set=default_train_set)
     ):
-        assert element == (
-            expected_results[idx]["set"],
-            expected_results[idx]["element"],
-        )
+        assert isinstance(element, Element)
+        assert element == expected_results[idx]["element"]
 
-    assert len(responses.calls) == len(BASE_API_CALLS) + len(expected_calls)
+    assert len(responses.calls) == len(BASE_API_CALLS) + 1
     assert [
         (call.request.method, call.request.url) for call in responses.calls
-    ] == BASE_API_CALLS + [("GET", expected_call) for expected_call in expected_calls]
+    ] == BASE_API_CALLS + [
+        (
+            "GET",
+            f"http://testserver/api/v1/datasets/{default_dataset.id}/elements/{query_params}",
+        )
+    ]
 
 
 @pytest.mark.parametrize(
     ("payload", "error"),
     [
         # Dataset
         (
```

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_elements.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_elements.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_entities.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_metadata.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
                 "name": "fake_name",
                 "value": "fake_value",
                 "entity_id": "fake_entity_id",
             }
         ],
     ],
 )
-def test_create_metadatas(responses, mock_elements_worker, metadata_list):
+def test_create_metadata_bulk(responses, mock_elements_worker, metadata_list):
     element = Element({"id": "12341234-1234-1234-1234-123412341234"})
     responses.add(
         responses.POST,
         "http://testserver/api/v1/element/12341234-1234-1234-1234-123412341234/metadata/bulk/",
         status=201,
         json={
             "worker_run_id": "56785678-5678-5678-5678-567856785678",
@@ -276,15 +276,15 @@
                     "dates": [],
                     "entity_id": metadata_list[0].get("entity_id"),
                 }
             ],
         },
     )
 
-    created_metadata_list = mock_elements_worker.create_metadatas(
+    created_metadata_list = mock_elements_worker.create_metadata_bulk(
         element, metadata_list
     )
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 1
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
@@ -323,15 +323,15 @@
                 "name": "fake_name",
                 "value": "fake_value",
                 "entity_id": "fake_entity_id",
             }
         ],
     ],
 )
-def test_create_metadatas_cached_element(
+def test_create_metadata_bulk_cached_element(
     responses, mock_elements_worker_with_cache, metadata_list
 ):
     element = CachedElement.create(
         id="12341234-1234-1234-1234-123412341234", type="thing"
     )
     responses.add(
         responses.POST,
@@ -348,15 +348,15 @@
                     "dates": [],
                     "entity_id": metadata_list[0].get("entity_id"),
                 }
             ],
         },
     )
 
-    created_metadata_list = mock_elements_worker_with_cache.create_metadatas(
+    created_metadata_list = mock_elements_worker_with_cache.create_metadata_bulk(
         element, metadata_list
     )
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 1
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
@@ -382,90 +382,90 @@
             "dates": [],
             "entity_id": metadata_list[0].get("entity_id"),
         }
     ]
 
 
 @pytest.mark.parametrize("wrong_element", [None, "not_element_type", 1234, 12.5])
-def test_create_metadatas_wrong_element(mock_elements_worker, wrong_element):
+def test_create_metadata_bulk_wrong_element(mock_elements_worker, wrong_element):
     wrong_metadata_list = [
         {"type": MetaType.Text, "name": "fake_name", "value": "fake_value"}
     ]
     with pytest.raises(
         AssertionError,
         match="element shouldn't be null and should be of type Element or CachedElement",
     ):
-        mock_elements_worker.create_metadatas(
-            element=wrong_element, metadatas=wrong_metadata_list
+        mock_elements_worker.create_metadata_bulk(
+            element=wrong_element, metadata_list=wrong_metadata_list
         )
 
 
 @pytest.mark.parametrize("wrong_type", [None, "not_metadata_type", 1234, 12.5])
-def test_create_metadatas_wrong_type(mock_elements_worker, wrong_type):
+def test_create_metadata_bulk_wrong_type(mock_elements_worker, wrong_type):
     element = Element({"id": "12341234-1234-1234-1234-123412341234"})
     wrong_metadata_list = [
         {"type": wrong_type, "name": "fake_name", "value": "fake_value"}
     ]
     with pytest.raises(
         AssertionError, match="type shouldn't be null and should be of type MetaType"
     ):
-        mock_elements_worker.create_metadatas(
-            element=element, metadatas=wrong_metadata_list
+        mock_elements_worker.create_metadata_bulk(
+            element=element, metadata_list=wrong_metadata_list
         )
 
 
 @pytest.mark.parametrize("wrong_name", [None, 1234, 12.5, [1, 2, 3, 4]])
-def test_create_metadatas_wrong_name(mock_elements_worker, wrong_name):
+def test_create_metadata_bulk_wrong_name(mock_elements_worker, wrong_name):
     element = Element({"id": "fake_element_id"})
     wrong_metadata_list = [
         {"type": MetaType.Text, "name": wrong_name, "value": "fake_value"}
     ]
     with pytest.raises(
         AssertionError, match="name shouldn't be null and should be of type str"
     ):
-        mock_elements_worker.create_metadatas(
-            element=element, metadatas=wrong_metadata_list
+        mock_elements_worker.create_metadata_bulk(
+            element=element, metadata_list=wrong_metadata_list
         )
 
 
 @pytest.mark.parametrize("wrong_value", [None, [1, 2, 3, 4]])
-def test_create_metadatas_wrong_value(mock_elements_worker, wrong_value):
+def test_create_metadata_bulk_wrong_value(mock_elements_worker, wrong_value):
     element = Element({"id": "fake_element_id"})
     wrong_metadata_list = [
         {"type": MetaType.Text, "name": "fake_name", "value": wrong_value}
     ]
     with pytest.raises(
         AssertionError,
         match=re.escape(
             "value shouldn't be null and should be of type (str or float or int)"
         ),
     ):
-        mock_elements_worker.create_metadatas(
-            element=element, metadatas=wrong_metadata_list
+        mock_elements_worker.create_metadata_bulk(
+            element=element, metadata_list=wrong_metadata_list
         )
 
 
 @pytest.mark.parametrize("wrong_entity", [[1, 2, 3, 4], 1234, 12.5])
-def test_create_metadatas_wrong_entity(mock_elements_worker, wrong_entity):
+def test_create_metadata_bulk_wrong_entity(mock_elements_worker, wrong_entity):
     element = Element({"id": "fake_element_id"})
     wrong_metadata_list = [
         {
             "type": MetaType.Text,
             "name": "fake_name",
             "value": "fake_value",
             "entity_id": wrong_entity,
         }
     ]
     with pytest.raises(AssertionError, match="entity_id should be None or a str"):
-        mock_elements_worker.create_metadatas(
-            element=element, metadatas=wrong_metadata_list
+        mock_elements_worker.create_metadata_bulk(
+            element=element, metadata_list=wrong_metadata_list
         )
 
 
-def test_create_metadatas_api_error(responses, mock_elements_worker):
+def test_create_metadata_bulk_api_error(responses, mock_elements_worker):
     element = Element({"id": "12341234-1234-1234-1234-123412341234"})
     metadata_list = [
         {
             "type": MetaType.Text,
             "name": "fake_name",
             "value": "fake_value",
             "entity_id": "fake_entity_id",
@@ -474,15 +474,15 @@
     responses.add(
         responses.POST,
         "http://testserver/api/v1/element/12341234-1234-1234-1234-123412341234/metadata/bulk/",
         status=500,
     )
 
     with pytest.raises(ErrorResponse):
-        mock_elements_worker.create_metadatas(element, metadata_list)
+        mock_elements_worker.create_metadata_bulk(element, metadata_list)
 
     assert len(responses.calls) == len(BASE_API_CALLS) + 5
     assert [
         (call.request.method, call.request.url) for call in responses.calls
     ] == BASE_API_CALLS + [
         # We retry 5 times the API call
         (
```

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_task.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_task.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_training.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_transcriptions.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_transcriptions.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_elements_worker/test_worker.py` & `arkindex-base-worker-0.3.7rc7/tests/test_elements_worker/test_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_image.py` & `arkindex-base-worker-0.3.7rc7/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_merge.py` & `arkindex-base-worker-0.3.7rc7/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc6/tests/test_utils.py` & `arkindex-base-worker-0.3.7rc7/tests/test_utils.py`

 * *Files identical despite different names*

