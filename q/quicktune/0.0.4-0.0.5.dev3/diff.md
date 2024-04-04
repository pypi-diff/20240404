# Comparing `tmp/quicktune-0.0.4.tar.gz` & `tmp/quicktune-0.0.5.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicktune-0.0.4.tar", last modified: Fri Mar 22 09:05:37 2024, max compression
+gzip compressed data, was "quicktune-0.0.5.dev3.tar", last modified: Thu Apr  4 12:19:27 2024, max compression
```

## Comparing `quicktune-0.0.4.tar` & `quicktune-0.0.5.dev3.tar`

### file list

```diff
@@ -1,49 +1,56 @@
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.049372 quicktune-0.0.4/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     1494 2024-03-20 20:59:48.000000 quicktune-0.0.4/LICENSE
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)       56 2024-03-22 09:05:23.000000 quicktune-0.0.4/MANIFEST.in
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4048 2024-03-22 09:05:37.049372 quicktune-0.0.4/PKG-INFO
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     1345 2024-03-22 01:52:19.000000 quicktune-0.0.4/README.md
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      878 2024-03-22 08:44:03.000000 quicktune-0.0.4/pyproject.toml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)       38 2024-03-22 09:05:37.049372 quicktune-0.0.4/setup.cfg
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.039372 quicktune-0.0.4/src/
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.039372 quicktune-0.0.4/src/quicktune/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      375 2024-03-21 12:22:12.000000 quicktune-0.0.4/src/quicktune/__init__.py
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.039372 quicktune-0.0.4/src/quicktune/finetune/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-21 11:10:16.000000 quicktune-0.0.4/src/quicktune/finetune/__init__.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    38329 2024-03-21 21:43:18.000000 quicktune-0.0.4/src/quicktune/finetune/finetune.py
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.039372 quicktune-0.0.4/src/quicktune/finetune/utils/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-21 11:11:37.000000 quicktune-0.0.4/src/quicktune/finetune/utils/__init__.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      746 2024-03-21 16:40:49.000000 quicktune-0.0.4/src/quicktune/finetune/utils/available_models.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    24012 2024-03-21 16:43:03.000000 quicktune-0.0.4/src/quicktune/finetune/utils/build_parser.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4231 2024-03-21 11:15:22.000000 quicktune-0.0.4/src/quicktune/finetune/utils/compute_embeddings.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4043 2024-03-21 22:51:40.000000 quicktune-0.0.4/src/quicktune/finetune/utils/eval_autofinetune.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    11635 2024-03-21 14:10:41.000000 quicktune-0.0.4/src/quicktune/finetune/utils/finetuning_stategies.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    10751 2024-03-21 11:11:37.000000 quicktune-0.0.4/src/quicktune/finetune/utils/stoch_norm.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    46656 2024-03-21 11:11:37.000000 quicktune-0.0.4/src/quicktune/finetune/utils/train.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    22021 2024-03-21 12:54:07.000000 quicktune-0.0.4/src/quicktune/finetune/utils/utils.py
--rwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)    17987 2024-03-21 11:11:37.000000 quicktune-0.0.4/src/quicktune/finetune/utils/validate.py
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.039372 quicktune-0.0.4/src/quicktune/optimizers/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      251 2024-03-21 12:21:53.000000 quicktune-0.0.4/src/quicktune/optimizers/__init__.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    10772 2024-03-21 22:12:42.000000 quicktune-0.0.4/src/quicktune/optimizers/bo.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    19422 2024-03-21 22:42:25.000000 quicktune-0.0.4/src/quicktune/optimizers/dyhpo.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      937 2024-03-21 22:23:21.000000 quicktune-0.0.4/src/quicktune/optimizers/gp.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    30326 2024-03-21 22:01:55.000000 quicktune-0.0.4/src/quicktune/optimizers/quicktune.py
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.049372 quicktune-0.0.4/src/quicktune/tools/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      157 2024-03-21 09:45:47.000000 quicktune-0.0.4/src/quicktune/tools/__init__.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    21531 2024-03-22 08:41:17.000000 quicktune-0.0.4/src/quicktune/tools/metadataset.py
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4178 2024-03-22 09:04:44.000000 quicktune-0.0.4/src/quicktune/tools/searchspace.py
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.049372 quicktune-0.0.4/src/quicktune/tools/searchspaces/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2350 2024-03-22 08:36:00.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v1.yml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2352 2024-03-22 08:37:44.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v2.yml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     3096 2024-03-22 08:37:46.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v3.yml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2382 2024-03-22 08:37:50.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v4.yml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      605 2024-03-22 08:37:52.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v5.yml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2328 2024-03-22 08:36:34.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v6.yml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2328 2024-03-22 08:37:56.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v7.yml
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2298 2024-03-22 08:38:00.000000 quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v8.yml
-drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-22 09:05:37.049372 quicktune-0.0.4/src/quicktune.egg-info/
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4048 2024-03-22 09:05:37.000000 quicktune-0.0.4/src/quicktune.egg-info/PKG-INFO
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     1470 2024-03-22 09:05:37.000000 quicktune-0.0.4/src/quicktune.egg-info/SOURCES.txt
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)        1 2024-03-22 09:05:37.000000 quicktune-0.0.4/src/quicktune.egg-info/dependency_links.txt
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      109 2024-03-22 09:05:37.000000 quicktune-0.0.4/src/quicktune.egg-info/requires.txt
--rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)       10 2024-03-22 09:05:37.000000 quicktune-0.0.4/src/quicktune.egg-info/top_level.txt
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     1494 2024-03-20 20:59:48.000000 quicktune-0.0.5.dev3/LICENSE
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)       56 2024-03-22 09:05:23.000000 quicktune-0.0.5.dev3/MANIFEST.in
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     3694 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/PKG-INFO
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      969 2024-04-04 10:27:22.000000 quicktune-0.0.5.dev3/README.md
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      890 2024-04-04 12:18:23.000000 quicktune-0.0.5.dev3/pyproject.toml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)       38 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/setup.cfg
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.923933 quicktune-0.0.5.dev3/src/
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.923933 quicktune-0.0.5.dev3/src/quicktune/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      375 2024-03-21 12:22:12.000000 quicktune-0.0.5.dev3/src/quicktune/__init__.py
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.923933 quicktune-0.0.5.dev3/src/quicktune/finetune/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-21 11:10:16.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/__init__.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    39607 2024-04-04 09:13:45.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/finetune.py
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)        0 2024-03-21 11:11:37.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/__init__.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      746 2024-03-21 16:40:49.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/available_models.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    24012 2024-03-21 16:43:03.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/build_parser.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4231 2024-03-21 11:15:22.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/compute_embeddings.py
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/custom/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      519 2024-04-04 09:12:05.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/custom/__init__.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    16056 2024-04-04 09:08:28.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/custom/loader.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    18599 2024-04-04 09:08:28.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/custom/transforms_factory.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4043 2024-03-21 22:51:40.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/eval_autofinetune.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    11635 2024-03-21 14:10:41.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/finetuning_stategies.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    10751 2024-03-21 11:11:37.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/stoch_norm.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    46656 2024-03-21 11:11:37.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/train.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    22021 2024-04-04 09:38:08.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/utils.py
+-rwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)    17987 2024-03-21 11:11:37.000000 quicktune-0.0.5.dev3/src/quicktune/finetune/utils/validate.py
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/src/quicktune/optimizers/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      251 2024-03-21 12:21:53.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/__init__.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    10772 2024-03-26 14:47:41.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/bo.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     9422 2024-03-26 21:33:41.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/cost_metalearner.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    18910 2024-04-04 10:50:58.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/dyhpo.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      936 2024-03-22 19:22:57.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/gp.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     7460 2024-03-26 21:40:02.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/performance_metalearner.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    30156 2024-04-04 10:08:14.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/quicktune.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     7835 2024-04-04 10:00:36.000000 quicktune-0.0.5.dev3/src/quicktune/optimizers/utils.py
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/src/quicktune/tools/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      157 2024-03-21 09:45:47.000000 quicktune-0.0.5.dev3/src/quicktune/tools/__init__.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)    21526 2024-03-28 09:24:40.000000 quicktune-0.0.5.dev3/src/quicktune/tools/metadataset.py
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     4178 2024-03-22 09:04:44.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspace.py
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2350 2024-03-22 08:36:00.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v1.yml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2352 2024-03-22 08:37:44.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v2.yml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     3096 2024-03-22 08:37:46.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v3.yml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2382 2024-03-22 08:37:50.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v4.yml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      605 2024-03-22 08:37:52.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v5.yml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2328 2024-03-22 08:36:34.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v6.yml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2328 2024-03-22 08:37:56.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v7.yml
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     2298 2024-03-22 08:38:00.000000 quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v8.yml
+drwxr-xr-x   0 evilknivl  (1000) evilknivl  (1000)        0 2024-04-04 12:19:27.933933 quicktune-0.0.5.dev3/src/quicktune.egg-info/
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     3694 2024-04-04 12:19:27.000000 quicktune-0.0.5.dev3/src/quicktune.egg-info/PKG-INFO
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)     1753 2024-04-04 12:19:27.000000 quicktune-0.0.5.dev3/src/quicktune.egg-info/SOURCES.txt
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)        1 2024-04-04 12:19:27.000000 quicktune-0.0.5.dev3/src/quicktune.egg-info/dependency_links.txt
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)      111 2024-04-04 12:19:27.000000 quicktune-0.0.5.dev3/src/quicktune.egg-info/requires.txt
+-rw-r--r--   0 evilknivl  (1000) evilknivl  (1000)       10 2024-04-04 12:19:27.000000 quicktune-0.0.5.dev3/src/quicktune.egg-info/top_level.txt
```

### Comparing `quicktune-0.0.4/LICENSE` & `quicktune-0.0.5.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/PKG-INFO` & `quicktune-0.0.5.dev3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicktune
-Version: 0.0.4
+Version: 0.0.5.dev3
 Summary: Quick-Tune: Quickly Learning Which Pretrained Model to Finetune and How
 Author-email: Ivo Rapant <rapanti@cs.uni-freiburg.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, rapanti
         
         Redistribution and use in source and binary forms, with or without
@@ -41,22 +41,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch<2,>=1.12.1
+Requires-Dist: torch>=1.12.1
 Requires-Dist: torchvision>=0.13.1
 Requires-Dist: torchaudio>=0.12.1
 Requires-Dist: ConfigSpace
 Requires-Dist: gpytorch
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
+Requires-Dist: timm
 Requires-Dist: tqdm
 
 # QuickTune (WIP)
 ## Quick-Tune: Quickly Learning Which Pre Trained Model to Fine Tune and How [ICLR2024](https://openreview.net/forum?id=tqh1zdXIra)
 
 This repo contains the code for running experiments with QuickTune
 
@@ -67,31 +68,21 @@
 
 ### Prepare Environment
 To install QuickTune, you can simply use `pip`:
 ```bash
 pip install quicktune
 ```
 
-This project depends on a custom version of [*timm*](https://github.com/huggingface/pytorch-image-models), which is not available on PyPI. You can install it by running the following command:
-```bash
-pip install git+https://github.com/rapanti/qt_timm
-```
-
 ### Download the QuickTune Meta-Dataset:
 ```bash
 wget https://rewind.tf.uni-freiburg.de/index.php/s/oMxC5sfrkA53ESo/download/qt_metadataset.zip
 unzip qt_metadataset.zip
 ```
 
-### Download the metalearned Optimizer
-```bash
-wget https://rewind.tf.uni-freiburg.de/index.php/s/XBsMjps5n3N9we6
-```
-
-### Prepare Custom Dataset
+### Run on Custom Dataset
 The custom dataset must be in Pytorch's [ImageFolder](https://pytorch.org/vision/main/generated/torchvision.datasets.ImageFolder.html) format, e.g. download the Imagenette dataset:
 ```bash
 wget https://s3.amazonaws.com/fast-ai-imageclas/imagenette2-320.tgz
 tar -xvzf imagenette2-320.tgz
 ```
 
 Modify the quicktuning [script](examples/quicktuning.py) in the examples folder to your needs.
```

### Comparing `quicktune-0.0.4/README.md` & `quicktune-0.0.5.dev3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,31 +10,21 @@
 
 ### Prepare Environment
 To install QuickTune, you can simply use `pip`:
 ```bash
 pip install quicktune
 ```
 
-This project depends on a custom version of [*timm*](https://github.com/huggingface/pytorch-image-models), which is not available on PyPI. You can install it by running the following command:
-```bash
-pip install git+https://github.com/rapanti/qt_timm
-```
-
 ### Download the QuickTune Meta-Dataset:
 ```bash
 wget https://rewind.tf.uni-freiburg.de/index.php/s/oMxC5sfrkA53ESo/download/qt_metadataset.zip
 unzip qt_metadataset.zip
 ```
 
-### Download the metalearned Optimizer
-```bash
-wget https://rewind.tf.uni-freiburg.de/index.php/s/XBsMjps5n3N9we6
-```
-
-### Prepare Custom Dataset
+### Run on Custom Dataset
 The custom dataset must be in Pytorch's [ImageFolder](https://pytorch.org/vision/main/generated/torchvision.datasets.ImageFolder.html) format, e.g. download the Imagenette dataset:
 ```bash
 wget https://s3.amazonaws.com/fast-ai-imageclas/imagenette2-320.tgz
 tar -xvzf imagenette2-320.tgz
 ```
 
 Modify the quicktuning [script](examples/quicktuning.py) in the examples folder to your needs.
```

### Comparing `quicktune-0.0.4/pyproject.toml` & `quicktune-0.0.5.dev3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "quicktune"
-version = "0.0.4"
+version = "0.0.5.dev3"
 dependencies = [
-  "torch>=1.12.1,<2",
+  "torch>=1.12.1",
   "torchvision>=0.13.1",
   "torchaudio>=0.12.1",
   "ConfigSpace",
   "gpytorch",
   "pandas",
   "pyyaml",
   "scikit-learn",
+  "timm",
   "tqdm",
 ]
 requires-python = ">=3.9"
 authors = [{ name = "Ivo Rapant", email = "rapanti@cs.uni-freiburg.de" }]
 readme = "README.md"
 description = "Quick-Tune: Quickly Learning Which Pretrained Model to Finetune and How"
 classifiers = [
```

### Comparing `quicktune-0.0.4/src/quicktune/finetune/finetune.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/finetune.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,38 +34,41 @@
 import yaml
 from timm import utils
 from timm.data import (
     AugMixDataset,
     FastCollateMixup,
     Mixup,
     create_dataset,
-    create_loader,
+    # create_loader,
     resolve_data_config,
 )
 from timm.loss import (
     BinaryCrossEntropy,
     JsdCrossEntropy,
     LabelSmoothingCrossEntropy,
     SoftTargetCrossEntropy,
 )
 from timm.models import (
-    convert_splitbn_model,
-    convert_sync_batchnorm,
+    # convert_splitbn_model,
+    # convert_sync_batchnorm,
     create_model,
     load_checkpoint,
     model_parameters,
     resume_checkpoint,
     safe_model_name,
-    set_fast_norm,
+    # set_fast_norm,
 )
+from timm.layers import convert_splitbn_model, convert_sync_batchnorm, set_fast_norm
 from timm.optim import create_optimizer_v2, optimizer_kwargs
 from timm.scheduler import create_scheduler_v2, scheduler_kwargs
 from timm.utils import ApexScaler, NativeScaler
 from torch.nn.parallel import DistributedDataParallel as NativeDDP
 
+from quicktune.finetune.utils.custom import create_loader
+
 from quicktune.finetune.utils.finetuning_stategies import (
     BatchSpectralShrinkage,
     BehavioralRegularization,
     CoTuningLoss,
     Relationship,
     SPRegularization,
     convert_to_stoch_norm,
@@ -151,15 +154,17 @@
     amp_dtype = torch.float16
     if args.amp:
         if args.amp_impl == "apex":
             assert has_apex, "AMP impl specified as APEX but APEX is not installed."
             use_amp = "apex"
             assert args.amp_dtype == "float16"
         else:
-            assert has_native_amp, "Please update PyTorch to a version with native AMP (or use APEX)."
+            assert (
+                has_native_amp
+            ), "Please update PyTorch to a version with native AMP (or use APEX)."
             use_amp = "native"
             assert args.amp_dtype in ("float16", "bfloat16")
         if args.amp_dtype == "bfloat16":
             amp_dtype = torch.bfloat16
 
     utils.random_seed(args.seed, args.rank)
 
@@ -182,17 +187,21 @@
     if args.in_chans is not None:
         in_chans = args.in_chans
     elif args.input_size is not None:
         in_chans = args.input_size[0]
 
     if args.dataset_augmentation_path:
         try:
-            dataset_aug_path = get_dataset_path(args.dataset_augmentation_path, args.dataset)
+            dataset_aug_path = get_dataset_path(
+                args.dataset_augmentation_path, args.dataset
+            )
             # dataset_path = get_dataset_path(args.data_dir, args.dataset)
-            icgen_dataset_info = get_icgen_dataset_info_json(dataset_aug_path, args.dataset)
+            icgen_dataset_info = get_icgen_dataset_info_json(
+                dataset_aug_path, args.dataset
+            )
 
             actual_num_classes = icgen_dataset_info["number_classes"]
             original_num_classes = get_number_of_classes(dataset_aug_path)
             args.num_classes = actual_num_classes
             extra_dataset_info = {"icgen_dataset_info": icgen_dataset_info}
 
             assert args.dataset.startswith(
@@ -200,20 +209,24 @@
             ), "dataset_augmentation_path is only supported for tfds_icgn datasets"
 
             print(f"Number of classes in original dataset: {original_num_classes}")
             print(f"Number of classes sampled from: {actual_num_classes}")
             print(
                 f"Number of train samples: {icgen_dataset_info['number_train_samples_per_class']*actual_num_classes}"
             )
-            print(f"Number of test samples: {icgen_dataset_info['number_test_samples_per_class']*actual_num_classes}")
+            print(
+                f"Number of test samples: {icgen_dataset_info['number_test_samples_per_class']*actual_num_classes}"
+            )
 
         except Exception as e:
             raise ValueError(f"Error reading dataset information: {e}")
     else:
-        assert args.num_classes is not None, "num_classes not inferred from data, please set it manually"
+        assert (
+            args.num_classes is not None
+        ), "num_classes not inferred from data, please set it manually"
         # we don't need sub-sampling the datasets (only used when ICGen augmentations are used and dataset_augmentation_path is set)
         extra_dataset_info = {}
 
     model = create_model(
         args.model,
         pretrained=args.pretrained,
         in_chans=in_chans,
@@ -232,15 +245,17 @@
         model.set_grad_checkpointing(enable=True)
 
     if utils.is_primary(args):
         _logger.info(
             f"Model {safe_model_name(args.model)} created, param count:{sum([m.numel() for m in model.parameters()])}"
         )
 
-    data_config = resolve_data_config(vars(args), model=model, verbose=utils.is_primary(args))
+    data_config = resolve_data_config(
+        vars(args), model=model, verbose=utils.is_primary(args)
+    )
 
     # correct data config mean
     if args.in_chans == 1:
         data_config["mean"] = data_config["mean"][:1]
         data_config["std"] = data_config["std"][:1]
 
     # setup augmentation batch splits for contrastive loss or split bn
@@ -285,15 +300,17 @@
         model = memory_efficient_fusion(model)
 
     if args.lr is None:
         global_batch_size = args.batch_size * args.world_size
         batch_ratio = global_batch_size / args.lr_base_size
         if not args.lr_base_scale:
             on = args.opt.lower()
-            args.lr_base_scale = "sqrt" if any([o in on for o in ("ada", "lamb")]) else "linear"
+            args.lr_base_scale = (
+                "sqrt" if any([o in on for o in ("ada", "lamb")]) else "linear"
+            )
         if args.lr_base_scale == "sqrt":
             batch_ratio = batch_ratio**0.5
         args.lr = args.lr_base * batch_ratio
         if utils.is_primary(args):
             _logger.info(
                 f"Learning rate ({args.lr}) calculated from base learning rate ({args.lr_base}) "
                 f"and global batch size ({global_batch_size}) with {args.lr_base_scale} scaling."
@@ -324,18 +341,22 @@
         return_source_output=return_source_output,
     )
 
     backbone_regularizations = []
     if args.sp_reg > 0.0:
         backbone_regularizations.append(SPRegularization(model, head_name, args.sp_reg))
     if args.bss_reg > 0.0:
-        backbone_regularizations.append(BatchSpectralShrinkage(regularization_weight=args.bss_reg))
+        backbone_regularizations.append(
+            BatchSpectralShrinkage(regularization_weight=args.bss_reg)
+        )
     if args.delta_reg > 0.0:
         source_model = copy.deepcopy(model)
-        backbone_regularizations.append(BehavioralRegularization(source_model, regularization_weight=args.delta_reg))
+        backbone_regularizations.append(
+            BehavioralRegularization(source_model, regularization_weight=args.delta_reg)
+        )
     if args.cotuning_reg > 0.0:
         compute_relationship = True
         source_model = copy.deepcopy(model)
         backbone_regularizations.append(CoTuningLoss(args.cotuning_reg))
     else:
         compute_relationship = False
 
@@ -372,30 +393,34 @@
         )
 
     # setup exponential moving average of model weights, SWA could be used here too
     model_ema = None
     if args.model_ema:
         # Important to create EMA model after cuda(), DP wrapper, and AMP but before DDP wrapper
         model_ema = utils.ModelEmaV2(
-            model, decay=args.model_ema_decay, device="cpu" if args.model_ema_force_cpu else None
+            model,
+            decay=args.model_ema_decay,
+            device="cpu" if args.model_ema_force_cpu else None,
         )
         if args.resume:
             load_checkpoint(model_ema.module, args.resume, use_ema=True)
 
     # setup distributed training
     if args.distributed:
         if has_apex and use_amp == "apex":
             # Apex DDP preferred unless native amp is activated
             if utils.is_primary(args):
                 _logger.info("Using NVIDIA APEX DistributedDataParallel.")
             model = ApexDDP(model, delay_allreduce=True)
         else:
             if utils.is_primary(args):
                 _logger.info("Using native Torch DistributedDataParallel.")
-            model = NativeDDP(model, device_ids=[device], broadcast_buffers=not args.no_ddp_bb)
+            model = NativeDDP(
+                model, device_ids=[device], broadcast_buffers=not args.no_ddp_bb
+            )
         # NOTE: EMA model does not need to be wrapped by DDP
 
     # create the train and eval datasets
     dataset_train = create_dataset(
         args.dataset,
         root=args.data_dir,
         split=args.train_split,
@@ -432,15 +457,17 @@
             prob=args.mixup_prob,
             switch_prob=args.mixup_switch_prob,
             mode=args.mixup_mode,
             label_smoothing=args.smoothing,
             num_classes=args.num_classes,
         )
         if args.prefetcher:
-            assert not num_aug_splits  # collate conflict (need to support deinterleaving in collate mixup)
+            assert (
+                not num_aug_splits
+            )  # collate conflict (need to support deinterleaving in collate mixup)
             collate_fn = FastCollateMixup(**mixup_args)
         else:
             mixup_fn = Mixup(**mixup_args)
 
     # wrap dataset in AugMix helper
     if num_aug_splits > 1:
         dataset_train = AugMixDataset(dataset_train, num_splits=num_aug_splits)
@@ -448,15 +475,15 @@
     # create data loaders w/ augmentation pipeline
     train_interpolation = args.train_interpolation
     if args.no_aug or not train_interpolation:
         train_interpolation = data_config["interpolation"]
     loader_train = create_loader(
         dataset_train,
         input_size=data_config["input_size"],
-        in_chans=in_chans,
+        # in_chans=in_chans,
         batch_size=args.batch_size,
         is_training=True,
         use_prefetcher=args.prefetcher,
         no_aug=args.no_aug,
         re_prob=args.reprob,
         re_mode=args.remode,
         re_count=args.recount,
@@ -476,28 +503,27 @@
         distributed=args.distributed,
         collate_fn=collate_fn,
         pin_memory=args.pin_mem,
         device=device,
         use_multi_epochs_loader=args.use_multi_epochs_loader,
         worker_seeding=args.worker_seeding,
         trivial_augment=args.trivial_augment,
-        random_augment=args.random_augment,
+        rand_augment=args.random_augment,
         ra_num_ops=args.ra_num_ops,
         ra_magnitude=args.ra_magnitude,
         persistent_workers=args.persistent_workers,
     )
 
     eval_workers = args.workers
     if args.distributed and ("tfds" in args.dataset or "wds" in args.dataset):
         # FIXME reduces validation padding issues when using TFDS, WDS w/ workers and distributed training
         eval_workers = min(2, args.workers)
     loader_eval = create_loader(
         dataset_eval,
         input_size=data_config["input_size"],
-        in_chans=in_chans,
         batch_size=args.validation_batch_size or args.batch_size,
         is_training=False,
         use_prefetcher=args.prefetcher,
         interpolation=data_config["interpolation"],
         mean=data_config["mean"],
         std=data_config["std"],
         num_workers=eval_workers,
@@ -517,32 +543,43 @@
             + "_"
             + args.dataset_augmentation_path.replace("/", "_")
             + "_"
             + args.dataset.replace("/", "_")
             + ".npy"
         )
         output_dir = utils.get_outdir(
-            os.path.join(args.output, "..", "relationships") if args.output else "./output/relationships"
+            os.path.join(args.output, "..", "relationships")
+            if args.output
+            else "./output/relationships"
+        )
+        relationship = Relationship(
+            loader_train,
+            source_model,
+            device,
+            cache=os.path.join(output_dir, file_name),
         )
-        relationship = Relationship(loader_train, source_model, device, cache=os.path.join(output_dir, file_name))
     else:
         relationship = None
     # setup loss function
     if args.jsd_loss:
         assert num_aug_splits > 1  # JSD only valid with aug splits set
-        train_loss_fn = JsdCrossEntropy(num_splits=num_aug_splits, smoothing=args.smoothing)
+        train_loss_fn = JsdCrossEntropy(
+            num_splits=num_aug_splits, smoothing=args.smoothing
+        )
     elif mixup_active:
         # smoothing is handled with mixup target transform which outputs sparse, soft targets
         if args.bce_loss:
             train_loss_fn = BinaryCrossEntropy(target_threshold=args.bce_target_thresh)
         else:
             train_loss_fn = SoftTargetCrossEntropy()
     elif args.smoothing:
         if args.bce_loss:
-            train_loss_fn = BinaryCrossEntropy(smoothing=args.smoothing, target_threshold=args.bce_target_thresh)
+            train_loss_fn = BinaryCrossEntropy(
+                smoothing=args.smoothing, target_threshold=args.bce_target_thresh
+            )
         else:
             train_loss_fn = LabelSmoothingCrossEntropy(smoothing=args.smoothing)
     else:
         train_loss_fn = nn.CrossEntropyLoss()
     train_loss_fn = train_loss_fn.to(device=device)
     validate_loss_fn = nn.CrossEntropyLoss().to(device=device)
 
@@ -559,15 +596,17 @@
             exp_name = "-".join(
                 [
                     datetime.now().strftime("%y%m%d-%H%M%S"),
                     safe_model_name(args.model),
                     str(data_config["input_size"][-1]),
                 ]
             )
-        output_dir = utils.get_outdir(args.output if args.output else "./output/train", exp_name)
+        output_dir = utils.get_outdir(
+            args.output if args.output else "./output/train", exp_name
+        )
 
         if has_synetune and args.report_synetune:
             # report = Reporter()
             output_dir = args.st_checkpoint_dir
             os.makedirs(output_dir, exist_ok=True)
 
         else:
@@ -696,15 +735,17 @@
             )
 
             if has_synetune and args.report_synetune:
                 report(epoch=epoch + 1, eval_accuracy=eval_metrics["top1"])
 
             if model_ema is not None and not args.model_ema_force_cpu:
                 if args.distributed and args.dist_bn in ("broadcast", "reduce"):
-                    utils.distribute_bn(model_ema, args.world_size, args.dist_bn == "reduce")
+                    utils.distribute_bn(
+                        model_ema, args.world_size, args.dist_bn == "reduce"
+                    )
 
                 ema_eval_metrics = validate(
                     model_ema.module,
                     loader_eval,
                     validate_loss_fn,
                     args,
                     amp_autocast=amp_autocast,
@@ -725,15 +766,17 @@
                     write_header=best_metric is None,
                     log_wandb=args.log_wandb and has_wandb,
                 )
 
             if not args.test_mode and saver is not None:
                 # save proper checkpoint with eval metric
                 save_metric = eval_metrics[eval_metric]
-                best_metric, best_epoch = saver.save_checkpoint(epoch, metric=save_metric)
+                best_metric, best_epoch = saver.save_checkpoint(
+                    epoch, metric=save_metric
+                )
 
             if lr_scheduler is not None:
                 # step LR for next epoch
                 lr_scheduler.step(epoch + 1, eval_metrics[eval_metric])
 
             if np.isnan(train_metrics["loss"]):
                 invalid_loss_value = True
@@ -804,15 +847,17 @@
     num_batches_per_epoch = len(loader)
     last_idx = num_batches_per_epoch - 1
     num_updates = epoch * num_batches_per_epoch
 
     for batch_idx, (input, target) in enumerate(loader):
         if args.test_mode:
             if batch_idx > 1:
-                print("--------- test_mode set to True: breaking epoch for test reasons ---------")
+                print(
+                    "--------- test_mode set to True: breaking epoch for test reasons ---------"
+                )
                 break
 
         last_batch = batch_idx == last_idx
         data_time_m.update(time.time() - end)
         if not args.prefetcher:
             input, target = input.to(device), target.to(device)
             if mixup_fn is not None:
@@ -839,27 +884,33 @@
                     output = backbone_regularization.source_model(input)
                     if len(output) == 2:
                         output_source, layer_outputs_source = output
                     elif len(output) == 3:
                         output_source, _, layer_outputs_source = output
                     loss += backbone_regularization(layer_outputs_source, features)
                 if isinstance(backbone_regularization, CoTuningLoss):
-                    source_label = torch.from_numpy(relationship[target.cpu().numpy()]).to(device).float()
+                    source_label = (
+                        torch.from_numpy(relationship[target.cpu().numpy()])
+                        .to(device)
+                        .float()
+                    )
                     loss += backbone_regularization(source_output, source_label)
 
         if not args.distributed:
             losses_m.update(loss.item(), input.size(0))
         optimizer.zero_grad()
         if loss_scaler is not None:
             loss_scaler(
                 loss,
                 optimizer,
                 clip_grad=args.clip_grad,
                 clip_mode=args.clip_mode,
-                parameters=model_parameters(model, exclude_head="agc" in args.clip_mode),
+                parameters=model_parameters(
+                    model, exclude_head="agc" in args.clip_mode
+                ),
                 create_graph=second_order,
             )
         else:
             loss.backward(create_graph=second_order)
             if args.clip_grad is not None:
                 utils.dispatch_clip_grad(
                     model_parameters(model, exclude_head="agc" in args.clip_mode),
@@ -875,19 +926,23 @@
             torch.cuda.synchronize()
         num_updates += 1
         batch_time_m.update(time.time() - end)
         if last_batch or batch_idx % args.log_interval == 0:
             num_logs += 1
             lrl = [param_group["lr"] for param_group in optimizer.param_groups]
             lr = sum(lrl) / len(lrl)
-            temp_backbone_grad_norm, temp_head_grad_norm = compute_gradient_norm(model, head_name)
+            temp_backbone_grad_norm, temp_head_grad_norm = compute_gradient_norm(
+                model, head_name
+            )
             backbone_grad_norm = (num_logs - 1) * backbone_grad_norm / num_logs + (
                 1 / num_logs
             ) * temp_backbone_grad_norm
-            head_grad_norm = (num_logs - 1) * head_grad_norm / num_logs + (1 / num_logs) * temp_head_grad_norm
+            head_grad_norm = (num_logs - 1) * head_grad_norm / num_logs + (
+                1 / num_logs
+            ) * temp_head_grad_norm
 
             if args.distributed:
                 reduced_loss = utils.reduce_tensor(loss.data, args.world_size)
                 losses_m.update(reduced_loss.item(), input.size(0))
 
             if utils.is_primary(args):
                 # fixing the batch_idx and last_idx
@@ -914,15 +969,18 @@
                         head_grad_norm=head_grad_norm,
                         backbone_grad_norm=backbone_grad_norm,
                     )
                 )
 
                 if args.save_images and output_dir:
                     torchvision.utils.save_image(
-                        input, os.path.join(output_dir, "train-batch-%d.jpg" % batch_idx), padding=0, normalize=True
+                        input,
+                        os.path.join(output_dir, "train-batch-%d.jpg" % batch_idx),
+                        padding=0,
+                        normalize=True,
                     )
 
         if (
             saver is not None
             and args.recovery_interval
             and (last_batch or (batch_idx + 1) % args.recovery_interval == 0)
         ):
@@ -937,15 +995,19 @@
             break
         # end for
 
     if hasattr(optimizer, "sync_lookahead"):
         optimizer.sync_lookahead()
 
     return OrderedDict(
-        [("loss", losses_m.avg), ("head_grad_norm", head_grad_norm), ("backbone_grad_norm", backbone_grad_norm)]
+        [
+            ("loss", losses_m.avg),
+            ("head_grad_norm", head_grad_norm),
+            ("backbone_grad_norm", backbone_grad_norm),
+        ]
     )
 
 
 @extend_metrics
 def validate(
     model,
     loader,
@@ -966,15 +1028,17 @@
 
     end = time.time()
     last_idx = len(loader) - 1
     with torch.no_grad():
         for batch_idx, (input, target) in enumerate(loader):
             if args.test_mode:
                 if batch_idx > 1:
-                    print("--------- test_mode set to True: breaking epoch for test reasons ---------")
+                    print(
+                        "--------- test_mode set to True: breaking epoch for test reasons ---------"
+                    )
                     break
 
             last_batch = batch_idx == last_idx
             if not args.prefetcher:
                 input = input.to(device)
                 target = target.to(device)
             if args.channels_last:
@@ -1014,21 +1078,31 @@
 
             losses_m.update(reduced_loss.item(), input.size(0))
             top1_m.update(acc1.item(), output.size(0))
             top5_m.update(acc5.item(), output.size(0))
 
             batch_time_m.update(time.time() - end)
             end = time.time()
-            if utils.is_primary(args) and (last_batch or batch_idx % args.log_interval == 0):
+            if utils.is_primary(args) and (
+                last_batch or batch_idx % args.log_interval == 0
+            ):
                 log_name = "Test" + log_suffix
                 _logger.info(
                     "{0}: [{1:>4d}/{2}]  "
                     "Time: {batch_time.val:.3f} ({batch_time.avg:.3f})  "
                     "Loss: {loss.val:>7.4f} ({loss.avg:>6.4f})  "
                     "Acc@1: {top1.val:>7.4f} ({top1.avg:>7.4f})  "
                     "Acc@5: {top5.val:>7.4f} ({top5.avg:>7.4f})".format(
-                        log_name, batch_idx, last_idx, batch_time=batch_time_m, loss=losses_m, top1=top1_m, top5=top5_m
+                        log_name,
+                        batch_idx,
+                        last_idx,
+                        batch_time=batch_time_m,
+                        loss=losses_m,
+                        top1=top1_m,
+                        top5=top5_m,
                     )
                 )
-    metrics = OrderedDict([("loss", losses_m.avg), ("top1", top1_m.avg), ("top5", top5_m.avg)])
+    metrics = OrderedDict(
+        [("loss", losses_m.avg), ("top1", top1_m.avg), ("top5", top5_m.avg)]
+    )
 
     return metrics
```

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/available_models.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/available_models.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/build_parser.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/build_parser.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/compute_embeddings.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/compute_embeddings.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/eval_autofinetune.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/eval_autofinetune.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/finetuning_stategies.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/finetuning_stategies.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/stoch_norm.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/stoch_norm.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/train.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/train.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/utils.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.model = model
         self.source_head = source_head
 
     def forward(self, *args, **kwargs):
         output, features = self.model(*args, **kwargs)
         x = self.model.last_layer_output
         source_output = None
-        if isinstance(self.model._model, models.xcit.XCiT):
+        if isinstance(self.model._model, models.xcit.Xcit):
             if self.model._model.global_pool:
                 x = x[:, 1:].mean(dim=1) if self.model._model.global_pool == "avg" else x[:, 0]
 
         elif (
             isinstance(self.model._model, models.swin_transformer_v2.SwinTransformerV2)
             or isinstance(self.model._model, models.swin_transformer_v2_cr.SwinTransformerV2Cr)
             or isinstance(self.model._model, models.swin_transformer.SwinTransformer)
@@ -179,15 +179,15 @@
         if change_head:
             num_ftrs = layers[-2].in_channels
             model.fc = nn.Conv2d(num_ftrs, num_classes, layers[-2].kernel_size, layers[-2].stride, device=device)
         head = model.fc
         last_hidden_layer_name = "global_pool"
         head_name = "fc"
 
-    elif isinstance(model, models.xcit.XCiT):
+    elif isinstance(model, models.xcit.Xcit):
         source_head = copy.deepcopy(model.head)
         if change_head:
             num_ftrs = model.head.in_features
             model.head = nn.Linear(num_ftrs, num_classes).to(device)
 
         last_hidden_layer_name = "norm"
         head_name = "head"
@@ -331,15 +331,15 @@
         if change_head:
             num_ftrs = layers[-2].in_channels
             model.fc = nn.Conv2d(num_ftrs, num_classes, layers[-2].kernel_size, layers[-2].stride, device=device)
         head = model.fc
         last_hidden_layer_name = "global_pool"
         head_name = "fc"
 
-    elif isinstance(model, models.xcit.XCiT):
+    elif isinstance(model, models.xcit.Xcit):
         source_head = copy.deepcopy(model.head)
         if change_head:
             num_ftrs = model.head.in_features
             model.head = nn.Linear(num_ftrs, num_classes).to(device)
 
         patch_embed, pos_embed, pos_drop, blocks, cls_attn_blocks, norm, head = list(model.children())
         hidden_layers = [patch_embed, pos_embed, pos_drop] + list(blocks) + list(cls_attn_blocks) + [norm]
```

### Comparing `quicktune-0.0.4/src/quicktune/finetune/utils/validate.py` & `quicktune-0.0.5.dev3/src/quicktune/finetune/utils/validate.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/optimizers/bo.py` & `quicktune-0.0.5.dev3/src/quicktune/optimizers/bo.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/optimizers/dyhpo.py` & `quicktune-0.0.5.dev3/src/quicktune/optimizers/dyhpo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 import logging
-import os
 from copy import deepcopy
-from typing import Dict, Tuple
+from typing import Dict, List, Optional, Tuple, Union
 
 import gpytorch
 import numpy as np
 import torch
 import torch.nn as nn
 
 from quicktune.optimizers.gp import GPRegressionModel
@@ -27,19 +26,18 @@
         nr_epochs: int = 1000,
         early_stopping_patience: int = 10,
         learning_rate: float = 0.001,
         include_metafeatures: bool = True,
         meta_checkpoint=None,
         output_path: str = ".",
         seed: int = 42,
+        configuration: Optional[dict] = None,
     ):
         """
-        The constructor for the DyHPO model.
         Args:
-
             device: The device where the experiments will be run on.
             dataset_name: The name of the dataset for the current run.
             output_path: The path where the intermediate/final results
                 will be stored.
             seed: The seed that will be used to store the checkpoint
                 properly.
         """
@@ -52,44 +50,36 @@
         self.refine_epochs = 50
         self.learning_rate = learning_rate
         self.dev = device
         self.seed = seed
         self.output_dim = output_dim
         self.model, self.likelihood, self.mll = self.get_model_likelihood_mll(self.output_dim)
 
+        self.configuration = configuration
+
         self.model.to(self.dev)
         self.likelihood.to(self.dev)
         self.feature_extractor.to(self.dev)
 
-        self.optimizer = torch.optim.Adam(
-            [
-                {"params": self.model.parameters(), "lr": self.learning_rate},
-                {"params": self.feature_extractor.parameters(), "lr": self.learning_rate},
-            ],
-        )
+        params = list(self.model.parameters()) + list(self.feature_extractor.parameters())
+        self.optimizer = torch.optim.Adam(params, lr=self.learning_rate)
 
         # the number of initial points for which we will retrain fully from scratch
         # This is basically equal to the dimensionality of the search space + 1.
         self.initial_nr_points = 10
         # keeping track of the total hpo iterations. It will be used during the optimization
         # process to switch from fully training the model, to refining.
         self.iterations = 0
         # flag for when the optimization of the model should start from scratch.
         self.restart = True
 
         self.logger = logging.getLogger(__name__)
 
-        self.checkpoint_path = os.path.join(
-            output_path,
-            "dyhpo-checkpoints",
-            f"{dataset_name}-seed{self.seed}",
-        )
-
         self.metafeatures: torch.Tensor
-        self.checkpoint_file = os.path.join(self.checkpoint_path, "checkpoint.pth")
+        self.checkpoint_file = "checkpoint.pth"
         self.cost_aware = False
         self.include_metafeatures = include_metafeatures
         self.meta_checkpoint = meta_checkpoint
 
     def set_cost_predictor(self, cost_predictor):
         self.cost_predictor = cost_predictor
         self.cost_aware = True
@@ -103,23 +93,16 @@
             self.model, self.likelihood, self.mll = self.get_model_likelihood_mll(
                 self.output_dim,
             )
 
         else:
             self.load_checkpoint(self.meta_checkpoint)
 
-        self.optimizer = torch.optim.Adam(
-            [
-                {"params": self.model.parameters(), "lr": self.learning_rate},
-                {
-                    "params": self.feature_extractor.parameters(),
-                    "lr": self.learning_rate,
-                },
-            ]
-        )
+        params = list(self.model.parameters()) + list(self.feature_extractor.parameters())
+        self.optimizer = torch.optim.Adam(params, lr=self.learning_rate)
 
     def get_model_likelihood_mll(
         self,
         train_size: int,
     ) -> Tuple[
         GPRegressionModel,
         gpytorch.likelihoods.GaussianLikelihood,
@@ -166,22 +149,22 @@
             projected_x = self.feature_extractor(X_train, train_budgets, train_curves)
         self.model.set_train_data(projected_x, y_train, strict=False)
         output = self.model(projected_x)
         training_errored = False
 
         try:
             # Calc loss and backprop derivatives
-            loss = -self.mll(output, self.model.train_targets)
+            loss = -self.mll(output, self.model.train_targets)  # type: ignore
             loss_value = loss.detach().to("cpu").item()
             mse = gpytorch.metrics.mean_squared_error(output, self.model.train_targets)
             self.logger.debug(
                 f"Epoch {epoch_nr} - MSE {mse:.5f}, "
                 f"Loss: {loss_value:.3f}, "
                 f"lengthscale: {self.model.covar_module.base_kernel.lengthscale.item():.3f}, "
-                f"noise: {self.model.likelihood.noise.item():.3f}, "
+                f"noise: {self.model.likelihood.noise.item():.3f}"  # type: ignore
             )
             loss.backward()
             self.optimizer.step()
         except Exception as training_error:
             self.logger.error(f"The following error happened while training: {training_error}")
             # An error has happened, trigger the restart of the optimization and restart
             # the model with default hyperparameters.
@@ -197,17 +180,14 @@
             data: A dictionary which has the training examples, training features,
                 training budgets and in the end the training curves.
             load_checkpoint: A flag whether to load the state from a previous checkpoint,
                 or whether to start from scratch.
         """
         self.iterations += 1
         self.logger.debug(f"Starting iteration: {self.iterations}")
-        # whether the state has been changed. Basically, if a better loss was found during
-        # this optimization iteration then the state (weights) were changed.
-        weights_changed = False
 
         if load_checkpoint:
             try:
                 self.load_checkpoint()
             except FileNotFoundError:
                 self.logger.error(
                     f"No checkpoint file found at: {self.checkpoint_file} - Training the GP from the beginning"
@@ -239,18 +219,14 @@
             # - We are switching from the full training phase in the beginning to refining.
             # - We are restarting because our refining diverged
             if self.initial_nr_points <= self.iterations:
                 self.restart = False
         else:
             nr_epochs = self.refine_epochs
 
-        # where the mean squared error will be stored
-        # when predicting on the train set
-        mse = 0.0
-
         for epoch_nr in range(0, nr_epochs):
             if self.include_metafeatures:
                 batch_metafeatures = self.metafeatures.repeat(X_train.size(dim=0), 1)
             else:
                 batch_metafeatures = None
             training_errored = self.train_step(
                 X_train,
@@ -272,15 +248,15 @@
             self.load_checkpoint()
 
     def predict_pipeline(
         self,
         train_data: Dict[str, torch.Tensor],
         test_data: Dict[str, torch.Tensor],
         to_numpy: bool = True,
-    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    ) -> Tuple[np.ndarray, np.ndarray, Union[np.ndarray, None]]:
         """
         Args:
             train_data: A dictionary that has the training
                 examples, features, budgets and learning curves.
             test_data: Same as for the training data, but it is
                 for the testing part and it does not feature labels.
         Returns:
@@ -346,38 +322,39 @@
         else:
             means = preds.mean.reshape(
                 -1,
             )
             stds = preds.stddev.reshape(
                 -1,
             )
-        return means, stds, costs
+        return means, stds, costs  # type: ignore
 
     def load_checkpoint(self, checkpoint_file=None):
         """
         Load the state from a previous checkpoint.
         """
         if checkpoint_file is None:
             checkpoint_file = self.checkpoint_file
         checkpoint = torch.load(checkpoint_file)
         self.model.load_state_dict(checkpoint["gp_state_dict"])
-        self.feature_extractor.load_state_dict(checkpoint["feature_extractor_state_dict"])
+        msg = self.feature_extractor.load_state_dict(checkpoint["feature_extractor_state_dict"])
+        print(msg)
         self.original_feature_extractor.load_state_dict(checkpoint["feature_extractor_state_dict"])
         self.likelihood.load_state_dict(checkpoint["likelihood_state_dict"])
 
     def save_checkpoint(self, state: Dict = {}, checkpoint_file: str = ""):
         """
         Save the given state or the current state in a checkpoint file.
         Args:
             state: The state to save, if none, it will
             save the current state.
         """
-        if checkpoint_file == "":
-            os.makedirs(self.checkpoint_path, exist_ok=True)
-            checkpoint_file = self.checkpoint_file
+        # if checkpoint_file == "":
+        #     os.makedirs(self.checkpoint_path, exist_ok=True)
+        #     checkpoint_file = self.checkpoint_file
 
         if state == {}:
             torch.save(self.get_state(), checkpoint_file)
         else:
             torch.save(state, checkpoint_file)
 
     def get_state(self) -> Dict[str, Dict]:
@@ -453,23 +430,23 @@
         return x
 
 
 class FeatureExtractor(nn.Module):
     def __init__(
         self,
         configuration: dict = {},
-        input_dim_hps=None,
-        output_dim=32,
-        input_dim_curves=1,
-        output_dim_curves=16,
-        hidden_dim=128,
-        input_dim_metafeatures=7684,
-        output_dim_metafeatures=0,
-        encoder_dim_ranges=None,
-        encoder_num_layers=1,
+        input_dim_hps: int = 0,
+        output_dim: int = 32,
+        input_dim_curves: int = 1,
+        output_dim_curves: int = 16,
+        hidden_dim: int = 128,
+        input_dim_metafeatures: int = 7684,
+        output_dim_metafeatures: int = 0,
+        encoder_dim_ranges: Optional[List[Tuple[int, int]]] = None,
+        encoder_num_layers: int = 1,
     ):
         super().__init__()
 
         self.input_dim = (
             configuration.get("input_dim_hps", input_dim_hps)
             + configuration.get("output_dim_curves", output_dim_curves)
             + configuration.get("output_dim_metafeatures", output_dim_metafeatures)
```

### Comparing `quicktune-0.0.4/src/quicktune/optimizers/gp.py` & `quicktune-0.0.5.dev3/src/quicktune/optimizers/gp.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,21 @@
     def __init__(
         self,
         train_x: torch.Tensor,
         train_y: torch.Tensor,
         likelihood: gpytorch.likelihoods.GaussianLikelihood,
     ):
         """
-        Constructor of the GPRegressionModel.
         Args:
             train_x: The initial train examples for the GP.
             train_y: The initial train labels for the GP.
             likelihood: The likelihood to be used.
         """
         super(GPRegressionModel, self).__init__(train_x, train_y, likelihood)
 
         self.mean_module = gpytorch.means.ConstantMean()
         self.covar_module = gpytorch.kernels.ScaleKernel(gpytorch.kernels.RBFKernel())
 
-    def forward(self, x):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
         mean_x = self.mean_module(x)
         covar_x = self.covar_module(x)
-
-        return gpytorch.distributions.MultivariateNormal(mean_x, covar_x)
+        return gpytorch.distributions.MultivariateNormal(mean_x, covar_x)  # type: ignore
```

### Comparing `quicktune-0.0.4/src/quicktune/optimizers/quicktune.py` & `quicktune-0.0.5.dev3/src/quicktune/optimizers/quicktune.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,40 +15,38 @@
 from quicktune.optimizers.dyhpo import DyHPO
 
 
 class QuickTuneOptimizer:
     def __init__(
         self,
         model: DyHPO,
-        hp_candidates: np.ndarray,
+        hp_candidates: List,
         log_indicator: List[bool],
         hp_names: List[str],
-        init_conf_indices: list = [],
+        init_conf_indices: Optional[List] = None,
         seed: int = 11,
         max_benchmark_epochs: int = 50,
         fantasize_step: int = 1,
         minimization: bool = True,
         total_budget: int = 10000,  # budget in epochs (not time)
-        device: str = '',
-        dataset_name: str = "dataset",
+        device: str = "",
+        dataset_name: str = "",
         output_path: str = ".",
         acqf_fc: str = "ucb",
         explore_factor=1.0,
         learning_rate: float = 0.001,
         apply_preprocessing: bool = False,
         verbose: bool = True,
     ):
         """
         Args:
             hp_candidates: np.ndarray
-                The full list of hyperparameter candidates for
-                a given dataset.
+                The full list of hyperparameter candidates for a given dataset.
             log_indicator: List
-                A list with boolean values indicating if a
-                hyperparameter has been log sampled or not.
+                A list with boolean values indicating if a hyperparameter has been log sampled or not.
             seed: int
                 The seed that will be used for the surrogate.
             max_benchmark_epochs: int
                 The maximal budget that a hyperparameter configuration
                 has been evaluated in the benchmark for.
             fantasize_step: int
                 The number of steps for which we are looking ahead to
@@ -72,25 +70,23 @@
         cudnn.benchmark = False
         torch.manual_seed(seed)
         np.random.seed(seed)
 
         if device:
             self.device = torch.device(device)
         else:
-            self.device = torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")            
+            self.device = torch.device("cuda") if torch.cuda.is_available() else torch.device("cpu")
 
         self.hp_candidates = hp_candidates
         self.log_indicator = log_indicator
         self.hp_names = hp_names
 
         if apply_preprocessing:
-            self.scaler = MinMaxScaler()
             self.hp_candidates = self.preprocess_hp_candidates()
         else:
-            self.scaler = None
             self.hp_candidates = np.array(self.hp_candidates)
 
         self.minimization = minimization
         self.seed = seed
         self.learning_rate = learning_rate
 
         if verbose:
@@ -115,15 +111,15 @@
         self.max_benchmark_epochs = max_benchmark_epochs
         self.total_budget = total_budget
         self.fantasize_step = fantasize_step
         self.nr_features = self.hp_candidates.shape[1]
         self.rng = np.random.default_rng(seed)
 
         conf_individual_budget = 1
-        if not init_conf_indices:
+        if init_conf_indices is None:
             initial_configurations_nr = 1
             self.init_conf_indices = self.rng.choice(
                 self.hp_candidates.shape[0], initial_configurations_nr, replace=False
             )
         else:
             initial_configurations_nr = len(init_conf_indices)
             self.init_conf_indices = np.array(init_conf_indices)
@@ -155,15 +151,15 @@
         self.dataset_name = dataset_name
 
         self.no_improvement_threshold = int(self.max_benchmark_epochs + 0.2 * self.max_benchmark_epochs)
         self.no_improvement_patience = 0
         self.converged_configs = []
         self.acq_fc = acqf_fc
         self.explore_factor = explore_factor
-        self.cost_trainer = None
+        self.cost_trainer: Optional[torch.nn.Module] = None
 
     def _prepare_dataset_and_budgets(self) -> Dict[str, torch.Tensor]:
         """
         Prepare the data that will be the input to the surrogate.
         Returns:
             data: A Dictionary that contains inside the training examples,
             the budgets, the curves and lastly the labels.
@@ -207,15 +203,15 @@
         self.logger.info("Started training the model")
 
         self.model.train_pipeline(
             data,
             load_checkpoint=False,
         )
 
-    def _predict(self) -> Tuple[np.ndarray, np.ndarray, np.ndarray, List, List]:
+    def _predict(self) -> Tuple[np.ndarray, np.ndarray, Optional[np.ndarray], List, np.ndarray]:
         """
         Predict the performances of the hyperparameter configurations
         as well as the standard deviations based on the surrogate model.
         Returns:
             mean_predictions, std_predictions, hp_indices, non_scaled_budgets:
                 The mean predictions and the standard deviations over
                 all model predictions for the given hyperparameter
@@ -270,14 +266,15 @@
             self.init_conf_indices = np.array(init_conf_indices)
 
         self.init_budgets = [conf_individual_budget] * initial_configurations_nr
 
     def suggest(self) -> Tuple[int, int]:
         """
         Suggest a hyperparameter configuration to be evaluated next.
+
         Returns:
             best_config_index, budget: The index of the hyperparamter
                 configuration to be evaluated and the budget for
                 what it is going to be evaluated for.
         """
         suggest_time_start = time.time()
         # check if we still have random hyperparameters to evaluate
@@ -285,14 +282,15 @@
             self.logger.info("Not enough configurations to build a model. Returning randomly sampled configuration")
 
             random_indice = self.init_conf_indices[self.initial_random_index]
             budget = self.init_budgets[self.initial_random_index]
             self.initial_random_index += 1
 
             return random_indice, budget
+
         else:
             mean_predictions, std_predictions, costs, hp_indices, non_scaled_budgets = self._predict()
 
             best_prediction_index = self.find_suggested_config(
                 mean_predictions, std_predictions, non_scaled_budgets, costs
             )
             """
@@ -398,20 +396,17 @@
         """
         examples = []
         for hp_index in hp_indices:
             examples.append(self.hp_candidates[hp_index])
 
         return examples
 
-    def generate_candidate_configurations(
-        self,
-    ) -> Tuple[List, List, List, List]:
+    def generate_candidate_configurations(self) -> Tuple[List, List, List, List]:
         """
-        Generate candidate configurations that will be
-        fantasized upon.
+        Generate candidate configurations that will be fantasized upon.
         Returns:
             (configurations, hp_indices, hp_budgets, learning_curves): Tuple
                 A tuple of configurations, their indices in the hp list
                 and the budgets that they should be fantasized upon.
         """
         hp_indices = []
         hp_budgets = []
@@ -425,22 +420,20 @@
                 budgets = self.examples[hp_index]
                 # Take the max budget evaluated for a certain hpc
                 max_budget = max(budgets)
                 next_budget = max_budget + self.fantasize_step
                 # take the learning curve until the point we have evaluated so far
                 # curve = self.performances[hp_index][:max_budget - 1] if max_budget > 1 else [0.0]
                 curve = self.performances[hp_index][:max_budget]
-                # if the curve is shorter than the length of the kernel size,
-                # pad it with zeros
+                # if the curve is shorter than the length of the kernel size, pad it with zeros
                 difference_curve_length = self.max_benchmark_epochs - len(curve)
                 if difference_curve_length > 0:
                     curve.extend([0.0] * difference_curve_length)
             else:
-                # The hpc was not evaluated before, so fantasize its
-                # performance
+                # The hpc was not evaluated before, so fantasize its performance
                 next_budget = self.fantasize_step
                 curve = [0, 0, 0]
 
             # this hyperparameter configuration is not evaluated fully
             if next_budget <= self.max_benchmark_epochs:
                 hp_indices.append(hp_index)
                 hp_budgets.append(next_budget)
@@ -486,17 +479,17 @@
         return train_examples, train_labels, train_budgets, train_curves
 
     def acq(
         self,
         best_value: float,
         mean: float,
         std: float,
-        explore_factor: Optional[float] = 0.25,
+        explore_factor: float = 0.25,
         acq_fc: str = "ei",
-        cost: Optional[float] = 1,
+        cost: float = 1,
     ) -> float:
         """
         The acquisition function that will be called
         to evaluate the score of a hyperparameter configuration.
         Parameters
         ----------
         best_value: float
@@ -504,16 +497,14 @@
         mean: float
             Point mean of the posterior process.
         std: float
             Point std of the posterior process.
         explore_factor: float
             The exploration factor for when ucb is used as the
             acquisition function.
-        ei_calibration_factor: float
-            The factor used to calibrate expected improvement.
         acq_fc: str
             The type of acquisition function to use.
         Returns
         -------
         acq_value: float
             The value of the acquisition function.
         """
@@ -539,15 +530,15 @@
             return acq_value / (1e-4)
 
     def find_suggested_config(
         self,
         mean_predictions: np.ndarray,
         mean_stds: np.ndarray,
         budgets: List,
-        costs: Optional[np.array] = None,
+        costs: Optional[np.ndarray] = None,
         return_highest_acq_value: bool = False,
     ):
         """
         Find the hyperparameter configuration that has the highest score
         with the acquisition function.
         Args:
             mean_predictions: The mean predictions of the posterior.
@@ -659,18 +650,19 @@
             self.info_dict["epochs"] = [budget]
 
         if "overhead" in self.info_dict:
             self.info_dict["overhead"].append(overhead)
         else:
             self.info_dict["overhead"] = [overhead]
 
-        with open(os.path.join(self.output_path, f"{self.dataset_name}_{self.seed}.json"), "w") as fp:
+        output_path = os.path.join(self.output_path, f"{self.dataset_name}_{self.seed}.json")
+        with open(output_path, "w") as fp:
             json.dump(self.info_dict, fp)
 
-    def preprocess_hp_candidates(self) -> List:
+    def preprocess_hp_candidates(self) -> np.ndarray:
         """
         Preprocess the list of all hyperparameter candidates
         by  performing a log transform for the hyperparameters that
         were log sampled.
         Returns:
             log_hp_candidates: The list of all hyperparameter configurations
                 where hyperparameters that were log sampled are log transformed.
@@ -681,17 +673,18 @@
             new_hp_candidate = []
             for index, hp_value in enumerate(hp_candidate):
                 new_hp_candidate.append(math.log(hp_value) if self.log_indicator[index] else hp_value)
 
             log_hp_candidates.append(new_hp_candidate)
 
         log_hp_candidates = np.array(log_hp_candidates)
+        
         # scaler for the hp configurations
-
-        log_hp_candidates = self.scaler.fit_transform(log_hp_candidates)
+        scaler = MinMaxScaler()
+        log_hp_candidates = scaler.fit_transform(log_hp_candidates)
 
         return log_hp_candidates
 
     @staticmethod
     def patch_curves_to_same_length(curves, max_curve_length=50):
         """
         Patch the given curves to the same length.
```

### Comparing `quicktune-0.0.4/src/quicktune/tools/metadataset.py` & `quicktune-0.0.5.dev3/src/quicktune/tools/metadataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import List
+from typing import List, Optional
 
 import numpy as np
 import pandas as pd
 import yaml
 from sklearn.compose import ColumnTransformer
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
@@ -81,15 +81,15 @@
     - verbose: bool, whether to print information (default: False)
     """
 
     def __init__(
         self,
         path: str,
         version: str,
-        curves_to_load: List[str] | None = None,
+        curves_to_load: Optional[List[str]] = None,
         preprocess_args: bool = True,
         aggregate_data: bool = False,
         drop_constant_args: bool = True,
         impute_numerical_args: bool = True,
         encode_categorical_args: bool = True,
         standardize_numerical_args: bool = True,
         load_only_dataset_descriptors: bool = False,
@@ -318,15 +318,15 @@
         if self.encode_categorical_args:
             cat_columns.remove("experiment")
 
             cat_transformer = Pipeline(steps=[("onehot", OneHotEncoder(handle_unknown="ignore"))])
             col_transformer = ColumnTransformer(transformers=[("cat", cat_transformer, cat_columns)])
 
             # Fit and transform the data
-            df_cat_transformed = col_transformer.fit_transform(args_df).toarray()
+            df_cat_transformed = col_transformer.fit_transform(args_df).toarray()  # type: ignore
             new_cat_columns = col_transformer.get_feature_names_out().tolist()
             df_cat_transformed = pd.DataFrame(df_cat_transformed, columns=new_cat_columns)
         else:
             df_cat_transformed = args_df.select_dtypes(include=["object"])
 
         # non_cat_columns = args_df.select_dtypes(include=['float64', 'int64', 'bool']).columns.tolist()
         non_cat_columns = NON_CAT_COLS
@@ -501,45 +501,44 @@
         else:
             return self.curves[curve_name][self.dataset_name][run_id]
 
     def get_curve_len(self, *args, **kwargs):
         assert self.dataset_name is not None, "Dataset name not set. Use set_dataset_name() to set it."
         return len(self.get_curve(*args, **kwargs))
 
-    # def get_hyperparameters(self, hp_index=None):
     def get_hyperparameters(self, hp_index):
         return self.hyperparameters_candidates.iloc[hp_index]
 
     def get_num_hyperparameters(self):
         return len(self.hyperparameters_candidates)
 
     def get_hyperparameters_names(self):
         return self.hyperparameter_names
 
-    def set_preset_metafeatures(self, preset_metafeatures):
-        self.preset_metafeatures = preset_metafeatures
+    # def set_preset_metafeatures(self, preset_metafeatures):
+    #     self.preset_metafeatures = preset_metafeatures
 
     def get_metafeatures(self):
         if self.augmentation_id is not None:
             adapted_dataset_name = "/".join(self.dataset_name.split("/")[1:])
             adapted_dataset_name = f"{adapted_dataset_name}-{self.augmentation_id}"
         else:
             adapted_dataset_name = self.dataset_name
 
         if self.preset_metafeatures is None:
             return self.metafeatures.loc[adapted_dataset_name].values
         else:
             return self.preset_metafeatures
 
-    def set_action_on_model(self, target_model, action_on_model):
-        # set action
-        self.action_on_model = action_on_model
-        self.target_model = target_model
-
-    def reset_action_on_model(self):
-        self.action_on_model = None
-        self.target_model = None
+    # def set_action_on_model(self, target_model, action_on_model):
+    #     # set action
+    #     self.action_on_model = action_on_model
+    #     self.target_model = target_model
+
+    # def reset_action_on_model(self):
+    #     self.action_on_model = None
+    #     self.target_model = None
 
     def set_subsample_models(self, subsample_models_in_hub):
         self.subsample_models_in_hub = subsample_models_in_hub
         self.model_vars = self.dataset_args_df.columns[self.dataset_args_df.columns.str.startswith("cat__model_")]
         self.selected_models = np.random.choice(self.model_vars, self.subsample_models_in_hub, replace=False)
```

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspace.py` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspace.py`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v1.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v1.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v2.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v2.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v3.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v3.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v4.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v4.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v5.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v5.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v6.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v6.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v7.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v7.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune/tools/searchspaces/search_space_v8.yml` & `quicktune-0.0.5.dev3/src/quicktune/tools/searchspaces/search_space_v8.yml`

 * *Files identical despite different names*

### Comparing `quicktune-0.0.4/src/quicktune.egg-info/PKG-INFO` & `quicktune-0.0.5.dev3/src/quicktune.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicktune
-Version: 0.0.4
+Version: 0.0.5.dev3
 Summary: Quick-Tune: Quickly Learning Which Pretrained Model to Finetune and How
 Author-email: Ivo Rapant <rapanti@cs.uni-freiburg.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, rapanti
         
         Redistribution and use in source and binary forms, with or without
@@ -41,22 +41,23 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch<2,>=1.12.1
+Requires-Dist: torch>=1.12.1
 Requires-Dist: torchvision>=0.13.1
 Requires-Dist: torchaudio>=0.12.1
 Requires-Dist: ConfigSpace
 Requires-Dist: gpytorch
 Requires-Dist: pandas
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
+Requires-Dist: timm
 Requires-Dist: tqdm
 
 # QuickTune (WIP)
 ## Quick-Tune: Quickly Learning Which Pre Trained Model to Fine Tune and How [ICLR2024](https://openreview.net/forum?id=tqh1zdXIra)
 
 This repo contains the code for running experiments with QuickTune
 
@@ -67,31 +68,21 @@
 
 ### Prepare Environment
 To install QuickTune, you can simply use `pip`:
 ```bash
 pip install quicktune
 ```
 
-This project depends on a custom version of [*timm*](https://github.com/huggingface/pytorch-image-models), which is not available on PyPI. You can install it by running the following command:
-```bash
-pip install git+https://github.com/rapanti/qt_timm
-```
-
 ### Download the QuickTune Meta-Dataset:
 ```bash
 wget https://rewind.tf.uni-freiburg.de/index.php/s/oMxC5sfrkA53ESo/download/qt_metadataset.zip
 unzip qt_metadataset.zip
 ```
 
-### Download the metalearned Optimizer
-```bash
-wget https://rewind.tf.uni-freiburg.de/index.php/s/XBsMjps5n3N9we6
-```
-
-### Prepare Custom Dataset
+### Run on Custom Dataset
 The custom dataset must be in Pytorch's [ImageFolder](https://pytorch.org/vision/main/generated/torchvision.datasets.ImageFolder.html) format, e.g. download the Imagenette dataset:
 ```bash
 wget https://s3.amazonaws.com/fast-ai-imageclas/imagenette2-320.tgz
 tar -xvzf imagenette2-320.tgz
 ```
 
 Modify the quicktuning [script](examples/quicktuning.py) in the examples folder to your needs.
```

### Comparing `quicktune-0.0.4/src/quicktune.egg-info/SOURCES.txt` & `quicktune-0.0.5.dev3/src/quicktune.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,25 @@
 src/quicktune/finetune/utils/compute_embeddings.py
 src/quicktune/finetune/utils/eval_autofinetune.py
 src/quicktune/finetune/utils/finetuning_stategies.py
 src/quicktune/finetune/utils/stoch_norm.py
 src/quicktune/finetune/utils/train.py
 src/quicktune/finetune/utils/utils.py
 src/quicktune/finetune/utils/validate.py
+src/quicktune/finetune/utils/custom/__init__.py
+src/quicktune/finetune/utils/custom/loader.py
+src/quicktune/finetune/utils/custom/transforms_factory.py
 src/quicktune/optimizers/__init__.py
 src/quicktune/optimizers/bo.py
+src/quicktune/optimizers/cost_metalearner.py
 src/quicktune/optimizers/dyhpo.py
 src/quicktune/optimizers/gp.py
+src/quicktune/optimizers/performance_metalearner.py
 src/quicktune/optimizers/quicktune.py
+src/quicktune/optimizers/utils.py
 src/quicktune/tools/__init__.py
 src/quicktune/tools/metadataset.py
 src/quicktune/tools/searchspace.py
 src/quicktune/tools/searchspaces/search_space_v1.yml
 src/quicktune/tools/searchspaces/search_space_v2.yml
 src/quicktune/tools/searchspaces/search_space_v3.yml
 src/quicktune/tools/searchspaces/search_space_v4.yml
```

