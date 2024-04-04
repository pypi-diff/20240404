# Comparing `tmp/deephyper-0.6.0.tar.gz` & `tmp/deephyper-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephyper-0.6.0.tar", last modified: Mon Aug 21 15:21:32 2023, max compression
+gzip compressed data, was "deephyper-0.7.0.tar", last modified: Thu Apr  4 07:29:02 2024, max compression
```

## Comparing `deephyper-0.6.0.tar` & `deephyper-0.7.0.tar`

### file list

```diff
@@ -1,265 +1,269 @@
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.539949 deephyper-0.6.0/
--rw-r--r--   0 romainegele   (501) staff       (20)     1531 2023-04-18 19:40:47.000000 deephyper-0.6.0/LICENSE.md
--rw-r--r--   0 romainegele   (501) staff       (20)       99 2021-11-16 07:10:00.000000 deephyper-0.6.0/MANIFEST.in
--rw-r--r--   0 romainegele   (501) staff       (20)    10794 2023-08-21 15:21:32.540062 deephyper-0.6.0/PKG-INFO
--rw-r--r--   0 romainegele   (501) staff       (20)     9228 2023-08-21 14:53:56.000000 deephyper-0.6.0/README.md
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.514040 deephyper-0.6.0/deephyper/
--rw-r--r--   0 romainegele   (501) staff       (20)     1297 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      109 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/__version__.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.515151 deephyper-0.6.0/deephyper/analysis/
--rw-r--r--   0 romainegele   (501) staff       (20)      130 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/analysis/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      627 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/analysis/_rank.py
--rw-r--r--   0 romainegele   (501) staff       (20)      953 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/analysis/hpo.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.515383 deephyper-0.6.0/deephyper/core/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/__init__.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.516180 deephyper-0.6.0/deephyper/core/analytics/
--rw-r--r--   0 romainegele   (501) staff       (20)      301 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/core/analytics/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1364 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/analytics/_analytics.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1222 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/analytics/_dashboard.py
--rw-r--r--   0 romainegele   (501) staff       (20)     9098 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/analytics/_db_manager.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5701 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/analytics/_quick_plot.py
--rw-r--r--   0 romainegele   (501) staff       (20)     4269 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/analytics/_topk.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.516521 deephyper-0.6.0/deephyper/core/analytics/dashboard/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/analytics/dashboard/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3507 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/analytics/dashboard/_pyplot.py
--rw-r--r--   0 romainegele   (501) staff       (20)    20546 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/analytics/dashboard/_views.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.517470 deephyper-0.6.0/deephyper/core/cli/
--rw-r--r--   0 romainegele   (501) staff       (20)      205 2023-07-05 07:15:50.000000 deephyper-0.6.0/deephyper/core/cli/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1600 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/_cli.py
--rw-r--r--   0 romainegele   (501) staff       (20)      827 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/cli/_cobalt_nodelist.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6917 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/cli/_hps.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6849 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/cli/_nas.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2325 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/cli/_new_problem.py
--rw-r--r--   0 romainegele   (501) staff       (20)      938 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/cli/_nodelist.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1811 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/cli/_start_project.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.509906 deephyper-0.6.0/deephyper/core/cli/templates/
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.518207 deephyper-0.6.0/deephyper/core/cli/templates/hps/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/hps/__init__.py.tmpl
--rw-r--r--   0 romainegele   (501) staff       (20)     1631 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/hps/load_data.py.tmpl
--rw-r--r--   0 romainegele   (501) staff       (20)     1254 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/hps/model_run.py.tmpl
--rw-r--r--   0 romainegele   (501) staff       (20)      357 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/hps/problem.py.tmpl
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.518837 deephyper-0.6.0/deephyper/core/cli/templates/nas/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/nas/__init__.py.tmpl
--rw-r--r--   0 romainegele   (501) staff       (20)     1631 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/nas/load_data.py.tmpl
--rw-r--r--   0 romainegele   (501) staff       (20)      950 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/nas/problem.py.tmpl
--rw-r--r--   0 romainegele   (501) staff       (20)     2604 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/core/cli/templates/nas/search_space.py.tmpl
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.519191 deephyper-0.6.0/deephyper/core/exceptions/
--rw-r--r--   0 romainegele   (501) staff       (20)      772 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/exceptions/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      655 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/exceptions/loading.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.519416 deephyper-0.6.0/deephyper/core/exceptions/nas/
--rw-r--r--   0 romainegele   (501) staff       (20)      187 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/exceptions/nas/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1838 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/exceptions/nas/space.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2811 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/exceptions/problem.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1822 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/core/parser.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.520137 deephyper-0.6.0/deephyper/core/utils/
--rw-r--r--   0 romainegele   (501) staff       (20)       56 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/core/utils/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      292 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/utils/_files.py
--rw-r--r--   0 romainegele   (501) staff       (20)      525 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/core/utils/_import.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2257 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/utils/_introspection.py
--rw-r--r--   0 romainegele   (501) staff       (20)      608 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/core/utils/_timeout.py
--rw-r--r--   0 romainegele   (501) staff       (20)      534 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/core/utils/joblib_utils.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.520578 deephyper-0.6.0/deephyper/ensemble/
--rw-r--r--   0 romainegele   (501) staff       (20)      702 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/ensemble/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    11171 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/ensemble/_bagging_ensemble.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3990 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/ensemble/_base_ensemble.py
--rw-r--r--   0 romainegele   (501) staff       (20)    19600 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/ensemble/_uq_bagging_ensemble.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.522654 deephyper-0.6.0/deephyper/evaluator/
--rw-r--r--   0 romainegele   (501) staff       (20)     2731 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2025 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/_decorator.py
--rw-r--r--   0 romainegele   (501) staff       (20)     9193 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_distributed.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2225 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_encoder.py
--rw-r--r--   0 romainegele   (501) staff       (20)    18601 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/_evaluator.py
--rw-r--r--   0 romainegele   (501) staff       (20)     4965 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/_job.py
--rw-r--r--   0 romainegele   (501) staff       (20)     4490 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_mochi_process_pool.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5080 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_mpi_comm.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7828 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/evaluator/_nest_asyncio.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2271 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_process_pool.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1285 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_queued.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5074 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/_ray.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1874 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/_run_function_utils.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2238 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_serial.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2702 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/_thread_pool.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7539 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/callback.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.523295 deephyper-0.6.0/deephyper/evaluator/storage/
--rw-r--r--   0 romainegele   (501) staff       (20)      893 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/storage/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7576 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/evaluator/storage/_memory_storage.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7596 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/storage/_ray_storage.py
--rw-r--r--   0 romainegele   (501) staff       (20)     9461 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/storage/_redis_storage.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7166 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/evaluator/storage/_storage.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.523513 deephyper-0.6.0/deephyper/keras/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/__init__.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.524329 deephyper-0.6.0/deephyper/keras/callbacks/
--rw-r--r--   0 romainegele   (501) staff       (20)      581 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/keras/callbacks/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3539 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/keras/callbacks/csv_extended_logger.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5317 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/callbacks/learning_rate_warmup.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2047 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/callbacks/stop_if_unfeasible.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1364 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/callbacks/stop_on_timeout.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1499 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/callbacks/time_stopping.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1000 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/callbacks/utils.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.524714 deephyper-0.6.0/deephyper/keras/layers/
--rw-r--r--   0 romainegele   (501) staff       (20)      960 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/layers/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    36142 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/keras/layers/_mpnn.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1788 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/layers/_padding.py
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/keras/utils.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.525549 deephyper-0.6.0/deephyper/nas/
--rw-r--r--   0 romainegele   (501) staff       (20)      818 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/nas/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7837 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/_keras_search_space.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7301 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/_nx_search_space.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1605 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/losses.py
--rw-r--r--   0 romainegele   (501) staff       (20)      262 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/nas/lr_scheduler.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3474 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/metrics.py
--rw-r--r--   0 romainegele   (501) staff       (20)     8363 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/node.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.525874 deephyper-0.6.0/deephyper/nas/operation/
--rw-r--r--   0 romainegele   (501) staff       (20)      370 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/nas/operation/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     4141 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/operation/_base.py
--rw-r--r--   0 romainegele   (501) staff       (20)     8004 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/nas/operation/_merge.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.526095 deephyper-0.6.0/deephyper/nas/preprocessing/
--rw-r--r--   0 romainegele   (501) staff       (20)       90 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/nas/preprocessing/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1247 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/nas/preprocessing/_base.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.527303 deephyper-0.6.0/deephyper/nas/run/
--rw-r--r--   0 romainegele   (501) staff       (20)      733 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/run/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     4751 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/run/_run_base_trainer.py
--rw-r--r--   0 romainegele   (501) staff       (20)      645 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/nas/run/_run_debug.py
--rw-r--r--   0 romainegele   (501) staff       (20)      343 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/nas/run/_run_debug_arch.py
--rw-r--r--   0 romainegele   (501) staff       (20)      770 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/nas/run/_run_debug_hp_arch.py
--rw-r--r--   0 romainegele   (501) staff       (20)      680 2023-01-27 13:53:43.000000 deephyper-0.6.0/deephyper/nas/run/_run_debug_slow.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6405 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/run/_run_distributed_base_trainer.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6420 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/run/_run_horovod.py
--rw-r--r--   0 romainegele   (501) staff       (20)      722 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/nas/run/_test_horovod.py
--rw-r--r--   0 romainegele   (501) staff       (20)    12348 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/run/_util.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.527425 deephyper-0.6.0/deephyper/nas/spacelib/
--rw-r--r--   0 romainegele   (501) staff       (20)       52 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/nas/spacelib/__init__.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.528029 deephyper-0.6.0/deephyper/nas/spacelib/tabular/
--rw-r--r--   0 romainegele   (501) staff       (20)      373 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/nas/spacelib/tabular/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2637 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/nas/spacelib/tabular/dense_skipco.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2179 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/nas/spacelib/tabular/feed_forward.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1655 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/nas/spacelib/tabular/one_layer.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2268 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/nas/spacelib/tabular/supervised_reg_auto_encoder.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.528607 deephyper-0.6.0/deephyper/nas/trainer/
--rw-r--r--   0 romainegele   (501) staff       (20)      184 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/trainer/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      973 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/nas/trainer/_arch.py
--rw-r--r--   0 romainegele   (501) staff       (20)    21958 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/nas/trainer/_base.py
--rw-r--r--   0 romainegele   (501) staff       (20)    21070 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/nas/trainer/_horovod.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1156 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/nas/trainer/_utils.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.528934 deephyper-0.6.0/deephyper/problem/
--rw-r--r--   0 romainegele   (501) staff       (20)      875 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/problem/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    12172 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/problem/_hyperparameter.py
--rw-r--r--   0 romainegele   (501) staff       (20)    19985 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/problem/_neuralarchitecture.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.529171 deephyper-0.6.0/deephyper/search/
--rw-r--r--   0 romainegele   (501) staff       (20)      663 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/search/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7307 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/search/_search.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.529547 deephyper-0.6.0/deephyper/search/hps/
--rw-r--r--   0 romainegele   (501) staff       (20)      457 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/search/hps/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    45010 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/search/hps/_cbo.py
--rw-r--r--   0 romainegele   (501) staff       (20)    16247 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/search/hps/_mpi_dbo.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.530346 deephyper-0.6.0/deephyper/search/nas/
--rw-r--r--   0 romainegele   (501) staff       (20)      733 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/search/nas/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    14052 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/search/nas/_agebo.py
--rw-r--r--   0 romainegele   (501) staff       (20)     9952 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/search/nas/_ambsmixed.py
--rw-r--r--   0 romainegele   (501) staff       (20)      771 2022-06-09 07:10:12.000000 deephyper-0.6.0/deephyper/search/nas/_base.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3028 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/search/nas/_random.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5662 2023-08-21 14:54:30.000000 deephyper-0.6.0/deephyper/search/nas/_regevo.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6069 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/search/nas/_regevomixed.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.530459 deephyper-0.6.0/deephyper/sklearn/
--rw-r--r--   0 romainegele   (501) staff       (20)       47 2022-04-11 13:44:35.000000 deephyper-0.6.0/deephyper/sklearn/__init__.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.530686 deephyper-0.6.0/deephyper/sklearn/classifier/
--rw-r--r--   0 romainegele   (501) staff       (20)      342 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/sklearn/classifier/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6739 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/sklearn/classifier/_autosklearn1.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.530910 deephyper-0.6.0/deephyper/sklearn/regressor/
--rw-r--r--   0 romainegele   (501) staff       (20)      341 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/sklearn/regressor/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6472 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/sklearn/regressor/_autosklearn1.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.531815 deephyper-0.6.0/deephyper/skopt/
--rw-r--r--   0 romainegele   (501) staff       (20)     4406 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    10975 2022-11-15 14:19:01.000000 deephyper-0.6.0/deephyper/skopt/acquisition.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2888 2022-10-19 18:01:05.000000 deephyper-0.6.0/deephyper/skopt/benchmarks.py
--rw-r--r--   0 romainegele   (501) staff       (20)     9497 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/skopt/callbacks.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.532238 deephyper-0.6.0/deephyper/skopt/learning/
--rw-r--r--   0 romainegele   (501) staff       (20)      553 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/learning/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    20515 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/learning/forest.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.532647 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/
--rw-r--r--   0 romainegele   (501) staff       (20)       94 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    15391 2022-10-19 18:01:05.000000 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/gpr.py
--rw-r--r--   0 romainegele   (501) staff       (20)    14672 2022-10-19 18:01:05.000000 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/kernels.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.532978 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/tests/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/tests/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3818 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/tests/test_gpr.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7824 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/tests/test_kernels.py
--rw-r--r--   0 romainegele   (501) staff       (20)     4713 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/learning/gbrt.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.533297 deephyper-0.6.0/deephyper/skopt/learning/tests/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/skopt/learning/tests/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3034 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/learning/tests/test_forest.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3191 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/skopt/learning/tests/test_gbrt.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.533795 deephyper-0.6.0/deephyper/skopt/moo/
--rw-r--r--   0 romainegele   (501) staff       (20)     2951 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/moo/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    12023 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/moo/_hv.py
--rw-r--r--   0 romainegele   (501) staff       (20)    11209 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/moo/_multiobjective.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5596 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/moo/_pf.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.534655 deephyper-0.6.0/deephyper/skopt/optimizer/
--rw-r--r--   0 romainegele   (501) staff       (20)      390 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/skopt/optimizer/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    12427 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/optimizer/base.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5020 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/optimizer/dummy.py
--rw-r--r--   0 romainegele   (501) staff       (20)     8325 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/optimizer/forest.py
--rw-r--r--   0 romainegele   (501) staff       (20)     7968 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/optimizer/gbrt.py
--rw-r--r--   0 romainegele   (501) staff       (20)    11926 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/optimizer/gp.py
--rw-r--r--   0 romainegele   (501) staff       (20)    50530 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/optimizer/optimizer.py
--rw-r--r--   0 romainegele   (501) staff       (20)    51782 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/plots.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.535730 deephyper-0.6.0/deephyper/skopt/sampler/
--rw-r--r--   0 romainegele   (501) staff       (20)      305 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/skopt/sampler/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      655 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/sampler/base.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6274 2022-10-19 18:01:05.000000 deephyper-0.6.0/deephyper/skopt/sampler/grid.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5951 2022-10-19 18:01:05.000000 deephyper-0.6.0/deephyper/skopt/sampler/halton.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3556 2022-07-12 07:29:08.000000 deephyper-0.6.0/deephyper/skopt/sampler/hammersly.py
--rw-r--r--   0 romainegele   (501) staff       (20)     5671 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/sampler/lhs.py
--rw-r--r--   0 romainegele   (501) staff       (20)    18637 2022-10-19 18:01:05.000000 deephyper-0.6.0/deephyper/skopt/sampler/sobol.py
--rw-r--r--   0 romainegele   (501) staff       (20)    20969 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/searchcv.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.536252 deephyper-0.6.0/deephyper/skopt/space/
--rw-r--r--   0 romainegele   (501) staff       (20)       86 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/space/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)    50995 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/space/space.py
--rw-r--r--   0 romainegele   (501) staff       (20)     8914 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/skopt/space/transformers.py
--rw-r--r--   0 romainegele   (501) staff       (20)    29472 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/skopt/utils.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.537250 deephyper-0.6.0/deephyper/stopper/
--rw-r--r--   0 romainegele   (501) staff       (20)     4487 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     6000 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/_asha_stopper.py
--rw-r--r--   0 romainegele   (501) staff       (20)      812 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/_const_stopper.py
--rw-r--r--   0 romainegele   (501) staff       (20)      368 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/_idle_stopper.py
--rw-r--r--   0 romainegele   (501) staff       (20)    19513 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/_lcmodel_stopper.py
--rw-r--r--   0 romainegele   (501) staff       (20)     3189 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/_median_stopper.py
--rw-r--r--   0 romainegele   (501) staff       (20)     2747 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/_stopper.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.537666 deephyper-0.6.0/deephyper/stopper/integration/
--rw-r--r--   0 romainegele   (501) staff       (20)       85 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/integration/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1823 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/integration/deepxde.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1737 2023-08-21 14:53:56.000000 deephyper-0.6.0/deephyper/stopper/integration/tensorflow.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.538047 deephyper-0.6.0/deephyper/test/
--rw-r--r--   0 romainegele   (501) staff       (20)      170 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/test/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      711 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/_command.py
--rw-r--r--   0 romainegele   (501) staff       (20)      405 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/test/_parse_result.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.538155 deephyper-0.6.0/deephyper/test/nas/
--rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/__init__.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.538534 deephyper-0.6.0/deephyper/test/nas/linearReg/
--rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/test/nas/linearReg/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      897 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/linearReg/load_data.py
--rw-r--r--   0 romainegele   (501) staff       (20)      611 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/linearReg/problem.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.538895 deephyper-0.6.0/deephyper/test/nas/linearRegHybrid/
--rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/test/nas/linearRegHybrid/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)      897 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/linearRegHybrid/load_data.py
--rw-r--r--   0 romainegele   (501) staff       (20)      817 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/linearRegHybrid/problem.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.539327 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputs/
--rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputs/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1047 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputs/load_data.py
--rw-r--r--   0 romainegele   (501) staff       (20)      678 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputs/problem.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.539716 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputsGen/
--rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputsGen/__init__.py
--rw-r--r--   0 romainegele   (501) staff       (20)     1408 2023-04-18 19:40:47.000000 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputsGen/load_data.py
--rw-r--r--   0 romainegele   (501) staff       (20)      680 2022-11-02 12:44:29.000000 deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputsGen/problem.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.514806 deephyper-0.6.0/deephyper.egg-info/
--rw-r--r--   0 romainegele   (501) staff       (20)    10794 2023-08-21 15:21:32.000000 deephyper-0.6.0/deephyper.egg-info/PKG-INFO
--rw-r--r--   0 romainegele   (501) staff       (20)     7705 2023-08-21 15:21:32.000000 deephyper-0.6.0/deephyper.egg-info/SOURCES.txt
--rw-r--r--   0 romainegele   (501) staff       (20)        1 2023-08-21 15:21:32.000000 deephyper-0.6.0/deephyper.egg-info/dependency_links.txt
--rw-r--r--   0 romainegele   (501) staff       (20)      122 2023-08-21 15:21:32.000000 deephyper-0.6.0/deephyper.egg-info/entry_points.txt
--rw-r--r--   0 romainegele   (501) staff       (20)     1132 2023-08-21 15:21:32.000000 deephyper-0.6.0/deephyper.egg-info/requires.txt
--rw-r--r--   0 romainegele   (501) staff       (20)       10 2023-08-21 15:21:32.000000 deephyper-0.6.0/deephyper.egg-info/top_level.txt
--rw-r--r--   0 romainegele   (501) staff       (20)      242 2023-04-18 19:40:50.000000 deephyper-0.6.0/pyproject.toml
--rw-r--r--   0 romainegele   (501) staff       (20)     1504 2023-08-21 15:21:32.540441 deephyper-0.6.0/setup.cfg
--rw-r--r--   0 romainegele   (501) staff       (20)     5776 2023-08-21 14:53:58.000000 deephyper-0.6.0/setup.py
-drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2023-08-21 15:21:32.539835 deephyper-0.6.0/tests/
--rw-r--r--   0 romainegele   (501) staff       (20)     1432 2023-04-18 19:40:50.000000 deephyper-0.6.0/tests/test_quickstart.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.941745 deephyper-0.7.0/
+-rw-r--r--   0 romainegele   (501) staff       (20)     1531 2023-04-18 19:40:47.000000 deephyper-0.7.0/LICENSE.md
+-rw-r--r--   0 romainegele   (501) staff       (20)       99 2021-11-16 07:10:00.000000 deephyper-0.7.0/MANIFEST.in
+-rw-r--r--   0 romainegele   (501) staff       (20)    14523 2024-04-04 07:29:02.941574 deephyper-0.7.0/PKG-INFO
+-rw-r--r--   0 romainegele   (501) staff       (20)     9348 2024-04-04 07:05:19.000000 deephyper-0.7.0/README.md
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.908834 deephyper-0.7.0/deephyper/
+-rw-r--r--   0 romainegele   (501) staff       (20)     1297 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      109 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/__version__.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.910344 deephyper-0.7.0/deephyper/analysis/
+-rw-r--r--   0 romainegele   (501) staff       (20)      130 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/analysis/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1700 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/analysis/_matplotlib.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    26720 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/analysis/_paxplot.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1405 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/analysis/_rank.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    13215 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/analysis/hpo.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.910589 deephyper-0.7.0/deephyper/core/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/__init__.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.911374 deephyper-0.7.0/deephyper/core/analytics/
+-rw-r--r--   0 romainegele   (501) staff       (20)      301 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/core/analytics/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1364 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/analytics/_analytics.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1222 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/analytics/_dashboard.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     9098 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/analytics/_db_manager.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5701 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/analytics/_quick_plot.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     4269 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/analytics/_topk.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.911765 deephyper-0.7.0/deephyper/core/analytics/dashboard/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/analytics/dashboard/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3507 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/analytics/dashboard/_pyplot.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    20546 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/analytics/dashboard/_views.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.912903 deephyper-0.7.0/deephyper/core/cli/
+-rw-r--r--   0 romainegele   (501) staff       (20)      205 2023-07-05 07:15:50.000000 deephyper-0.7.0/deephyper/core/cli/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1600 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/_cli.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      827 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/cli/_cobalt_nodelist.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6917 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/cli/_hps.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6849 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/cli/_nas.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2325 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/cli/_new_problem.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      938 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/cli/_nodelist.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1811 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/cli/_start_project.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.904368 deephyper-0.7.0/deephyper/core/cli/templates/
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.913403 deephyper-0.7.0/deephyper/core/cli/templates/hps/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/hps/__init__.py.tmpl
+-rw-r--r--   0 romainegele   (501) staff       (20)     1631 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/hps/load_data.py.tmpl
+-rw-r--r--   0 romainegele   (501) staff       (20)     1254 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/hps/model_run.py.tmpl
+-rw-r--r--   0 romainegele   (501) staff       (20)      357 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/hps/problem.py.tmpl
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.913866 deephyper-0.7.0/deephyper/core/cli/templates/nas/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/nas/__init__.py.tmpl
+-rw-r--r--   0 romainegele   (501) staff       (20)     1631 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/nas/load_data.py.tmpl
+-rw-r--r--   0 romainegele   (501) staff       (20)      950 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/nas/problem.py.tmpl
+-rw-r--r--   0 romainegele   (501) staff       (20)     2604 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/core/cli/templates/nas/search_space.py.tmpl
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.914230 deephyper-0.7.0/deephyper/core/exceptions/
+-rw-r--r--   0 romainegele   (501) staff       (20)      887 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/core/exceptions/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      655 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/exceptions/loading.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.914469 deephyper-0.7.0/deephyper/core/exceptions/nas/
+-rw-r--r--   0 romainegele   (501) staff       (20)      187 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/exceptions/nas/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1838 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/exceptions/nas/space.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2811 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/exceptions/problem.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1822 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/core/parser.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.915228 deephyper-0.7.0/deephyper/core/utils/
+-rw-r--r--   0 romainegele   (501) staff       (20)      123 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/core/utils/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      292 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/utils/_files.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      525 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/core/utils/_import.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2257 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/core/utils/_introspection.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      951 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/core/utils/_timeout.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      534 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/core/utils/joblib_utils.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.915715 deephyper-0.7.0/deephyper/ensemble/
+-rw-r--r--   0 romainegele   (501) staff       (20)      702 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/ensemble/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    11171 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/ensemble/_bagging_ensemble.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3990 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/ensemble/_base_ensemble.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    19600 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/ensemble/_uq_bagging_ensemble.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.917952 deephyper-0.7.0/deephyper/evaluator/
+-rw-r--r--   0 romainegele   (501) staff       (20)     2731 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2025 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/_decorator.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     9193 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/_distributed.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2225 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/_encoder.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    19925 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/evaluator/_evaluator.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5033 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/evaluator/_job.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     4490 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/_mochi_process_pool.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5317 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/evaluator/_mpi_comm.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7828 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/evaluator/_nest_asyncio.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2271 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/_process_pool.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1285 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/_queued.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5074 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/_ray.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1874 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/_run_function_utils.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2238 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/_serial.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2702 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/_thread_pool.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     8506 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/evaluator/callback.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.918672 deephyper-0.7.0/deephyper/evaluator/storage/
+-rw-r--r--   0 romainegele   (501) staff       (20)      893 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/storage/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7576 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/evaluator/storage/_memory_storage.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7596 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/storage/_ray_storage.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     9461 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/storage/_redis_storage.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7166 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/evaluator/storage/_storage.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.918938 deephyper-0.7.0/deephyper/keras/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/__init__.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.919850 deephyper-0.7.0/deephyper/keras/callbacks/
+-rw-r--r--   0 romainegele   (501) staff       (20)      581 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/keras/callbacks/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3539 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/keras/callbacks/csv_extended_logger.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5317 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/callbacks/learning_rate_warmup.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2047 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/callbacks/stop_if_unfeasible.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1364 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/callbacks/stop_on_timeout.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1499 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/callbacks/time_stopping.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1000 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/callbacks/utils.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.920253 deephyper-0.7.0/deephyper/keras/layers/
+-rw-r--r--   0 romainegele   (501) staff       (20)      960 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/layers/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    36142 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/keras/layers/_mpnn.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1788 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/layers/_padding.py
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/keras/utils.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.921256 deephyper-0.7.0/deephyper/nas/
+-rw-r--r--   0 romainegele   (501) staff       (20)      818 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/nas/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7837 2024-03-28 14:31:00.000000 deephyper-0.7.0/deephyper/nas/_keras_search_space.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7301 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/_nx_search_space.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1605 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/losses.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      262 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/nas/lr_scheduler.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3474 2024-03-28 14:31:00.000000 deephyper-0.7.0/deephyper/nas/metrics.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     8363 2024-03-28 14:31:00.000000 deephyper-0.7.0/deephyper/nas/node.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.921697 deephyper-0.7.0/deephyper/nas/operation/
+-rw-r--r--   0 romainegele   (501) staff       (20)      370 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/nas/operation/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     4141 2024-03-28 14:31:00.000000 deephyper-0.7.0/deephyper/nas/operation/_base.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     8004 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/nas/operation/_merge.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.921999 deephyper-0.7.0/deephyper/nas/preprocessing/
+-rw-r--r--   0 romainegele   (501) staff       (20)       90 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/nas/preprocessing/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1247 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/nas/preprocessing/_base.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.923478 deephyper-0.7.0/deephyper/nas/run/
+-rw-r--r--   0 romainegele   (501) staff       (20)      733 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/run/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     4751 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/run/_run_base_trainer.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      645 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/nas/run/_run_debug.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      343 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/nas/run/_run_debug_arch.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      770 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/nas/run/_run_debug_hp_arch.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      680 2023-01-27 13:53:43.000000 deephyper-0.7.0/deephyper/nas/run/_run_debug_slow.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6405 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/run/_run_distributed_base_trainer.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6420 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/run/_run_horovod.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      722 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/nas/run/_test_horovod.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    12348 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/run/_util.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.923638 deephyper-0.7.0/deephyper/nas/spacelib/
+-rw-r--r--   0 romainegele   (501) staff       (20)       52 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/nas/spacelib/__init__.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.924259 deephyper-0.7.0/deephyper/nas/spacelib/tabular/
+-rw-r--r--   0 romainegele   (501) staff       (20)      373 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/nas/spacelib/tabular/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2637 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/nas/spacelib/tabular/dense_skipco.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2179 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/nas/spacelib/tabular/feed_forward.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1655 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/nas/spacelib/tabular/one_layer.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2268 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/nas/spacelib/tabular/supervised_reg_auto_encoder.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.924904 deephyper-0.7.0/deephyper/nas/trainer/
+-rw-r--r--   0 romainegele   (501) staff       (20)      184 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/trainer/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      973 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/nas/trainer/_arch.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    21958 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/nas/trainer/_base.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    21070 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/nas/trainer/_horovod.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1156 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/nas/trainer/_utils.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.925301 deephyper-0.7.0/deephyper/problem/
+-rw-r--r--   0 romainegele   (501) staff       (20)      875 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/problem/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    12308 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/problem/_hyperparameter.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    19985 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/problem/_neuralarchitecture.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.925560 deephyper-0.7.0/deephyper/search/
+-rw-r--r--   0 romainegele   (501) staff       (20)      663 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/search/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     8585 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/search/_search.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.926084 deephyper-0.7.0/deephyper/search/hps/
+-rw-r--r--   0 romainegele   (501) staff       (20)      549 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/search/hps/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    52499 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/search/hps/_cbo.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2263 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/search/hps/_eds.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    16707 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/search/hps/_mpi_dbo.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.927021 deephyper-0.7.0/deephyper/search/nas/
+-rw-r--r--   0 romainegele   (501) staff       (20)      733 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/search/nas/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    14386 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/search/nas/_agebo.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    10213 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/search/nas/_ambsmixed.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      771 2022-06-09 07:10:12.000000 deephyper-0.7.0/deephyper/search/nas/_base.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3028 2023-09-27 12:06:41.000000 deephyper-0.7.0/deephyper/search/nas/_random.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5662 2023-09-27 12:06:43.000000 deephyper-0.7.0/deephyper/search/nas/_regevo.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6069 2023-09-27 12:06:45.000000 deephyper-0.7.0/deephyper/search/nas/_regevomixed.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.927190 deephyper-0.7.0/deephyper/sklearn/
+-rw-r--r--   0 romainegele   (501) staff       (20)       47 2022-04-11 13:44:35.000000 deephyper-0.7.0/deephyper/sklearn/__init__.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.927434 deephyper-0.7.0/deephyper/sklearn/classifier/
+-rw-r--r--   0 romainegele   (501) staff       (20)      342 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/sklearn/classifier/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6739 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/sklearn/classifier/_autosklearn1.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.927754 deephyper-0.7.0/deephyper/sklearn/regressor/
+-rw-r--r--   0 romainegele   (501) staff       (20)      341 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/sklearn/regressor/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6472 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/sklearn/regressor/_autosklearn1.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.928856 deephyper-0.7.0/deephyper/skopt/
+-rw-r--r--   0 romainegele   (501) staff       (20)     4406 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/skopt/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    15452 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/acquisition.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2888 2022-10-19 18:01:05.000000 deephyper-0.7.0/deephyper/skopt/benchmarks.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     9497 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/skopt/callbacks.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.929263 deephyper-0.7.0/deephyper/skopt/learning/
+-rw-r--r--   0 romainegele   (501) staff       (20)      553 2023-10-19 09:03:07.000000 deephyper-0.7.0/deephyper/skopt/learning/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    23704 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/learning/forest.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.929736 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/
+-rw-r--r--   0 romainegele   (501) staff       (20)       94 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    15391 2022-10-19 18:01:05.000000 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/gpr.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    14672 2022-10-19 18:01:05.000000 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/kernels.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.930135 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/tests/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/tests/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3818 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/tests/test_gpr.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7824 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/tests/test_kernels.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5193 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/learning/gbrt.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.930552 deephyper-0.7.0/deephyper/skopt/learning/tests/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/skopt/learning/tests/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3034 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/learning/tests/test_forest.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3191 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/skopt/learning/tests/test_gbrt.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.931105 deephyper-0.7.0/deephyper/skopt/moo/
+-rw-r--r--   0 romainegele   (501) staff       (20)     2951 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/skopt/moo/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    12023 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/skopt/moo/_hv.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    11209 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/skopt/moo/_multiobjective.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5879 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/moo/_pf.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.932477 deephyper-0.7.0/deephyper/skopt/optimizer/
+-rw-r--r--   0 romainegele   (501) staff       (20)      390 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/skopt/optimizer/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3563 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/optimizer/_pymoo.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    12427 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/optimizer/base.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5020 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/optimizer/dummy.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     8325 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/optimizer/forest.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     7968 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/optimizer/gbrt.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    11926 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/optimizer/gp.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    58778 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/optimizer/optimizer.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    51782 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/plots.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.933660 deephyper-0.7.0/deephyper/skopt/sampler/
+-rw-r--r--   0 romainegele   (501) staff       (20)      305 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/skopt/sampler/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      655 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/sampler/base.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6274 2022-10-19 18:01:05.000000 deephyper-0.7.0/deephyper/skopt/sampler/grid.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5951 2022-10-19 18:01:05.000000 deephyper-0.7.0/deephyper/skopt/sampler/halton.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3556 2022-07-12 07:29:08.000000 deephyper-0.7.0/deephyper/skopt/sampler/hammersly.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     5671 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/sampler/lhs.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    18637 2022-10-19 18:01:05.000000 deephyper-0.7.0/deephyper/skopt/sampler/sobol.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    20969 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/searchcv.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.934151 deephyper-0.7.0/deephyper/skopt/space/
+-rw-r--r--   0 romainegele   (501) staff       (20)       86 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/skopt/space/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    46919 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/space/space.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     8914 2023-11-16 17:34:55.000000 deephyper-0.7.0/deephyper/skopt/space/transformers.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    29428 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/skopt/utils.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.935255 deephyper-0.7.0/deephyper/stopper/
+-rw-r--r--   0 romainegele   (501) staff       (20)     4487 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/stopper/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     6005 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/stopper/_asha_stopper.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      807 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/stopper/_const_stopper.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      368 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/stopper/_idle_stopper.py
+-rw-r--r--   0 romainegele   (501) staff       (20)    23864 2024-04-04 07:05:19.000000 deephyper-0.7.0/deephyper/stopper/_lcmodel_stopper.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     3189 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/stopper/_median_stopper.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     2747 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/stopper/_stopper.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.935703 deephyper-0.7.0/deephyper/stopper/integration/
+-rw-r--r--   0 romainegele   (501) staff       (20)       85 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/stopper/integration/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1823 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/stopper/integration/deepxde.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1737 2023-08-21 14:53:56.000000 deephyper-0.7.0/deephyper/stopper/integration/tensorflow.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.936131 deephyper-0.7.0/deephyper/test/
+-rw-r--r--   0 romainegele   (501) staff       (20)      170 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/test/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      711 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/_command.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      405 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/test/_parse_result.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.936268 deephyper-0.7.0/deephyper/test/nas/
+-rw-r--r--   0 romainegele   (501) staff       (20)        0 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/__init__.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.936671 deephyper-0.7.0/deephyper/test/nas/linearReg/
+-rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/test/nas/linearReg/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      897 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/linearReg/load_data.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      611 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/linearReg/problem.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.937089 deephyper-0.7.0/deephyper/test/nas/linearRegHybrid/
+-rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/test/nas/linearRegHybrid/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      897 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/linearRegHybrid/load_data.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      817 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/linearRegHybrid/problem.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.937506 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputs/
+-rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputs/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1047 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputs/load_data.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      678 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputs/problem.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.937952 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputsGen/
+-rw-r--r--   0 romainegele   (501) staff       (20)       43 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputsGen/__init__.py
+-rw-r--r--   0 romainegele   (501) staff       (20)     1408 2023-04-18 19:40:47.000000 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputsGen/load_data.py
+-rw-r--r--   0 romainegele   (501) staff       (20)      680 2022-11-02 12:44:29.000000 deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputsGen/problem.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.938328 deephyper-0.7.0/deephyper.egg-info/
+-rw-r--r--   0 romainegele   (501) staff       (20)    14523 2024-04-04 07:29:02.000000 deephyper-0.7.0/deephyper.egg-info/PKG-INFO
+-rw-r--r--   0 romainegele   (501) staff       (20)     7835 2024-04-04 07:29:02.000000 deephyper-0.7.0/deephyper.egg-info/SOURCES.txt
+-rw-r--r--   0 romainegele   (501) staff       (20)        1 2024-04-04 07:29:02.000000 deephyper-0.7.0/deephyper.egg-info/dependency_links.txt
+-rw-r--r--   0 romainegele   (501) staff       (20)      122 2024-04-04 07:29:02.000000 deephyper-0.7.0/deephyper.egg-info/entry_points.txt
+-rw-r--r--   0 romainegele   (501) staff       (20)     1183 2024-04-04 07:29:02.000000 deephyper-0.7.0/deephyper.egg-info/requires.txt
+-rw-r--r--   0 romainegele   (501) staff       (20)       10 2024-04-04 07:29:02.000000 deephyper-0.7.0/deephyper.egg-info/top_level.txt
+-rw-r--r--   0 romainegele   (501) staff       (20)      242 2023-04-18 19:40:50.000000 deephyper-0.7.0/pyproject.toml
+-rw-r--r--   0 romainegele   (501) staff       (20)     1504 2024-04-04 07:29:02.942061 deephyper-0.7.0/setup.cfg
+-rw-r--r--   0 romainegele   (501) staff       (20)     5827 2024-04-04 07:08:55.000000 deephyper-0.7.0/setup.py
+drwxr-xr-x   0 romainegele   (501) staff       (20)        0 2024-04-04 07:29:02.938098 deephyper-0.7.0/tests/
+-rw-r--r--   0 romainegele   (501) staff       (20)     1432 2023-04-18 19:40:50.000000 deephyper-0.7.0/tests/test_quickstart.py
```

### Comparing `deephyper-0.6.0/LICENSE.md` & `deephyper-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/PKG-INFO` & `deephyper-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,7 @@
-Metadata-Version: 2.1
-Name: deephyper
-Version: 0.6.0
-Summary: Scalable asynchronous neural architecture and hyperparameter search for deep neural networks.
-Home-page: https://github.com/deephyper
-Author: Prasanna Balaprakash <pbalapra@ornl.gov>, Romain Egele <romainegele@gmail.com>, Misha Salim, Romit Maulik, Venkat Vishwanath, Stefan Wild
-Maintainer: Prasanna Balaprakash
-Maintainer-email: pbalapra@ornl.gov
-License: BSD 3-clause
-Project-URL: Documentation, http://deephyper.readthedocs.io
-Project-URL: Changes, https://github.com/deephyper/deephyper/releases
-Project-URL: Source Code, https://github.com/deephyper/deephyper
-Project-URL: Issue Tracker, https://github.com/deephyper/deephyper/issues
-Project-URL: Discussion, https://github.com/deephyper/deephyper/discussions
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: autodeuq
-Provides-Extra: automl
-Provides-Extra: jax-cpu
-Provides-Extra: jax-cuda
-Provides-Extra: hps
-Provides-Extra: nas
-Provides-Extra: hps-tl
-Provides-Extra: mpi
-Provides-Extra: ray
-Provides-Extra: redis
-Provides-Extra: dev
-Provides-Extra: analytics
-Provides-Extra: hvd
-Provides-Extra: default
-License-File: LICENSE.md
-
 <p align="center">
 <img src="docs/_static/logo/medium.png">
 </p>
 
 [![DOI](https://zenodo.org/badge/156403341.svg)](https://zenodo.org/badge/latestdoi/156403341)
 ![GitHub tag (latest by date)](https://img.shields.io/github/tag-date/deephyper/deephyper.svg?label=version)
 [![Documentation Status](https://readthedocs.org/projects/deephyper/badge/?version=latest)](https://deephyper.readthedocs.io/en/latest/?badge=latest)
@@ -73,15 +33,15 @@
 
 More details about the installation process can be found at [DeepHyper Installations](https://deephyper.readthedocs.io/en/latest/install/index.html).
 
 ## Quickstart
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/deephyper/tutorials/blob/main/tutorials/colab/DeepHyper_101.ipynb)
 
-The black-box function named `run` is defined by taking an input dictionary named `config`` which contains the different variables to optimize. Then the run-function is bound to an `Evaluator` in charge of distributing the computation of multiple evaluations. Finally, a Bayesian search named `CBO` is created and executed to find the values of config which **MAXIMIZE** the return value of `run(config)`.
+The black-box function named `run` is defined by taking an input job named `job` which contains the different variables to optimize `job.parameters`. Then the run-function is bound to an `Evaluator` in charge of distributing the computation of multiple evaluations. Finally, a Bayesian search named `CBO` is created and executed to find the values of config which **MAXIMIZE** the return value of `run(job)`.
 
 ```python
 def run(job):
     # The suggested parameters are accessible in job.parameters (dict)
     x = job.parameters["x"]
     b = job.parameters["b"]
 
@@ -165,19 +125,19 @@
 
 ## Citing DeepHyper
 
 If you wish to cite the Software, please use the following:
 
 ```
 @misc{deephyper_software,
-title = {"DeepHyper: A Python Package for Scalable Neural Architecture and Hyperparameter Search"},
-author = {{DeepHyper Development Team}},
-organization = {DeepHyper Team},
-year = 2018,
-url = {https://github.com/deephyper/deephyper}
+    title = {"DeepHyper: A Python Package for Scalable Neural Architecture and Hyperparameter Search"},
+    author = {Balaprakash, Prasanna and Egele, Romain and Salim, Misha and Maulik, Romit and Vishwanath, Venkat and Wild, Stefan and others},
+    organization = {DeepHyper Team},
+    year = 2018,
+    url = {https://github.com/deephyper/deephyper}
 } 
 ```
 
 Find all our publications on the [Research & Publication](https://deephyper.github.io/papers) page of the Documentation.
 
 ## How can I participate?
```

### Comparing `deephyper-0.6.0/deephyper/__init__.py` & `deephyper-0.7.0/deephyper/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/analytics/_analytics.py` & `deephyper-0.7.0/deephyper/core/analytics/_analytics.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/analytics/_dashboard.py` & `deephyper-0.7.0/deephyper/core/analytics/_dashboard.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/analytics/_db_manager.py` & `deephyper-0.7.0/deephyper/core/analytics/_db_manager.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/analytics/_quick_plot.py` & `deephyper-0.7.0/deephyper/core/analytics/_quick_plot.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/analytics/_topk.py` & `deephyper-0.7.0/deephyper/core/analytics/_topk.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/analytics/dashboard/_pyplot.py` & `deephyper-0.7.0/deephyper/core/analytics/dashboard/_pyplot.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/analytics/dashboard/_views.py` & `deephyper-0.7.0/deephyper/core/analytics/dashboard/_views.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/_cli.py` & `deephyper-0.7.0/deephyper/core/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/_cobalt_nodelist.py` & `deephyper-0.7.0/deephyper/core/cli/_cobalt_nodelist.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/_hps.py` & `deephyper-0.7.0/deephyper/core/cli/_hps.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/_nas.py` & `deephyper-0.7.0/deephyper/core/cli/_nas.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/_new_problem.py` & `deephyper-0.7.0/deephyper/core/cli/_new_problem.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/_nodelist.py` & `deephyper-0.7.0/deephyper/core/cli/_nodelist.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/_start_project.py` & `deephyper-0.7.0/deephyper/core/cli/_start_project.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/templates/hps/load_data.py.tmpl` & `deephyper-0.7.0/deephyper/core/cli/templates/hps/load_data.py.tmpl`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/templates/hps/model_run.py.tmpl` & `deephyper-0.7.0/deephyper/core/cli/templates/hps/model_run.py.tmpl`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/templates/nas/load_data.py.tmpl` & `deephyper-0.7.0/deephyper/core/cli/templates/nas/load_data.py.tmpl`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/templates/nas/problem.py.tmpl` & `deephyper-0.7.0/deephyper/core/cli/templates/nas/problem.py.tmpl`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/cli/templates/nas/search_space.py.tmpl` & `deephyper-0.7.0/deephyper/core/cli/templates/nas/search_space.py.tmpl`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/exceptions/__init__.py` & `deephyper-0.7.0/deephyper/core/exceptions/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
 
 class DeephyperRuntimeError(RuntimeError):
     """Raised when an error is detected in deephyper and that doesn’t fall in any of the other categories. The associated value is a string indicating what precisely went wrong."""
 
 
 class SearchTerminationError(RuntimeError):
-    """Raised when a search receives SIGALARM"""
+    """Raised when a search is terminated."""
+
+
+class MaximumJobsSpawnReached(SearchTerminationError):
+    """Raised when the maximum number of jobs is reached."""
 
 
 class RunFunctionError(RuntimeError):
     """Raised when error occurs in run-function"""
 
     def __init__(self, msg: str = None) -> None:
         self.msg = msg
```

### Comparing `deephyper-0.6.0/deephyper/core/exceptions/loading.py` & `deephyper-0.7.0/deephyper/core/exceptions/loading.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/exceptions/nas/space.py` & `deephyper-0.7.0/deephyper/core/exceptions/nas/space.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/exceptions/problem.py` & `deephyper-0.7.0/deephyper/core/exceptions/problem.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/parser.py` & `deephyper-0.7.0/deephyper/core/parser.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/utils/_import.py` & `deephyper-0.7.0/deephyper/core/utils/_import.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/utils/_introspection.py` & `deephyper-0.7.0/deephyper/core/utils/_introspection.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/core/utils/joblib_utils.py` & `deephyper-0.7.0/deephyper/core/utils/joblib_utils.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/ensemble/__init__.py` & `deephyper-0.7.0/deephyper/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/ensemble/_bagging_ensemble.py` & `deephyper-0.7.0/deephyper/ensemble/_bagging_ensemble.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/ensemble/_base_ensemble.py` & `deephyper-0.7.0/deephyper/ensemble/_base_ensemble.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/ensemble/_uq_bagging_ensemble.py` & `deephyper-0.7.0/deephyper/ensemble/_uq_bagging_ensemble.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/__init__.py` & `deephyper-0.7.0/deephyper/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_decorator.py` & `deephyper-0.7.0/deephyper/evaluator/_decorator.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_distributed.py` & `deephyper-0.7.0/deephyper/evaluator/_distributed.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_encoder.py` & `deephyper-0.7.0/deephyper/evaluator/_encoder.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_evaluator.py` & `deephyper-0.7.0/deephyper/evaluator/_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Dict, List, Hashable
 
 import numpy as np
 from deephyper.evaluator._job import Job
 from deephyper.skopt.optimizer import OBJECTIVE_VALUE_FAILURE
 from deephyper.core.utils._timeout import terminate_on_timeout
 from deephyper.evaluator.storage import Storage, MemoryStorage
+from deephyper.core.exceptions import MaximumJobsSpawnReached
 
 EVALUATORS = {
     "mpicomm": "_mpi_comm.MPICommEvaluator",
     "process": "_process_pool.ProcessPoolEvaluator",
     "ray": "_ray.RayEvaluator",
     "serial": "_serial.SerialEvaluator",
     "thread": "_thread_pool.ThreadPoolEvaluator",
@@ -89,14 +90,16 @@
         self._tasks_done = []  # Temp list to hold completed tasks from asyncio.
         self._tasks_pending = []  # Temp list to hold pending tasks from asyncio.
         self.jobs_done = []  # List used to store all jobs completed by the evaluator.
         self.job_id_gathered = []  # List of jobs'id gathered by the evaluator.
         self.timestamp = (
             time.time()
         )  # Recorded time of when this evaluator interface was created.
+        self.max_num_jobs_spawn = -1  # Maximum number of jobs to spawn.
+        self.num_jobs_spawn_counter = 0  # Counter of jobs spawned.
         self.loop = None  # Event loop for asyncio.
         self._start_dumping = False
         self._columns_dumped = None  # columns names dumped in csv file
         self.num_objective = None  # record if multi-objective are recorded
         self._stopper = None  # stopper object
 
         self._callbacks = [] if callbacks is None else callbacks
@@ -141,14 +144,18 @@
 
     def set_timeout(self, timeout):
         """Set a timeout for the Evaluator. It will create task with a "time budget" and will kill the the task if this budget
         is exhausted."""
         self._time_timeout_set = time.time()
         self._timeout = timeout
 
+    def set_max_num_jobs_spawn(self, max_num_jobs_spawn: int):
+        self.max_num_jobs_spawn = max_num_jobs_spawn
+        self.num_jobs_spawn_counter = 0
+
     def to_json(self):
         """Returns a json version of the evaluator."""
         out = {"type": type(self).__name__, "num_workers": self.num_workers}
         return out
 
     @staticmethod
     def create(run_function, method="serial", method_kwargs={}):
@@ -206,14 +213,24 @@
             while len(self._tasks_done) < n:
                 self._tasks_done, self._tasks_pending = await asyncio.wait(
                     self._tasks_running, return_when="FIRST_COMPLETED"
                 )
 
     async def _run_jobs(self, configs):
         for config in configs:
+
+            if (
+                self.max_num_jobs_spawn > 0
+                and self.num_jobs_spawn_counter >= self.max_num_jobs_spawn
+            ):
+                logging.info(
+                    f"Maximum number of jobs to spawn reached ({self.max_num_jobs_spawn})"
+                )
+                raise MaximumJobsSpawnReached
+
             # Create a Job object from the input configuration
             job_id = self._storage.create_new_job(self._search_id)
             self._storage.store_job_in(job_id, args=(config,))
             new_job = Job(job_id, config, self.run_function)
 
             if self._timeout:
                 time_consumed = time.time() - self._time_timeout_set
@@ -235,14 +252,16 @@
 
         job.output["metadata"]["timestamp_submit"] = time.time() - self.timestamp
 
         # call callbacks
         for cb in self._callbacks:
             cb.on_launch(job)
 
+        self.num_jobs_spawn_counter += 1
+
     def _on_done(self, job):
         """Called after a job has completed."""
         job.status = job.DONE
 
         job.output["metadata"]["timestamp_gather"] = time.time() - self.timestamp
 
         if np.isscalar(job.objective):
@@ -449,20 +468,33 @@
 
             resultsList.append(result)
 
         self.jobs_done = []
 
         if len(resultsList) != 0:
             mode = "a" if self._start_dumping else "w"
+
             with open(os.path.join(log_dir, filename), mode) as fp:
                 if not (self._start_dumping):
-                    self._columns_dumped = resultsList[0].keys()
-
-                writer = csv.DictWriter(fp, self._columns_dumped, extrasaction="ignore")
+                    # Waiting to start receiving non-failed jobs before dumping results
+                    for result in resultsList:
+                        if (
+                            "objective" in result
+                            and type(result["objective"]) is not str
+                        ) or (
+                            "objective_0" in result
+                            and type(result["objective_0"]) is not str
+                        ):
+                            self._columns_dumped = result.keys()
+
+                if self._columns_dumped is not None:
+                    writer = csv.DictWriter(
+                        fp, self._columns_dumped, extrasaction="ignore"
+                    )
 
-                if not (self._start_dumping):
-                    writer.writeheader()
-                    self._start_dumping = True
+                    if not (self._start_dumping):
+                        writer.writeheader()
+                        self._start_dumping = True
 
-                writer.writerows(resultsList)
+                    writer.writerows(resultsList)
 
         logging.info("dump_evals done")
```

### Comparing `deephyper-0.6.0/deephyper/evaluator/_job.py` & `deephyper-0.7.0/deephyper/evaluator/_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,18 @@
             return f"Job(id={self.id}, status={self.status}, config={self.config})"
 
     def __getitem__(self, index):
         cfg = copy.deepcopy(self.config)
         return (cfg, self.objective)[index]
 
     @property
+    def parameters(self):
+        return self.config
+
+    @property
     def result(self):
         """Alias for the objective property."""
         return self.objective
 
     @property
     def objective(self):
         """Objective returned by the run-function."""
```

### Comparing `deephyper-0.6.0/deephyper/evaluator/_mochi_process_pool.py` & `deephyper-0.7.0/deephyper/evaluator/_mochi_process_pool.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_mpi_comm.py` & `deephyper-0.7.0/deephyper/evaluator/_mpi_comm.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,20 @@
         self.root = root
         self.abort_on_exit = abort_on_exit
         self.wait_on_exit = wait_on_exit
         self.cancel_jobs_on_exit = cancel_jobs_on_exit
         self.num_workers = self.comm.Get_size() - 1  # 1 rank is the master
         self.sem = asyncio.Semaphore(self.num_workers)
         logging.info(f"Creating MPICommExecutor with {self.num_workers} max_workers...")
+
+        if self.num_workers == 0 and self.comm.Get_size() <= 1:
+            raise RuntimeError(
+                "No workers was detected because there was only 1 MPI rank. The number of MPI ranks must be greater than 1."
+            )
+
         self.executor = MPICommExecutor(comm=self.comm, root=self.root)
         self.master_executor = None
         logging.info("Creation of MPICommExecutor done")
 
     def __enter__(self):
         self.master_executor = self.executor.__enter__()
         if self.master_executor is not None:
```

### Comparing `deephyper-0.6.0/deephyper/evaluator/_nest_asyncio.py` & `deephyper-0.7.0/deephyper/evaluator/_nest_asyncio.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_process_pool.py` & `deephyper-0.7.0/deephyper/evaluator/_process_pool.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_queued.py` & `deephyper-0.7.0/deephyper/evaluator/_queued.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_ray.py` & `deephyper-0.7.0/deephyper/evaluator/_ray.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_run_function_utils.py` & `deephyper-0.7.0/deephyper/evaluator/_run_function_utils.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_serial.py` & `deephyper-0.7.0/deephyper/evaluator/_serial.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/_thread_pool.py` & `deephyper-0.7.0/deephyper/evaluator/_thread_pool.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/callback.py` & `deephyper-0.7.0/deephyper/evaluator/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,40 +177,60 @@
 
 class SearchEarlyStopping(Callback):
     """Stop the search gracefully when it does not improve for a given number of evaluations.
 
     Args:
         patience (int, optional): The number of not improving evaluations to wait for before stopping the search. Defaults to 10.
         objective_func (callable, optional): A function that takes a ``Job`` has input and returns the maximized scalar value monitored by this callback. Defaults to ``lambda j: j.result``.
+        threshold (float, optional): The threshold to reach before activating the patience to stop the search. Defaults to ``None``, patience is reinitialized after each improving observation.
+        verbose (bool, optional): Activation or deactivate the verbose mode. Defaults to ``True``.
     """
 
-    def __init__(self, patience: int = 10, objective_func=lambda j: j.result):
+    def __init__(
+        self,
+        patience: int = 10,
+        objective_func=lambda j: j.result,
+        threshold: float = None,
+        verbose: bool = 1,
+    ):
         self._best_objective = None
         self._n_lower = 0
         self._patience = patience
         self._objective_func = objective_func
+        self._threshold = threshold
+        self._verbose = verbose
 
     def on_done_other(self, job):
         self.on_done(job)
 
     def on_done(self, job):
         job_objective = self._objective_func(job)
         # if multi objectives are received
         if np.ndim(job_objective) > 0:
             job_objective = np.sum(job_objective)
         if self._best_objective is None:
             self._best_objective = job_objective
         else:
             if job_objective > self._best_objective:
-                print(
-                    f"Objective has improved from {self._best_objective:.5f} -> {job_objective:.5f}"
-                )
+                if self._verbose:
+                    print(
+                        f"Objective has improved from {self._best_objective:.5f} -> {job_objective:.5f}"
+                    )
                 self._best_objective = job_objective
                 self._n_lower = 0
             else:
                 self._n_lower += 1
 
         if self._n_lower >= self._patience:
-            print(
-                f"Stopping the search because it did not improve for the last {self._patience} evaluations!"
-            )
-            raise deephyper.core.exceptions.SearchTerminationError
+            if self._threshold is None:
+                if self._verbose:
+                    print(
+                        f"Stopping the search because it did not improve for the last {self._patience} evaluations!"
+                    )
+                raise deephyper.core.exceptions.SearchTerminationError
+            else:
+                if self._best_objective > self._threshold:
+                    if self._verbose:
+                        print(
+                            f"Stopping the search because it did not improve for the last {self._patience} evaluations!"
+                        )
+                    raise deephyper.core.exceptions.SearchTerminationError
```

### Comparing `deephyper-0.6.0/deephyper/evaluator/storage/__init__.py` & `deephyper-0.7.0/deephyper/evaluator/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/storage/_memory_storage.py` & `deephyper-0.7.0/deephyper/evaluator/storage/_memory_storage.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/storage/_ray_storage.py` & `deephyper-0.7.0/deephyper/evaluator/storage/_ray_storage.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/storage/_redis_storage.py` & `deephyper-0.7.0/deephyper/evaluator/storage/_redis_storage.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/evaluator/storage/_storage.py` & `deephyper-0.7.0/deephyper/evaluator/storage/_storage.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/callbacks/__init__.py` & `deephyper-0.7.0/deephyper/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/callbacks/csv_extended_logger.py` & `deephyper-0.7.0/deephyper/keras/callbacks/csv_extended_logger.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/callbacks/learning_rate_warmup.py` & `deephyper-0.7.0/deephyper/keras/callbacks/learning_rate_warmup.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/callbacks/stop_if_unfeasible.py` & `deephyper-0.7.0/deephyper/keras/callbacks/stop_if_unfeasible.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/callbacks/stop_on_timeout.py` & `deephyper-0.7.0/deephyper/keras/callbacks/stop_on_timeout.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/callbacks/time_stopping.py` & `deephyper-0.7.0/deephyper/keras/callbacks/time_stopping.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/callbacks/utils.py` & `deephyper-0.7.0/deephyper/keras/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/layers/__init__.py` & `deephyper-0.7.0/deephyper/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/layers/_mpnn.py` & `deephyper-0.7.0/deephyper/keras/layers/_mpnn.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/keras/layers/_padding.py` & `deephyper-0.7.0/deephyper/keras/layers/_padding.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/__init__.py` & `deephyper-0.7.0/deephyper/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/_keras_search_space.py` & `deephyper-0.7.0/deephyper/nas/_keras_search_space.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/_nx_search_space.py` & `deephyper-0.7.0/deephyper/nas/_nx_search_space.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/losses.py` & `deephyper-0.7.0/deephyper/nas/losses.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/metrics.py` & `deephyper-0.7.0/deephyper/nas/metrics.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/node.py` & `deephyper-0.7.0/deephyper/nas/node.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/operation/_base.py` & `deephyper-0.7.0/deephyper/nas/operation/_base.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/operation/_merge.py` & `deephyper-0.7.0/deephyper/nas/operation/_merge.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/preprocessing/_base.py` & `deephyper-0.7.0/deephyper/nas/preprocessing/_base.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/__init__.py` & `deephyper-0.7.0/deephyper/nas/run/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_run_base_trainer.py` & `deephyper-0.7.0/deephyper/nas/run/_run_base_trainer.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_run_debug.py` & `deephyper-0.7.0/deephyper/nas/run/_run_debug.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_run_debug_hp_arch.py` & `deephyper-0.7.0/deephyper/nas/run/_run_debug_hp_arch.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_run_debug_slow.py` & `deephyper-0.7.0/deephyper/nas/run/_run_debug_slow.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_run_distributed_base_trainer.py` & `deephyper-0.7.0/deephyper/nas/run/_run_distributed_base_trainer.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_run_horovod.py` & `deephyper-0.7.0/deephyper/nas/run/_run_horovod.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_test_horovod.py` & `deephyper-0.7.0/deephyper/nas/run/_test_horovod.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/run/_util.py` & `deephyper-0.7.0/deephyper/nas/run/_util.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/spacelib/tabular/dense_skipco.py` & `deephyper-0.7.0/deephyper/nas/spacelib/tabular/dense_skipco.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/spacelib/tabular/feed_forward.py` & `deephyper-0.7.0/deephyper/nas/spacelib/tabular/feed_forward.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/spacelib/tabular/one_layer.py` & `deephyper-0.7.0/deephyper/nas/spacelib/tabular/one_layer.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/spacelib/tabular/supervised_reg_auto_encoder.py` & `deephyper-0.7.0/deephyper/nas/spacelib/tabular/supervised_reg_auto_encoder.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/trainer/_arch.py` & `deephyper-0.7.0/deephyper/nas/trainer/_arch.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/trainer/_base.py` & `deephyper-0.7.0/deephyper/nas/trainer/_base.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/trainer/_horovod.py` & `deephyper-0.7.0/deephyper/nas/trainer/_horovod.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/nas/trainer/_utils.py` & `deephyper-0.7.0/deephyper/nas/trainer/_utils.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/problem/__init__.py` & `deephyper-0.7.0/deephyper/problem/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/problem/_hyperparameter.py` & `deephyper-0.7.0/deephyper/problem/_hyperparameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ConfigSpace.read_and_write import json as cs_json
 
 import deephyper.core.exceptions as dh_exceptions
 import deephyper.skopt
 
 
 def convert_to_skopt_dim(cs_hp, surrogate_model=None):
-    if surrogate_model in ["RF", "ET", "GBRT"]:
+    if surrogate_model in ["RF", "ET", "GBRT", "HGBRT", "MF", "BT"]:
         # models not sensitive to the metric space such as trees
         surrogate_model_type = "rule_based"
     else:
         # models sensitive to the metric space such as GP, neural networks
         surrogate_model_type = "distance_based"
 
     if isinstance(cs_hp, csh.UniformIntegerHyperparameter):
@@ -48,14 +48,19 @@
         ):
             transform = "identity"
         else:
             transform = "label"
         skopt_dim = deephyper.skopt.space.Categorical(
             categories=categories, name=cs_hp.name, transform=transform
         )
+    elif isinstance(cs_hp, csh.Constant):
+        categories = [cs_hp.value]
+        skopt_dim = deephyper.skopt.space.Categorical(
+            categories=categories, name=cs_hp.name, transform="label"
+        )
     else:
         raise TypeError(f"Cannot convert hyperparameter of type {type(cs_hp)}")
 
     return skopt_dim
 
 
 def convert_to_skopt_space(cs_space, surrogate_model=None):
@@ -63,37 +68,35 @@
 
     Args:
         cs_space (ConfigurationSpace): the ``ConfigurationSpace`` to convert.
         surrogate_model (str, optional): the type of surrogate model/base estimator used to perform Bayesian optimization. Defaults to None.
 
     Raises:
         TypeError: if the input space is not a ConfigurationSpace.
-        RuntimeError: if the input space contains forbiddens.
-        RuntimeError: if the input space contains conditions
 
     Returns:
         deephyper.skopt.space.Space: a scikit-optimize Space.
     """
 
     # verify pre-conditions
     if not (isinstance(cs_space, cs.ConfigurationSpace)):
         raise TypeError("Input space should be of type ConfigurationSpace")
 
-    if len(cs_space.get_conditions()) > 0:
-        raise RuntimeError("Cannot convert a ConfigSpace with Conditions!")
-
-    if len(cs_space.get_forbiddens()) > 0:
-        raise RuntimeError("Cannot convert a ConfigSpace with Forbiddens!")
+    sample_with_config_space = (
+        len(cs_space.get_conditions()) > 0 or len(cs_space.get_forbiddens()) > 0
+    )
 
     # convert the ConfigSpace to deephyper.skopt.space.Space
     dimensions = []
     for hp in cs_space.get_hyperparameters():
         dimensions.append(convert_to_skopt_dim(hp, surrogate_model))
 
-    skopt_space = deephyper.skopt.space.Space(dimensions)
+    skopt_space = deephyper.skopt.space.Space(
+        dimensions, config_space=cs_space if sample_with_config_space else None
+    )
     return skopt_space
 
 
 def check_hyperparameter(parameter, name=None, default_value=None):
     """Check if the passed parameter is a valid description of an hyperparameter.
 
     :meta private:
@@ -194,14 +197,17 @@
     def __str__(self):
         return repr(self)
 
     def __repr__(self):
         prob = repr(self._space)
         return prob
 
+    def __len__(self):
+        return len(self.hyperparameter_names)
+
     def add_hyperparameter(
         self, value, name: str = None, default_value=None
     ) -> csh.Hyperparameter:
         """Add an hyperparameter to the ``HpProblem``.
 
         Hyperparameters can be added to a ``HpProblem`` with a short syntax:
```

### Comparing `deephyper-0.6.0/deephyper/problem/_neuralarchitecture.py` & `deephyper-0.7.0/deephyper/problem/_neuralarchitecture.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/search/__init__.py` & `deephyper-0.7.0/deephyper/search/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/search/_search.py` & `deephyper-0.7.0/deephyper/search/_search.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import abc
 import copy
 import functools
 import logging
 import os
 import pathlib
+import time
 
 import numpy as np
 import pandas as pd
 import yaml
-from deephyper.core.exceptions import SearchTerminationError
+
+from deephyper.core.exceptions import MaximumJobsSpawnReached, SearchTerminationError
 from deephyper.core.utils._introspection import get_init_params_as_json
 from deephyper.core.utils._timeout import terminate_on_timeout
 from deephyper.evaluator import Evaluator
 from deephyper.evaluator.callback import TqdmCallback
 from deephyper.skopt.moo import non_dominated_set
 
 
@@ -45,14 +47,30 @@
         else:
             self._random_state = np.random.RandomState()
 
         # Create logging directory if does not exist
         self._log_dir = os.path.abspath(log_dir)
         pathlib.Path(log_dir).mkdir(parents=True, exist_ok=True)
 
+        self._path_results = os.path.join(self._log_dir, "results.csv")
+        if os.path.exists(self._path_results):
+            str_current_time = time.strftime("%Y%m%d-%H%M%S")
+            path_results_renamed = self._path_results.replace(
+                ".", f"_{str_current_time}."
+            )
+            logging.warning(
+                f"Results file already exists, it will be renamed to {path_results_renamed}"
+            )
+            os.rename(
+                self._path_results,
+                path_results_renamed,
+            )
+            evaluator._columns_dumped = None
+            evaluator._start_dumping = False
+
         self._verbose = verbose
 
         # if a callable is directly passed wrap it around the serial evaluator
         self.check_evaluator(evaluator)
 
     def check_evaluator(self, evaluator):
         if not (isinstance(evaluator, Evaluator)):
@@ -86,15 +104,19 @@
         """Dumps the context in the log folder."""
         context = self.to_json()
         path_context = os.path.join(self._log_dir, "context.yaml")
         with open(path_context, "w") as file:
             yaml.dump(context, file)
 
     def _set_timeout(self, timeout=None):
-        """If the `timeout` parameter is valid. Run the search in an other thread and trigger a timeout when this thread exhaust the allocated time budget."""
+        """If the `timeout` parameter is valid. Run the search in an other thread and trigger a timeout when this thread exhaust the allocated time budget.
+
+        Args:
+            timeout (int, optional): The time budget (in seconds) of the search before stopping. Defaults to ``None``, will not impose a time budget.
+        """
 
         if timeout is not None:
             if type(timeout) is not int:
                 raise ValueError(
                     f"'timeout' shoud be of type'int' but is of type '{type(timeout)}'!"
                 )
             if timeout <= 0:
@@ -102,58 +124,65 @@
 
         if np.isscalar(timeout) and timeout > 0:
             self._evaluator.set_timeout(timeout)
             self._search = functools.partial(
                 terminate_on_timeout, timeout, self._search
             )
 
-    def search(self, max_evals: int = -1, timeout: int = None):
+    def search(
+        self, max_evals: int = -1, timeout: int = None, max_evals_strict: bool = False
+    ):
         """Execute the search algorithm.
 
         Args:
             max_evals (int, optional): The maximum number of evaluations of the run function to perform before stopping the search. Defaults to ``-1``, will run indefinitely.
             timeout (int, optional): The time budget (in seconds) of the search before stopping. Defaults to ``None``, will not impose a time budget.
+            max_evals_strict (bool, optional): If ``True`` the search will not spawn more than ``max_evals`` jobs. Defaults to ``False``.
 
         Returns:
             DataFrame: a pandas DataFrame containing the evaluations performed or ``None`` if the search could not evaluate any configuration.
         """
-
         self._set_timeout(timeout)
+        if max_evals_strict:
+            self._evaluator.set_max_num_jobs_spawn(max_evals)
 
         # save the search call arguments for the context
         self._call_args.append({"timeout": timeout, "max_evals": max_evals})
         # save the context in the log folder
         self.dump_context()
         # init tqdm callback
         if max_evals > 1:
             for cb in self._evaluator._callbacks:
                 if isinstance(cb, TqdmCallback):
                     cb.set_max_evals(max_evals)
 
         try:
             self._search(max_evals, timeout)
-        except SearchTerminationError:
+        except SearchTerminationError as exc:
+            # Collect remaining jobs
+            if max_evals_strict and isinstance(exc, MaximumJobsSpawnReached):
+                self._evaluator.gather("ALL")
+
             if "saved_keys" in dir(self):
                 self._evaluator.dump_evals(saved_keys=self.saved_keys)
             else:
                 self._evaluator.dump_evals(log_dir=self._log_dir)
 
-        path_results = os.path.join(self._log_dir, "results.csv")
-        if not (os.path.exists(path_results)):
-            logging.warning(f"Could not find results file at {path_results}!")
+        if not (os.path.exists(self._path_results)):
+            logging.warning(f"Could not find results file at {self._path_results}!")
             return None
 
-        self.extend_results_with_pareto_efficient(path_results)
+        self.extend_results_with_pareto_efficient(self._path_results)
 
-        df_results = pd.read_csv(path_results)
+        df_results = pd.read_csv(self._path_results)
 
         return df_results
 
     @abc.abstractmethod
-    def _search(self, max_evals, timeout):
+    def _search(self, max_evals, timeout, max_evals_strict=False):
         """Search algorithm to be implemented.
 
         Args:
             max_evals (int, optional): The maximum number of evaluations of the run function to perform before stopping the search. Defaults to -1, will run indefinitely.
             timeout (int, optional): The time budget of the search before stopping.Defaults to None, will not impose a time budget.
         """
```

### Comparing `deephyper-0.6.0/deephyper/search/hps/_cbo.py` & `deephyper-0.7.0/deephyper/search/hps/_cbo.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,31 +15,64 @@
 from deephyper.search._search import Search
 from deephyper.skopt.moo import (
     non_dominated_set,
     non_dominated_set_ranked,
     MoScalarFunction,
     moo_functions,
 )
-
-from sklearn.ensemble import GradientBoostingRegressor
 from sklearn.base import is_regressor
 from deephyper.skopt.utils import use_named_args
 
 # Adapt minimization -> maximization with DeepHyper
 MAP_multi_point_strategy = {"cl_min": "cl_max", "cl_max": "cl_min", "qUCB": "qLCB"}
 
-MAP_acq_func = {"UCB": "LCB", "qUCB": "qLCB"}
+# TODO: check if qUCB is still valid
+MAP_acq_func = {"UCB": "LCB", "UCBd": "LCBd"}
 
 MAP_filter_failures = {"min": "max"}
 
 
 # schedulers
-def scheduler_periodic_exponential_decay(i, eta_0, periode, rate, delay):
-    """Periodic exponential decay scheduler for exploration-exploitation."""
-    eta_i = eta_0 * np.exp(-rate * ((i - 1 - delay) % periode))
+def scheduler_periodic_exponential_decay(i, eta_0, num_dim, period, rate, delay):
+    """Periodic exponential decay scheduler for exploration-exploitation.
+
+    Args:
+        i (int): current iteration.
+        eta_0 (float): initial value of the parameters ``[kappa, xi]`` to decay.
+        num_dim (int): number of dimensions of the search space.
+        period (int): period of the decay.
+        rate (float): rate of the decay.
+        delay (int): delay of the decay (decaying starts after ``delay`` iterations).
+
+    Returns:
+        tuple: an iterable of length 2 with the updated values at iteration ``i`` for ``[kappa, xi]``.
+    """
+    eta_i = eta_0 * np.exp(-rate * ((i - 1 - delay) % period))
+    return eta_i
+
+
+def scheduler_bandit(i, eta_0, num_dim, delta=0.05, lamb=0.2, delay=0):
+    """Bandit scheduler for exploration-exploitation. Only valid for the UCB acquisition function.
+
+    Args:
+        i (int): current iteration.
+        eta_0 (float): initial value of the parameters ``[kappa, xi]`` to decay.
+        num_dim (int): number of dimensions of the search space.
+        delta (float): confidence level.
+        lamb (float): factor of the initial scheduler. Defaults to ``0.2``.
+        delay (int): delay of the scheduler (decaying starts after ``delay`` iterations).
+
+    Returns:
+        tuple: an iterable of length 2 with the updated values at iteration ``i`` for ``[kappa, xi]``.
+    """
+    i = np.maximum(i + 1 - delay, 1)
+    beta_i = 2 * np.log(num_dim * i**2 * np.pi**2 / (6 * delta)) * lamb
+    beta_i = np.sqrt(beta_i)
+    eta_i = eta_0[:]
+    eta_i[0] = beta_i
     return eta_i
 
 
 class CBO(Search):
     """Centralized Bayesian Optimisation Search, previously named as "Asynchronous Model-Based Search" (AMBS). It follows a manager-workers architecture where the manager runs the Bayesian optimization loop and workers execute parallel evaluations of the black-box function.
 
     Example Usage:
@@ -49,62 +82,65 @@
 
     Args:
         problem (HpProblem): Hyperparameter problem describing the search space to explore.
         evaluator (Evaluator): An ``Evaluator`` instance responsible of distributing the tasks.
         random_state (int, optional): Random seed. Defaults to ``None``.
         log_dir (str, optional): Log directory where search's results are saved. Defaults to ``"."``.
         verbose (int, optional): Indicate the verbosity level of the search. Defaults to ``0``.
-        surrogate_model (Union[str,sklearn.base.RegressorMixin], optional): Surrogate model used by the Bayesian optimization. Can be a value in ``["RF", "GP", "ET", "GBRT", "DUMMY"]`` or a sklearn regressor. ``"RF"`` is for Random-Forest which is the best compromise between speed and quality when performing a lot of parallel evaluations, i.e., reaching more than hundreds of evaluations. ``"GP"`` is for Gaussian-Process which is the best choice when maximizing the quality of iteration but quickly slow down when reaching hundreds of evaluations, also it does not support conditional search space. ``"ET"`` is for Extra-Tree, faster than random forest but with worse mean estimate and poor uncertainty quantification capabilities. ``"GBRT"`` is for Gradient-Boosting Regression Tree, it has better mean estimate than other tree-based method worse uncertainty quantification capabilities and slower than ``"RF"``. Defaults to ``"RF"``.
+        surrogate_model (Union[str,sklearn.base.RegressorMixin], optional): Surrogate model used by the Bayesian optimization. Can be a value in ``["RF", "GP", "ET", "MF", "GBRT", "DUMMY"]`` or a sklearn regressor. ``"ET"`` is for Extremely Randomized Trees which is the best compromise between speed and quality when performing a lot of parallel evaluations, i.e., reaching more than hundreds of evaluations. ``"GP"`` is for Gaussian-Process which is the best choice when maximizing the quality of iteration but quickly slow down when reaching hundreds of evaluations, also it does not support conditional search space. ``"RF"`` is for Random-Forest, slower than extremely randomized trees but with better mean estimate and worse epistemic uncertainty quantification capabilities. ``"GBRT"`` is for Gradient-Boosting Regression Tree, it has better mean estimate than other tree-based method worse uncertainty quantification capabilities and slower than ``"RF"``. Defaults to ``"ET"``.
         acq_func (str, optional): Acquisition function used by the Bayesian optimization. Can be a value in ``["UCB", "EI", "PI", "gp_hedge"]``. Defaults to ``"UCB"``.
-        acq_optimizer (str, optional): Method used to minimze the acquisition function. Can be a value in ``["sampling", "lbfgs"]``. Defaults to ``"auto"``.
+        acq_optimizer (str, optional): Method used to minimze the acquisition function. Can be a value in ``["sampling", "lbfgs", "ga"]``. Defaults to ``"auto"``.
+        acq_optimizer_freq (int, optional): Frequency of optimization calls for the acquisition function. Defaults to ``10``, using optimizer every ``10`` surrogate model updates.
         kappa (float, optional): Manage the exploration/exploitation tradeoff for the "UCB" acquisition function. Defaults to ``1.96`` which corresponds to 95% of the confidence interval.
         xi (float, optional): Manage the exploration/exploitation tradeoff of ``"EI"`` and ``"PI"`` acquisition function. Defaults to ``0.001``.
         n_points (int, optional): The number of configurations sampled from the search space to infer each batch of new evaluated configurations.
         filter_duplicated (bool, optional): Force the optimizer to sample unique points until the search space is "exhausted" in the sens that no new unique points can be found given the sampling size ``n_points``. Defaults to ``True``.
         update_prior (bool, optional): Update the prior of the surrogate model with the new evaluated points. Defaults to ``False``. Should be set to ``True`` when all objectives and parameters are continuous.
         update_prior_quantile (float, optional): The quantile used to update the prior. Defaults to ``0.1``.
         multi_point_strategy (str, optional): Definition of the constant value use for the Liar strategy. Can be a value in ``["cl_min", "cl_mean", "cl_max", "qUCB"]``. All ``"cl_..."`` strategies follow the constant-liar scheme, where if $N$ new points are requested, the surrogate model is re-fitted $N-1$ times with lies (respectively, the minimum, mean and maximum objective found so far; for multiple objectives, these are the minimum, mean and maximum of the individual objectives) to infer the acquisition function. Constant-Liar strategy have poor scalability because of this repeated re-fitting. The ``"qUCB"`` strategy is much more efficient by sampling a new $kappa$ value for each new requested point without re-fitting the model, but it is only compatible with ``acq_func == "UCB"``. Defaults to ``"cl_max"``.
         n_jobs (int, optional): Number of parallel processes used to fit the surrogate model of the Bayesian optimization. A value of ``-1`` will use all available cores. Not used in ``surrogate_model`` if passed as own sklearn regressor. Defaults to ``1``.
         n_initial_points (int, optional): Number of collected objectives required before fitting the surrogate-model. Defaults to ``10``.
         initial_point_generator (str, optional): Sets an initial points generator. Can be either ``["random", "sobol", "halton", "hammersly", "lhs", "grid"]``. Defaults to ``"random"``.
         initial_points (List[Dict], optional): A list of initial points to evaluate where each point is a dictionnary where keys are names of hyperparameters and values their corresponding choice. Defaults to ``None`` for them to be generated randomly from the search space.
         sync_communcation (bool, optional): Performs the search in a batch-synchronous manner. Defaults to ``False`` for asynchronous updates.
-        filter_failures (str, optional): Replace objective of failed configurations by ``"min"`` or ``"mean"``. If ``"ignore"`` is passed then failed configurations will be filtered-out and not passed to the surrogate model. For multiple objectives, failure of any single objective will lead to treating that configuration as failed and each of these multiple objective will be replaced by their individual ``"min"`` or ``"mean"`` of past configurations. Defaults to ``"mean"`` to replace by failed configurations by the running mean of objectives.
+        filter_failures (str, optional): Replace objective of failed configurations by ``"min"`` or ``"mean"``. If ``"ignore"`` is passed then failed configurations will be filtered-out and not passed to the surrogate model. For multiple objectives, failure of any single objective will lead to treating that configuration as failed and each of these multiple objective will be replaced by their individual ``"min"`` or ``"mean"`` of past configurations. Defaults to ``"min"`` to replace failed configurations objectives by the running min of all objectives.
         max_failures (int, optional): Maximum number of failed configurations allowed before observing a valid objective value when ``filter_failures`` is not equal to ``"ignore"``. Defaults to ``100``.
         moo_lower_bounds (list, optional): List of lower bounds on the interesting range of objective values. Must be the same length as the number of obejctives. Defaults to ``None``, i.e., no bounds. Can bound only a single objective by providing ``None`` for all other values. For example, ``moo_lower_bounds=[None, 0.5, None]`` will explore all tradeoffs for the objectives at index 0 and 2, but only consider scores for objective 1 that exceed 0.5.
         moo_scalarization_strategy (str, optional): Scalarization strategy used in multiobjective optimization. Can be a value in ``["Linear", "Chebyshev", "AugChebyshev", "PBI", "Quadratic"]``. Defaults to ``"Chebyshev"``. Typically, randomized methods should be used to capture entire Pareto front, unless there is a known target solution a priori. Additional details on each scalarization can be found in :mod:`deephyper.skopt.moo`.
         moo_scalarization_weight (list, optional): Scalarization weights to be used in multiobjective optimization with length equal to the number of objective functions. Defaults to ``None`` for randomized weights. Only set if you want to fix the scalarization weights for a multiobjective HPS.
-        scheduler (dict, callable, optional): a method to manage the the value of ``kappa, xi`` with iterations. Defaults to ``None`` which does not use any scheduler.
+        scheduler (dict, callable, optional): a function to manage the value of ``kappa, xi`` with iterations. Defaults to ``None`` which does not use any scheduler. The periodic exponential decay scheduler can be used with  ``scheduler={"type": "periodic-exp-decay", "period": 30, "rate": 0.1}``. The scheduler can also be a callable function with signature ``scheduler(i, eta_0, **kwargs)`` where ``i`` is the current iteration, ``eta_0`` is the initial value of ``[kappa, xi]`` and ``kwargs`` are other fixed parameters of the function. Instead of fixing the decay ``"rate"`` the final ``kappa`` or ``xi` can be used ``{"type": "periodic-exp-decay", "period": 25, "kappa_final": 1.96}``.
         objective_scaler (str, optional): a way to map the objective space to some other support for example to normalize it. Defaults to ``"auto"`` which automatically set it to "identity" for any surrogate model except "RF" which will use "quantile-uniform".
         stopper (Stopper, optional): a stopper to leverage multi-fidelity when evaluating the function. Defaults to ``None`` which does not use any stopper.
     """
 
     def __init__(
         self,
         problem,
         evaluator,
         random_state: int = None,
         log_dir: str = ".",
         verbose: int = 0,
-        surrogate_model="RF",
-        acq_func: str = "UCB",
+        surrogate_model="ET",
+        surrogate_model_kwargs: dict = None,  # TODO: documentation
+        acq_func: str = "UCBd",
         acq_optimizer: str = "auto",
+        acq_optimizer_freq: int = 10,
         kappa: float = 1.96,
         xi: float = 0.001,
-        n_points: int = 10000,
+        n_points: int = 10_000,
         filter_duplicated: bool = True,
         update_prior: bool = False,
         update_prior_quantile: float = 0.1,
         multi_point_strategy: str = "cl_max",
         n_jobs: int = 1,  # 32 is good for Theta
         n_initial_points: int = 10,
         initial_point_generator: str = "random",
         initial_points=None,
         sync_communication: bool = False,
-        filter_failures: str = "mean",
+        filter_failures: str = "min",
         max_failures: int = 100,
         moo_lower_bounds=None,
         moo_scalarization_strategy: str = "Chebyshev",
         moo_scalarization_weight=None,
         scheduler=None,
         objective_scaler="auto",
         stopper=None,
@@ -114,29 +150,55 @@
         # get the __init__ parameters
         self._init_params = locals()
 
         # check input parameters
         if not (type(n_jobs) is int):
             raise ValueError(f"Parameter n_jobs={n_jobs} should be an integer value!")
 
-        surrogate_model_allowed = ["RF", "ET", "GBRT", "DUMMY", "GP", "MF"]
+        surrogate_model_allowed = [
+            # Trees
+            "RF",
+            "ET",
+            "TB",
+            "RS",
+            "MF",
+            # Other models
+            "GBRT",
+            "GP",
+            "HGBRT",
+            # Random Search
+            "DUMMY",
+        ]
         if surrogate_model in surrogate_model_allowed:
             base_estimator = self._get_surrogate_model(
                 surrogate_model,
-                n_jobs,
+                n_jobs=n_jobs,
                 random_state=self._random_state.randint(0, 2**31),
+                surrogate_model_kwargs=surrogate_model_kwargs,
             )
         elif is_regressor(surrogate_model):
             base_estimator = surrogate_model
         else:
             raise ValueError(
                 f"Parameter 'surrogate_model={surrogate_model}' should have a value in {surrogate_model_allowed}, or be a sklearn regressor!"
             )
 
-        acq_func_allowed = ["UCB", "EI", "PI", "gp_hedge", "qUCB"]
+        acq_func_allowed = [
+            "UCB",
+            "EI",
+            "PI",
+            "MES",
+            "gp_hedge",
+            "qUCB",
+            "UCBd",
+            "EId",
+            "PId",
+            "MESd",
+            "gp_hedged",
+        ]
         if not (acq_func in acq_func_allowed):
             raise ValueError(
                 f"Parameter 'acq_func={acq_func}' should have a value in {acq_func_allowed}!"
             )
 
         if not (np.isscalar(kappa)):
             raise ValueError("Parameter 'kappa' should be a scalar value!")
@@ -212,25 +274,18 @@
                     )
 
         self._multi_point_strategy = MAP_multi_point_strategy.get(
             multi_point_strategy, multi_point_strategy
         )
         self._fitted = False
 
-        # check if it is possible to convert the ConfigSpace to standard skopt Space
-        if (
-            isinstance(self._problem.space, CS.ConfigurationSpace)
-            and len(self._problem.space.get_forbiddens()) == 0
-            and len(self._problem.space.get_conditions()) == 0
-        ):
-            self._opt_space = convert_to_skopt_space(
-                self._problem.space, surrogate_model=surrogate_model
-            )
-        else:
-            self._opt_space = self._problem.space
+        # Map the ConfigSpace to Skop Space
+        self._opt_space = convert_to_skopt_space(
+            self._problem.space, surrogate_model=surrogate_model
+        )
 
         self._opt = None
         self._opt_kwargs = dict(
             dimensions=self._opt_space,
             base_estimator=base_estimator,
             # optimizer
             initial_point_generator=initial_point_generator,
@@ -241,15 +296,15 @@
                 "update_prior": update_prior,
                 "update_prior_quantile": 1 - update_prior_quantile,
                 "n_jobs": n_jobs,
                 "filter_failures": MAP_filter_failures.get(
                     filter_failures, filter_failures
                 ),
                 "max_failures": max_failures,
-                "boltzmann_gamma": 1,
+                "acq_optimizer_freq": acq_optimizer_freq,
             },
             # acquisition function
             acq_func=MAP_acq_func.get(acq_func, acq_func),
             acq_func_kwargs={"xi": xi, "kappa": kappa},
             n_initial_points=self._n_initial_points,
             initial_points=self._initial_points,
             random_state=self._random_state,
@@ -257,37 +312,67 @@
             moo_scalarization_strategy=self._moo_scalarization_strategy,
             moo_scalarization_weight=self._moo_scalarization_weight,
             objective_scaler=objective_scaler,
         )
 
         self._gather_type = "ALL" if sync_communication else "BATCH"
 
-        # scheduler policy
+        # Scheduler policy
+        scheduler = {"type": "bandit"} if scheduler is None else scheduler
         self.scheduler = None
         if type(scheduler) is dict:
             scheduler = scheduler.copy()
             scheduler_type = scheduler.pop("type", None)
-            assert scheduler_type in ["periodic-exp-decay"]
+            assert scheduler_type in ["periodic-exp-decay", "bandit"]
 
             if scheduler_type == "periodic-exp-decay":
+                rate = scheduler.get("rate", None)
+                period = scheduler.get("period", None)
+
+                # Automatically retrieve the "decay rate" of the scheduler by solving
+                # the equation: eta_0 * exp(-rate * period) = eta_final
+                if rate is None:
+                    if "UCB" in acq_func:
+                        kappa_final = scheduler.pop("kappa_final", 0.1)
+                        rate = -1 / period * np.log(kappa_final / kappa)
+                    elif "EI" in acq_func or "PI" in acq_func:
+                        xi_final = scheduler.pop("xi_final", 0.0001)
+                        rate = -1 / period * np.log(xi_final / xi)
+                    else:
+                        rate = 0.1
+
                 scheduler_params = {
-                    "periode": 25,
-                    "rate": 0.1,
+                    "period": period,
+                    "rate": rate,
                     "delay": n_initial_points,
                 }
                 scheduler_func = scheduler_periodic_exponential_decay
 
+            elif scheduler_type == "bandit":
+                scheduler_params = {
+                    "delta": 0.05,
+                    "lamb": 0.2,
+                    "delay": n_initial_points,
+                }
+                scheduler_func = scheduler_bandit
+
             scheduler_params.update(scheduler)
             eta_0 = np.array([kappa, xi])
             self.scheduler = functools.partial(
-                scheduler_func, eta_0=eta_0, **scheduler_params
+                scheduler_func,
+                eta_0=eta_0,
+                num_dim=len(self._problem),
+                **scheduler_params,
             )
             logging.info(
                 f"Set up scheduler '{scheduler_type}' with parameters '{scheduler_params}'"
             )
+        elif callable(scheduler):
+            self.scheduler = functools.partial(scheduler, eta_0=np.array([kappa, xi]))
+            logging.info(f"Set up scheduler '{scheduler}'")
 
         # stopper
         self._evaluator._stopper = stopper
 
     def _setup_optimizer(self):
         if self._fitted:
             self._opt_kwargs["n_initial_points"] = 0
@@ -446,62 +531,148 @@
                 # submit new configurations
                 logging.info(f"Submitting {len(new_batch)} configurations...")
                 t1 = time.time()
                 self._evaluator.submit(new_batch)
                 logging.info(f"Submition took {time.time() - t1:.4f} sec.")
 
     def _get_surrogate_model(
-        self, name: str, n_jobs: int = None, random_state: int = None
+        self,
+        name: str,
+        n_jobs: int = 1,
+        random_state: int = None,
+        surrogate_model_kwargs: dict = None,
     ):
         """Get a surrogate model from Scikit-Optimize.
 
         Args:
             name (str): name of the surrogate model.
             n_jobs (int): number of parallel processes to distribute the computation of the surrogate model.
+            random_state (int): random seed.
+            surrogate_model_kwargs (dict): additional parameters to pass to the surrogate model.
+
+        Returns:
+            sklearn.base.RegressorMixin: a surrogate model capabable of predicting y_mean and y_std.
 
         Raises:
             ValueError: when the name of the surrogate model is unknown.
         """
-        accepted_names = ["RF", "ET", "GBRT", "DUMMY", "GP", "MF"]
+
+        # Check if the surrogate model is supported
+        accepted_names = ["RF", "ET", "TB", "RS", "GBRT", "DUMMY", "GP", "MF", "HGBRT"]
         if not (name in accepted_names):
             raise ValueError(
                 f"Unknown surrogate model {name}, please choose among {accepted_names}."
             )
 
-        if name == "RF":
-            # TODO: for better performance the RF surrogate could be fit with a bootstrap sample of size max 1_000
-            # However this should be refreshed each time when creating the estimator
-            surrogate = deephyper.skopt.learning.RandomForestRegressor(
-                # n_estimators=100,
-                # max_features=1,
-                # min_samples_leaf=3,
+        if surrogate_model_kwargs is None:
+            surrogate_model_kwargs = {}
+
+        # Define default surrogate model parameters
+        if name in ["RF", "ET", "TB", "RS", "MF"]:
+            default_surrogate_model_kwargs = dict(
+                n_estimators=100,
+                max_samples=0.8,
+                min_samples_split=2,  # Aleatoric Variance will be 0
                 n_jobs=n_jobs,
                 random_state=random_state,
             )
-        elif name == "ET":
-            surrogate = deephyper.skopt.learning.ExtraTreesRegressor(
-                # n_estimators=100,
-                # min_samples_leaf=3,
+
+            # From https://link.springer.com/article/10.1007/s10994-006-6226-1
+            # We follow parameters indicated at: p. 8, Sec. 2.2.2
+            # Model: Random Forest from L. Breiman
+            if name == "RF":
+                default_surrogate_model_kwargs["splitter"] = "best"
+                default_surrogate_model_kwargs["max_features"] = "sqrt"
+                default_surrogate_model_kwargs["bootstrap"] = True
+            # Model: Extremely Randomized Forest
+            elif name == "ET":
+                default_surrogate_model_kwargs["splitter"] = "random"
+                default_surrogate_model_kwargs["max_features"] = 1.0
+                default_surrogate_model_kwargs["bootstrap"] = False
+                default_surrogate_model_kwargs["max_samples"] = None
+            # Model: Tree Bagging
+            elif name == "TB":
+                default_surrogate_model_kwargs["bootstrap"] = True
+                default_surrogate_model_kwargs["splitter"] = "best"
+                default_surrogate_model_kwargs["max_features"] = 1.0
+            elif name == "RS":
+                default_surrogate_model_kwargs["splitter"] = "best"
+                default_surrogate_model_kwargs["bootstrap"] = False
+                default_surrogate_model_kwargs["max_samples"] = None
+                default_surrogate_model_kwargs["max_features"] = "sqrt"
+            elif name == "MF":
+                default_surrogate_model_kwargs["bootstrap"] = False
+                default_surrogate_model_kwargs["max_samples"] = None
+
+        elif name == "GBRT":
+            default_surrogate_model_kwargs = dict(
+                n_estimtaors=10,
                 n_jobs=n_jobs,
                 random_state=random_state,
             )
-        elif name == "GBRT":
-            gbrt = GradientBoostingRegressor(n_estimators=30, loss="quantile")
-            surrogate = deephyper.skopt.learning.GradientBoostingQuantileRegressor(
-                base_estimator=gbrt, n_jobs=n_jobs, random_state=random_state
+        elif name == "HGBRT":
+            default_surrogate_model_kwargs = dict(
+                n_jobs=n_jobs,
+                random_state=random_state,
+            )
+        else:
+            default_surrogate_model_kwargs = {}
+
+        default_surrogate_model_kwargs.update(surrogate_model_kwargs)
+
+        if name in ["RF", "TB", "RS", "ET"]:
+            surrogate = deephyper.skopt.learning.RandomForestRegressor(
+                **default_surrogate_model_kwargs,
             )
+
+        # Model: Mondrian Forest
         elif name == "MF":
             try:
                 surrogate = deephyper.skopt.learning.MondrianForestRegressor(
-                    n_estimators=100, n_jobs=n_jobs, random_state=random_state
+                    **default_surrogate_model_kwargs,
                 )
             except AttributeError:
                 raise deephyper.core.exceptions.MissingRequirementError(
                     "Installing 'deephyper/scikit-garden' is required to use MondrianForest (MF) regressor as a surrogate model!"
                 )
+        # Model: Gradient Boosting Regression Tree (based on quantiles)
+        # https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingRegressor.html
+        elif name == "GBRT":
+            from sklearn.ensemble import GradientBoostingRegressor
+
+            gbrt = GradientBoostingRegressor(
+                n_estimators=default_surrogate_model_kwargs.pop("n_estimators"),
+                loss="quantile",
+            )
+            surrogate = deephyper.skopt.learning.GradientBoostingQuantileRegressor(
+                base_estimator=gbrt,
+                **default_surrogate_model_kwargs,
+            )
+        # Model: Histogram-based Gradient Boosting Regression Tree (based on quantiles)
+        # https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.HistGradientBoostingRegressor.html
+        elif name == "HGBRT":
+            from sklearn.ensemble import HistGradientBoostingRegressor
+
+            # Check wich parameters are categorical
+            categorical_features = []
+            for hp_name in self._problem.space:
+                hp = self._problem.space.get_hyperparameter(hp_name)
+
+                categorical_features.append(
+                    isinstance(hp, csh.CategoricalHyperparameter)
+                    # or isinstance(hp, csh.OrdinalHyperparameter)
+                )
+
+            gbrt = HistGradientBoostingRegressor(
+                loss="quantile", categorical_features=categorical_features
+            )
+            surrogate = deephyper.skopt.learning.GradientBoostingQuantileRegressor(
+                base_estimator=gbrt,
+                **default_surrogate_model_kwargs,
+            )
         else:  # for DUMMY and GP
             surrogate = name
 
         return surrogate
 
     def _return_cond(self, cond, cst_new):
         parent = cst_new.get_hyperparameter(cond.parent.name)
@@ -896,15 +1067,15 @@
     def __init__(
         self,
         problem,
         evaluator,
         random_state: int = None,
         log_dir: str = ".",
         verbose: int = 0,
-        surrogate_model="RF",
+        surrogate_model="ET",
         acq_func: str = "UCB",
         acq_optimizer: str = "auto",
         kappa: float = 1.96,
         xi: float = 0.001,
         n_points: int = 10000,
         filter_duplicated: bool = True,
         update_prior: bool = False,
```

### Comparing `deephyper-0.6.0/deephyper/search/hps/_mpi_dbo.py` & `deephyper-0.7.0/deephyper/search/hps/_mpi_dbo.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 
     Args:
         problem (HpProblem): Hyperparameter problem describing the search space to explore.
         evaluator (Evaluator): An ``Evaluator`` instance responsible of distributing the tasks.
         random_state (int, optional): Random seed. Defaults to ``None``.
         log_dir (str, optional): Log directory where search's results are saved. Defaults to ``"."``.
         verbose (int, optional): Indicate the verbosity level of the search. Defaults to ``0``.
-        surrogate_model (Union[str,sklearn.base.RegressorMixin], optional): Surrogate model used by the Bayesian optimization. Can be a value in ``["RF", "GP", "ET", "GBRT", "DUMMY"]`` or a sklearn regressor. ``"RF"`` is for Random-Forest which is the best compromise between speed and quality when performing a lot of parallel evaluations, i.e., reaching more than hundreds of evaluations. ``"GP"`` is for Gaussian-Process which is the best choice when maximizing the quality of iteration but quickly slow down when reaching hundreds of evaluations, also it does not support conditional search space. ``"ET"`` is for Extra-Tree, faster than random forest but with worse mean estimate and poor uncertainty quantification capabilities. ``"GBRT"`` is for Gradient-Boosting Regression Tree, it has better mean estimate than other tree-based method worse uncertainty quantification capabilities and slower than ``"RF"``. Defaults to ``"RF"``.
+        surrogate_model (Union[str,sklearn.base.RegressorMixin], optional): Surrogate model used by the Bayesian optimization. Can be a value in ``["RF", "GP", "ET", "MF", "GBRT", "DUMMY"]`` or a sklearn regressor. ``"ET"`` is for Extremely Randomized Trees which is the best compromise between speed and quality when performing a lot of parallel evaluations, i.e., reaching more than hundreds of evaluations. ``"GP"`` is for Gaussian-Process which is the best choice when maximizing the quality of iteration but quickly slow down when reaching hundreds of evaluations, also it does not support conditional search space. ``"RF"`` is for Random-Forest, slower than extremely randomized trees but with better mean estimate and worse epistemic uncertainty quantification capabilities. ``"GBRT"`` is for Gradient-Boosting Regression Tree, it has better mean estimate than other tree-based method worse uncertainty quantification capabilities and slower than ``"RF"``. Defaults to ``"ET"``.
         acq_func (str, optional): Acquisition function used by the Bayesian optimization. Can be a value in ``["UCB", "EI", "PI", "gp_hedge"]``. Defaults to ``"UCB"``.
         acq_optimizer (str, optional): Method used to minimze the acquisition function. Can be a value in ``["sampling", "lbfgs"]``. Defaults to ``"auto"``.
+        acq_optimizer_freq (int, optional): Frequency of optimization calls for the acquisition function. Defaults to ``10``, using optimizer every ``10`` surrogate model updates.
         kappa (float, optional): Manage the exploration/exploitation tradeoff for the "UCB" acquisition function. Defaults to ``1.96`` which corresponds to 95% of the confidence interval.
         xi (float, optional): Manage the exploration/exploitation tradeoff of ``"EI"`` and ``"PI"`` acquisition function. Defaults to ``0.001``.
         n_points (int, optional): The number of configurations sampled from the search space to infer each batch of new evaluated configurations.
         filter_duplicated (bool, optional): Force the optimizer to sample unique points until the search space is "exhausted" in the sens that no new unique points can be found given the sampling size ``n_points``. Defaults to ``True``.
         update_prior (bool, optional): Update the prior of the surrogate model with the new evaluated points. Defaults to ``False``. Should be set to ``True`` when all objectives and parameters are continuous.
         update_prior_quantile (float, optional): The quantile used to update the prior. Defaults to ``0.1``.
         multi_point_strategy (str, optional): Definition of the constant value use for the Liar strategy. Can be a value in ``["cl_min", "cl_mean", "cl_max", "qUCB"]``. All ``"cl_..."`` strategies follow the constant-liar scheme, where if $N$ new points are requested, the surrogate model is re-fitted $N-1$ times with lies (respectively, the minimum, mean and maximum objective found so far; for multiple objectives, these are the minimum, mean and maximum of the individual objectives) to infer the acquisition function. Constant-Liar strategy have poor scalability because of this repeated re-fitting. The ``"qUCB"`` strategy is much more efficient by sampling a new $kappa$ value for each new requested point without re-fitting the model, but it is only compatible with ``acq_func == "UCB"``. Defaults to ``"cl_max"``.
@@ -45,30 +46,31 @@
         initial_points (List[Dict], optional): A list of initial points to evaluate where each point is a dictionnary where keys are names of hyperparameters and values their corresponding choice. Defaults to ``None`` for them to be generated randomly from the search space.
         sync_communcation (bool, optional): Performs the search in a batch-synchronous manner. Defaults to ``False`` for asynchronous updates.
         filter_failures (str, optional): Replace objective of failed configurations by ``"min"`` or ``"mean"``. If ``"ignore"`` is passed then failed configurations will be filtered-out and not passed to the surrogate model. For multiple objectives, failure of any single objective will lead to treating that configuration as failed and each of these multiple objective will be replaced by their individual ``"min"`` or ``"mean"`` of past configurations. Defaults to ``"mean"`` to replace by failed configurations by the running mean of objectives.
         max_failures (int, optional): Maximum number of failed configurations allowed before observing a valid objective value when ``filter_failures`` is not equal to ``"ignore"``. Defaults to ``100``.
         moo_lower_bounds (list, optional): List of lower bounds on the interesting range of objective values. Must be the same length as the number of obejctives. Defaults to ``None``, i.e., no bounds. Can bound only a single objective by providing ``None`` for all other values. For example, ``moo_lower_bounds=[None, 0.5, None]`` will explore all tradeoffs for the objectives at index 0 and 2, but only consider scores for objective 1 that exceed 0.5.
         moo_scalarization_strategy (str, optional): Scalarization strategy used in multiobjective optimization. Can be a value in ``["Linear", "Chebyshev", "AugChebyshev", "PBI", "Quadratic"]``. Defaults to ``"Chebyshev"``. Typically, randomized methods should be used to capture entire Pareto front, unless there is a known target solution a priori. Additional details on each scalarization can be found in :mod:`deephyper.skopt.moo`.
         moo_scalarization_weight (list, optional): Scalarization weights to be used in multiobjective optimization with length equal to the number of objective functions. Defaults to ``None`` for randomized weights. Only set if you want to fix the scalarization weights for a multiobjective HPS.
-        scheduler (dict, callable, optional): a method to manage the the value of ``kappa, xi`` with iterations. Defaults to ``None`` which does not use any scheduler.
+        scheduler (dict, callable, optional): a function to manage the value of ``kappa, xi`` with iterations. Defaults to ``None`` which does not use any scheduler. The periodic exponential decay scheduler can be used with  ``scheduler={"type": "periodic-exp-decay", "period": 30, "rate": 0.1}``. The scheduler can also be a callable function with signature ``scheduler(i, eta_0, **kwargs)`` where ``i`` is the current iteration, ``eta_0`` is the initial value of ``[kappa, xi]`` and ``kwargs`` are other fixed parameters of the function.
         objective_scaler (str, optional): a way to map the objective space to some other support for example to normalize it. Defaults to ``"auto"`` which automatically set it to "identity" for any surrogate model except "RF" which will use "quantile-uniform".
         stopper (Stopper, optional): a stopper to leverage multi-fidelity when evaluating the function. Defaults to ``None`` which does not use any stopper.
         comm (Comm, optional): communicator used with MPI. Defaults to ``None`` for  ``COMM_WORLD``.
     """
 
     def __init__(
         self,
         problem,
         evaluator,
         random_state: int = None,
         log_dir: str = ".",
         verbose: int = 0,
-        surrogate_model="RF",
-        acq_func: str = "UCB",
+        surrogate_model="ET",
+        acq_func: str = "qUCBd",
         acq_optimizer: str = "auto",
+        acq_optimizer_freq: int = 10,
         kappa: float = 1.96,
         xi: float = 0.001,
         n_points: int = 10000,
         filter_duplicated: bool = True,
         update_prior: bool = False,
         update_prior_quantile: float = 0.1,
         multi_point_strategy: str = "cl_max",
@@ -103,29 +105,21 @@
         if type(random_state) is int:
             random_state = np.random.RandomState(random_state)
         elif isinstance(random_state, np.random.RandomState):
             random_state = random_state
         else:
             random_state = np.random.RandomState()
 
-        if acq_optimizer == "auto":
-            if acq_func[0] == "q":
-                acq_optimizer = "sampling"
-            elif acq_func[0] == "b":
-                acq_optimizer == "boltzmann_sampling"
-            else:
-                acq_optimizer = "sampling"
-
         if acq_func[0] == "q":
             kappa = scipy.stats.expon.rvs(
                 size=self.size, scale=kappa, random_state=random_state
-            )[self._evaluator.rank]
+            )[self.rank]
             xi = scipy.stats.expon.rvs(
                 size=self.size, scale=xi, random_state=random_state
-            )[self._evaluator.rank]
+            )[self.rank]
             acq_func = acq_func[1:]
         elif acq_func[0] == "b":
             acq_func[0] = acq_func[1:]
 
         # set random state for given rank
         random_state = np.random.RandomState(
             random_state.randint(low=0, high=2**31, size=self.size)[self.rank]
@@ -138,14 +132,15 @@
                 evaluator=evaluator,
                 random_state=random_state,
                 log_dir=log_dir,
                 verbose=verbose,
                 surrogate_model=surrogate_model,
                 acq_func=acq_func,
                 acq_optimizer=acq_optimizer,
+                acq_optimizer_freq=acq_optimizer_freq,
                 kappa=kappa,
                 xi=xi,
                 n_points=n_points,
                 filter_duplicated=filter_duplicated,
                 update_prior=update_prior,
                 update_prior_quantile=update_prior_quantile,
                 multi_point_strategy=multi_point_strategy,
@@ -171,14 +166,15 @@
                 evaluator=evaluator,
                 random_state=random_state,
                 log_dir=log_dir,
                 verbose=verbose,
                 surrogate_model=surrogate_model,
                 acq_func=acq_func,
                 acq_optimizer=acq_optimizer,
+                acq_optimizer_freq=acq_optimizer_freq,
                 kappa=kappa,
                 xi=xi,
                 n_points=n_points,
                 filter_duplicated=filter_duplicated,
                 update_prior=update_prior,
                 update_prior_quantile=update_prior_quantile,
                 multi_point_strategy=multi_point_strategy,
```

### Comparing `deephyper-0.6.0/deephyper/search/nas/__init__.py` & `deephyper-0.7.0/deephyper/search/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/search/nas/_agebo.py` & `deephyper-0.7.0/deephyper/search/nas/_agebo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import collections
 
-import deephyper.skopt
 import numpy as np
+
+import deephyper.skopt
+from deephyper.problem._hyperparameter import convert_to_skopt_space
 from deephyper.search.nas._regevo import RegularizedEvolution
 
 # Adapt minimization -> maximization with DeepHyper
 MAP_liar_strategy = {
     "cl_min": "cl_max",
     "cl_max": "cl_min",
 }
@@ -123,22 +125,28 @@
                         f"Initial points should be dict or list but {type(point)} was given!"
                     )
         self._liar_strategy = MAP_liar_strategy.get(liar_strategy, liar_strategy)
 
         base_estimator = self._get_surrogate_model(
             surrogate_model, n_jobs, random_state=self._random_state.randint(0, 2**31)
         )
+
+        # Map the ConfigSpace to Skop Space
+        self._hp_opt_space = convert_to_skopt_space(
+            self._problem._hp_space._space, surrogate_model=surrogate_model
+        )
+
         self._hp_opt = None
         self._hp_opt_kwargs = dict(
             acq_optimizer="sampling",
             acq_optimizer_kwargs={
                 "n_points": n_points,
                 "filter_duplicated": False,
             },
-            dimensions=self._problem._hp_space._space,
+            dimensions=self._hp_opt_space,
             base_estimator=base_estimator,
             acq_func=MAP_acq_func.get(acq_func, acq_func),
             acq_func_kwargs={"xi": xi, "kappa": kappa},
             n_initial_points=self._n_initial_points,
             initial_points=self._initial_points,
             random_state=self._random_state,
         )
@@ -210,14 +218,18 @@
                         children_batch.append(child)
 
                         # collect infos for hp optimization
                         new_i_hp_values = self._problem.extract_hp_values(
                             config=new_results[new_i][0]
                         )
                         new_i_y = new_results[new_i][1]
+
+                        if new_i_y == "F":
+                            new_i_y = -np.inf
+
                         hp_results_X.append(new_i_hp_values)
                         hp_results_y.append(-new_i_y)
 
                     self._hp_opt.tell(hp_results_X, hp_results_y)  # !fit: costly
                     new_hps = self._hp_opt.ask(
                         n_points=len(new_results), strategy=self._liar_strategy
                     )
```

### Comparing `deephyper-0.6.0/deephyper/search/nas/_ambsmixed.py` & `deephyper-0.7.0/deephyper/search/nas/_ambsmixed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 
 import ConfigSpace as CS
 import numpy as np
+
 import deephyper.skopt
 from deephyper.problem import HpProblem
+from deephyper.problem._hyperparameter import convert_to_skopt_space
 from deephyper.search.nas._base import NeuralArchitectureSearch
 
 # Adapt minimization -> maximization with DeepHyper
 MAP_liar_strategy = {
     "cl_min": "cl_max",
     "cl_max": "cl_min",
 }
@@ -106,17 +108,22 @@
         self._n_initial_points = self._evaluator.num_workers
         self._liar_strategy = MAP_liar_strategy.get(liar_strategy, liar_strategy)
 
         base_estimator = self._get_surrogate_model(
             surrogate_model, n_jobs, random_state=self._random_state.get_state()[1][0]
         )
 
+        # Map the ConfigSpace to Skop Space
+        self._hp_opt_space = convert_to_skopt_space(
+            self._problem._hp_space._space, surrogate_model=surrogate_model
+        )
+
         self._opt = None
         self._opt_kwargs = dict(
-            dimensions=self._space,
+            dimensions=self._hp_opt_space,
             base_estimator=base_estimator,
             acq_func=MAP_acq_func.get(acq_func, acq_func),
             acq_optimizer="sampling",
             acq_func_kwargs={"xi": xi, "kappa": kappa, "n_points": n_points},
             n_initial_points=self._n_initial_points,
             random_state=self._random_state,
         )
```

### Comparing `deephyper-0.6.0/deephyper/search/nas/_base.py` & `deephyper-0.7.0/deephyper/search/nas/_base.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/search/nas/_random.py` & `deephyper-0.7.0/deephyper/search/nas/_random.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/search/nas/_regevo.py` & `deephyper-0.7.0/deephyper/search/nas/_regevo.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/search/nas/_regevomixed.py` & `deephyper-0.7.0/deephyper/search/nas/_regevomixed.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/sklearn/classifier/_autosklearn1.py` & `deephyper-0.7.0/deephyper/sklearn/classifier/_autosklearn1.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/sklearn/regressor/_autosklearn1.py` & `deephyper-0.7.0/deephyper/sklearn/regressor/_autosklearn1.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/__init__.py` & `deephyper-0.7.0/deephyper/skopt/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/acquisition.py` & `deephyper-0.7.0/deephyper/skopt/acquisition.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import numpy as np
 import warnings
 
 from scipy.stats import norm
 
 
 def gaussian_acquisition_1D(
-    X, model, y_opt=None, acq_func="LCB", acq_func_kwargs=None, return_grad=True
+    X,
+    model,
+    y_opt=None,
+    acq_func="LCB",
+    acq_func_kwargs=None,
+    return_grad=True,
 ):
     """
     A wrapper around the acquisition function that is called by fmin_l_bfgs_b.
 
     This is because lbfgs allows only 1-D input.
     """
     return _gaussian_acquisition(
@@ -19,58 +24,75 @@
         acq_func=acq_func,
         acq_func_kwargs=acq_func_kwargs,
         return_grad=return_grad,
     )
 
 
 def _gaussian_acquisition(
-    X, model, y_opt=None, acq_func="LCB", return_grad=False, acq_func_kwargs=None
+    X,
+    model,
+    y_opt=None,
+    acq_func="LCB",
+    return_grad=False,
+    acq_func_kwargs=None,
 ):
     """
     Wrapper so that the output of this function can be
     directly passed to a minimizer.
     """
     # Check inputs
     X = np.asarray(X)
     if X.ndim != 2:
         raise ValueError(
             "X is {}-dimensional, however," " it must be 2-dimensional.".format(X.ndim)
         )
 
+    # Check if the deterministic acquisition function variant should be used
+    deterministic = False
+    if "d" == acq_func[-1]:
+        deterministic = True
+        acq_func = acq_func[:-1]
+
     if acq_func_kwargs is None:
         acq_func_kwargs = dict()
     xi = acq_func_kwargs.get("xi", 0.01)
     kappa = acq_func_kwargs.get("kappa", 1.96)
 
     # Evaluate acquisition function
     per_second = acq_func.endswith("ps")
     if per_second:
         model, time_model = model.estimators_
 
-    if acq_func == "LCB":
-        func_and_grad = gaussian_lcb(X, model, kappa, return_grad)
+    if acq_func in ["LCB"]:
+        func_and_grad = gaussian_lcb(
+            X, model, kappa, return_grad, deterministic=deterministic
+        )
+
         if return_grad:
             acq_vals, acq_grad = func_and_grad
         else:
             acq_vals = func_and_grad
 
     elif acq_func in ["EI", "PI", "EIps", "PIps"]:
         if acq_func in ["EI", "EIps"]:
-            func_and_grad = gaussian_ei(X, model, y_opt, xi, return_grad)
+            func_and_grad = gaussian_ei(
+                X, model, y_opt, xi, return_grad, deterministic=deterministic
+            )
         else:
-            func_and_grad = gaussian_pi(X, model, y_opt, xi, return_grad)
+            func_and_grad = gaussian_pi(
+                X, model, y_opt, xi, return_grad, deterministic=deterministic
+            )
 
         if return_grad:
             acq_vals = -func_and_grad[0]
             acq_grad = -func_and_grad[1]
         else:
             acq_vals = -func_and_grad
 
         if acq_func in ["EIps", "PIps"]:
-
             if return_grad:
                 mu, std, mu_grad, std_grad = time_model.predict(
                     X, return_std=True, return_mean_grad=True, return_std_grad=True
                 )
             else:
                 mu, std = time_model.predict(X, return_std=True)
 
@@ -82,23 +104,30 @@
             # inv_t = exp(g)
             # d(inv_t) = inv_t * grad(g)
             # d(inv_t) = inv_t * (-mu_grad + std * std_grad)
             if return_grad:
                 acq_grad *= inv_t
                 acq_grad += acq_vals * (-mu_grad + std * std_grad)
 
+    elif acq_func in ["MES"]:
+        acq_vals = -gaussian_mes(X, model, deterministic=deterministic)
+        if return_grad:
+            raise NotImplementedError(
+                "Gradient not implemented for MES acquisition function."
+            )
     else:
         raise ValueError("Acquisition function not implemented.")
 
     if return_grad:
         return acq_vals, acq_grad
+
     return acq_vals
 
 
-def gaussian_lcb(X, model, kappa=1.96, return_grad=False):
+def gaussian_lcb(X, model, kappa=1.96, return_grad=False, deterministic=False):
     """
     Use the lower confidence bound to estimate the acquisition
     values.
 
     The trade-off between exploitation and exploration is left to
     be controlled by the user through the parameter ``kappa``.
 
@@ -143,21 +172,27 @@
             )
 
             if kappa == "inf":
                 return -std, -std_grad
             return mu - kappa * std, mu_grad - kappa * std_grad
 
         else:
-            mu, std = model.predict(X, return_std=True)
+            if deterministic:
+                mu, std_al, std_ep = model.predict(
+                    X, return_std=True, disentangled_std=True
+                )
+                std = std_ep
+            else:
+                mu, std = model.predict(X, return_std=True)
             if kappa == "inf":
                 return -std
             return mu - kappa * std
 
 
-def gaussian_pi(X, model, y_opt=0.0, xi=0.01, return_grad=False):
+def gaussian_pi(X, model, y_opt=0.0, xi=0.01, return_grad=False, deterministic=False):
     """
     Use the probability of improvement to calculate the acquisition values.
 
     The conditional probability `P(y=f(x) | x)` form a gaussian with a
     certain mean and standard deviation approximated by the model.
 
     The PI condition is derived by computing ``E[u(f(x))]``
@@ -202,15 +237,21 @@
         warnings.simplefilter("ignore")
 
         if return_grad:
             mu, std, mu_grad, std_grad = model.predict(
                 X, return_std=True, return_mean_grad=True, return_std_grad=True
             )
         else:
-            mu, std = model.predict(X, return_std=True)
+            if deterministic:
+                mu, std_al, std_ep = model.predict(
+                    X, return_std=True, disentangled_std=True
+                )
+                std = std_ep
+            else:
+                mu, std = model.predict(X, return_std=True)
 
     # check dimensionality of mu, std so we can divide them below
     if (mu.ndim != 1) or (std.ndim != 1):
         raise ValueError(
             "mu and std are {}-dimensional and {}-dimensional, "
             "however both must be 1-dimensional. Did you train "
             "your model with an (N, 1) vector instead of an "
@@ -233,15 +274,15 @@
         improve_grad /= std**2
 
         return values, improve_grad * norm.pdf(scaled)
 
     return values
 
 
-def gaussian_ei(X, model, y_opt=0.0, xi=0.01, return_grad=False):
+def gaussian_ei(X, model, y_opt=0.0, xi=0.01, return_grad=False, deterministic=False):
     """
     Use the expected improvement to calculate the acquisition values.
 
     The conditional probability `P(y=f(x) | x)` form a gaussian with a certain
     mean and standard deviation approximated by the model.
 
     The EI condition is derived by computing ``E[u(f(x))]``
@@ -286,15 +327,21 @@
 
         if return_grad:
             mu, std, mu_grad, std_grad = model.predict(
                 X, return_std=True, return_mean_grad=True, return_std_grad=True
             )
 
         else:
-            mu, std = model.predict(X, return_std=True)
+            if deterministic:
+                mu, std_al, std_ep = model.predict(
+                    X, return_std=True, disentangled_std=True
+                )
+                std = std_ep
+            else:
+                mu, std = model.predict(X, return_std=True)
 
     # check dimensionality of mu, std so we can divide them below
     if (mu.ndim != 1) or (std.ndim != 1):
         raise ValueError(
             "mu and std are {}-dimensional and {}-dimensional, "
             "however both must be 1-dimensional. Did you train "
             "your model with an (N, 1) vector instead of an "
@@ -324,7 +371,91 @@
         exploit_grad = -mu_grad * cdf - pdf_grad
         explore_grad = std_grad * pdf + pdf_grad
 
         grad = exploit_grad + explore_grad
         return values, grad
 
     return values
+
+
+def gaussian_mes(X, model, k_samples=10, deterministic=False):
+    """
+    Use the max-value entropy to calculate the acquisition values.
+    Article: https://arxiv.org/abs/1703.01968
+    Source implementation: https://github.com/zi-w/Max-value-Entropy-Search/blob/master/acFuns/evaluateMES.m
+
+    The conditional probability `P(y=f(x) | x)` form a gaussian with a certain
+    mean and standard deviation approximated by the model.
+
+    The EI condition is derived by computing ``E[u(f(x))]``
+    where ``u(f(x)) = 0``, if ``f(x) > y_opt`` and ``u(f(x)) = y_opt - f(x)``,
+    if``f(x) < y_opt``.
+
+    This solves one of the issues of the PI condition by giving a reward
+    proportional to the amount of improvement got.
+
+    Note that the value returned by this function should be maximized to
+    obtain the ``X`` with maximum improvement.
+
+    Parameters
+    ----------
+    X : array-like, shape=(n_samples, n_features)
+        Values where the acquisition function should be computed.
+
+    model : sklearn estimator that implements predict with ``return_std``
+        The fit estimator that approximates the function through the
+        method ``predict``.
+        It should have a ``return_std`` parameter that returns the standard
+        deviation.
+
+    y_opt : float, default 0
+        Previous minimum value which we would like to improve upon.
+
+    xi : float, default=0.01
+        Controls how much improvement one wants over the previous best
+        values. Useful only when ``method`` is set to "EI"
+
+    return_grad : boolean, optional
+        Whether or not to return the grad. Implemented only for the case where
+        ``X`` is a single sample.
+
+    Returns
+    -------
+    values : array-like, shape=(X.shape[0],)
+        Acquisition function values computed at X.
+    """
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+
+        if deterministic:
+            mu, std_al, std_ep = model.predict(
+                X, return_std=True, disentangled_std=True
+            )
+            std = std_ep
+        else:
+            mu, std = model.predict(X, return_std=True)
+
+        # MES is defined for a maximization problem but the model prediction are for minimization
+        # we map minimization to maximization by multiplying by -1
+        mu *= -1
+
+    # check dimensionality of mu, std so we can divide them below
+    if (mu.ndim != 1) or (std.ndim != 1):
+        raise ValueError(
+            "mu, std_al, std_ep are {}-dimensional and {}-dimensional, "
+            "however both must be 1-dimensional. Did you train "
+            "your model with an (N, 1) vector instead of an "
+            "(N,) vector?".format(mu.ndim, std.ndim)
+        )
+
+    values = np.zeros_like(mu)
+    eps = 1e-10
+    std = np.maximum(std, eps)
+    for _ in range(k_samples):
+        y_sample = norm.rvs(loc=mu, scale=std)
+        gamma = (np.max(y_sample) - mu) / std
+        pdfgamma = np.maximum(norm.pdf(gamma), eps)
+        cdfgamma = np.maximum(norm.cdf(gamma), eps)
+        values += 0.5 * gamma * pdfgamma / cdfgamma - np.log(cdfgamma)
+    values /= k_samples
+
+    return values
```

### Comparing `deephyper-0.6.0/deephyper/skopt/benchmarks.py` & `deephyper-0.7.0/deephyper/skopt/benchmarks.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/callbacks.py` & `deephyper-0.7.0/deephyper/skopt/callbacks.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/__init__.py` & `deephyper-0.7.0/deephyper/skopt/learning/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/forest.py` & `deephyper-0.7.0/deephyper/skopt/learning/forest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,98 @@
 import numpy as np
 from sklearn.ensemble import ExtraTreesRegressor as _sk_ExtraTreesRegressor
 from sklearn.ensemble._forest import DecisionTreeRegressor, ForestRegressor
 
 from deephyper.core.utils.joblib_utils import Parallel, delayed
 
 
+def _accumulate_prediction_disentangled(tree, X, min_variance, out, lock):
+    """
+    This is a utility function for joblib's Parallel.
+
+    It can't go locally in ForestClassifier or ForestRegressor, because joblib
+    complains that it cannot pickle it when placed there.
+    """
+
+    mean_tree = tree.predict(X).T
+    var_tree = tree.tree_.impurity[tree.apply(X)]
+
+    # This rounding off is done in accordance with the
+    # adjustment done in section 4.3.3
+    # of http://arxiv.org/pdf/1211.0906v2.pdf to account
+    # for cases such as leaves with 1 sample in which there
+    # is zero variance.
+    var_tree = np.maximum(var_tree, min_variance)
+
+    with lock:
+        out[0] += mean_tree
+        out[1] += var_tree
+        out[2] += mean_tree**2
+
+
+def _return_mean_and_std_distentangled(X, n_outputs, trees, min_variance, n_jobs):
+    """
+    Returns `std(Y | X)`.
+
+    Can be calculated by E[Var(Y | Tree)] + Var(E[Y | Tree]) where
+    P(Tree) is `1 / len(trees)`.
+
+    Parameters
+    ----------
+    X : array-like, shape=(n_samples, n_features)
+        Input data.
+
+    n_outputs: int.
+        Number of outputs.
+
+    trees : list, shape=(n_estimators,)
+        List of fit sklearn trees as obtained from the ``estimators_``
+        attribute of a fit RandomForestRegressor or ExtraTreesRegressor.
+
+    predictions : array-like, shape=(n_samples,)
+        Prediction of each data point as returned by RandomForestRegressor
+        or ExtraTreesRegressor.
+
+    Returns
+    -------
+    std : array-like, shape=(n_samples,)
+        Standard deviation of `y` at `X`. If criterion
+        is set to "mse", then `std[i] ~= std(y | X[i])`.
+
+    """
+    # This derives std(y | x) as described in 4.3.2 of arXiv:1211.0906
+
+    mean = np.zeros((n_outputs, len(X)))
+    std_al = np.zeros((n_outputs, len(X)))
+    std_ep = np.zeros((n_outputs, len(X)))
+
+    # Parallel loop
+    lock = threading.Lock()
+    Parallel(n_jobs=n_jobs, verbose=0, require="sharedmem")(
+        delayed(_accumulate_prediction_disentangled)(
+            tree, X, min_variance, [mean, std_al, std_ep], lock
+        )
+        for tree in trees
+    )
+
+    mean, std_al, std_ep = mean.T, std_al.T, std_ep.T
+    mean /= len(trees)
+
+    std_al /= len(trees)
+    std_ep = std_ep / len(trees) - mean**2
+
+    std_al[std_al <= 0.0] = 0.0
+    std_al **= 0.5
+
+    std_ep[std_ep <= 0.0] = 0.0
+    std_ep **= 0.5
+
+    return mean.reshape(-1), std_al.reshape(-1), std_ep.reshape(-1)
+
+
 def _accumulate_prediction(tree, X, min_variance, out, lock):
     """
     This is a utility function for joblib's Parallel.
 
     It can't go locally in ForestClassifier or ForestRegressor, because joblib
     complains that it cannot pickle it when placed there.
     """
@@ -91,22 +175,21 @@
 
     criterion : string, optional (default="mse")
         The function to measure the quality of a split. Supported criteria
         are "mse" for the mean squared error, which is equal to variance
         reduction as feature selection criterion, and "mae" for the mean
         absolute error.
 
-    max_features : int, float, string or None, optional (default="auto")
+    max_features : int, float, string or None, optional (default="1.0")
         The number of features to consider when looking for the best split:
 
         - If int, then consider `max_features` features at each split.
         - If float, then `max_features` is a percentage and
           `int(max_features * n_features)` features are considered at each
           split.
-        - If "auto", then `max_features=n_features`.
         - If "sqrt", then `max_features=sqrt(n_features)`.
         - If "log2", then `max_features=log2(n_features)`.
         - If None, then `max_features=n_features`.
 
         .. note::
             The search for a split does not stop until at least one
             valid partition of the node samples is found, even if it
@@ -225,18 +308,18 @@
 
     def __init__(
         self,
         n_estimators=100,
         *,
         criterion="squared_error",
         max_depth=None,
-        min_samples_split=2,
+        min_samples_split=10,
         min_samples_leaf=1,
         min_weight_fraction_leaf=0.0,
-        max_features="auto",
+        max_features=1.0,
         max_leaf_nodes=None,
         min_impurity_decrease=0.0,
         bootstrap=True,
         oob_score=False,
         n_jobs=None,
         random_state=None,
         verbose=0,
@@ -244,27 +327,28 @@
         ccp_alpha=0.0,
         max_samples=None,
         min_variance=0.0,
         splitter="random"
     ):
         super().__init__(
             # !keyword-argument changing from sklearn==1.2.0, positional fixed it!
-            DecisionTreeRegressor(splitter=splitter),
+            DecisionTreeRegressor(),
             n_estimators=n_estimators,
             estimator_params=(
                 "criterion",
                 "max_depth",
                 "min_samples_split",
                 "min_samples_leaf",
                 "min_weight_fraction_leaf",
                 "max_features",
                 "max_leaf_nodes",
                 "min_impurity_decrease",
                 "random_state",
                 "ccp_alpha",
+                "splitter",
             ),
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
             random_state=random_state,
             verbose=verbose,
             warm_start=warm_start,
@@ -280,15 +364,15 @@
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
 
         self.min_variance = min_variance
         self.splitter = splitter
 
-    def predict(self, X, return_std=False):
+    def predict(self, X, return_std=False, disentangled_std=False):
         """Predict continuous output for X.
 
         Parameters
         ----------
         X : array of shape = (n_samples, n_features)
             Input data.
 
@@ -301,25 +385,32 @@
             Predicted values for X. If criterion is set to "mse",
             then `predictions[i] ~= mean(y | X[i])`.
 
         std : array-like of shape=(n_samples,)
             Standard deviation of `y` at `X`. If criterion
             is set to "mse", then `std[i] ~= std(y | X[i])`.
 
+        disentangled_std : the std is returned disentangled between aleatoric and epistemic.
         """
         if return_std:
             if self.criterion != "squared_error":
                 raise ValueError(
                     "Expected impurity to be 'squared_error', got %s instead"
                     % self.criterion
                 )
-            mean, std = _return_mean_and_std(
-                X, self.n_outputs_, self.estimators_, self.min_variance, self.n_jobs
-            )
-            return mean, std
+            if disentangled_std:
+                mean, std_al, std_ep = _return_mean_and_std_distentangled(
+                    X, self.n_outputs_, self.estimators_, self.min_variance, self.n_jobs
+                )
+                return mean, std_al, std_ep
+            else:
+                mean, std = _return_mean_and_std(
+                    X, self.n_outputs_, self.estimators_, self.min_variance, self.n_jobs
+                )
+                return mean, std
         else:
             mean = super(RandomForestRegressor, self).predict(X)
 
             return mean
 
 
 class ExtraTreesRegressor(_sk_ExtraTreesRegressor):
@@ -463,30 +554,31 @@
     ----------
     .. [1] L. Breiman, "Random Forests", Machine Learning, 45(1), 5-32, 2001.
 
     """
 
     def __init__(
         self,
-        n_estimators=10,
+        n_estimators=100,
         criterion="squared_error",
         max_depth=None,
-        min_samples_split=2,
+        min_samples_split=10,
         min_samples_leaf=1,
         min_weight_fraction_leaf=0.0,
-        max_features="auto",
+        max_features=1.0,
         max_leaf_nodes=None,
         min_impurity_decrease=0.0,
         bootstrap=False,
         oob_score=False,
         n_jobs=1,
         random_state=None,
         verbose=0,
         warm_start=False,
         min_variance=0.0,
+        max_samples=None,
     ):
         self.min_variance = min_variance
         super(ExtraTreesRegressor, self).__init__(
             n_estimators=n_estimators,
             criterion=criterion,
             max_depth=max_depth,
             min_samples_split=min_samples_split,
@@ -497,17 +589,18 @@
             min_impurity_decrease=min_impurity_decrease,
             bootstrap=bootstrap,
             oob_score=oob_score,
             n_jobs=n_jobs,
             random_state=random_state,
             verbose=verbose,
             warm_start=warm_start,
+            max_samples=max_samples,
         )
 
-    def predict(self, X, return_std=False):
+    def predict(self, X, return_std=False, disentangled_std=False):
         """
         Predict continuous output for X.
 
         Parameters
         ----------
         X : array-like of shape=(n_samples, n_features)
             Input data.
@@ -527,15 +620,21 @@
         """
         if return_std:
             if self.criterion != "squared_error":
                 raise ValueError(
                     "Expected impurity to be 'squared_error', got %s instead"
                     % self.criterion
                 )
-            mean, std = _return_mean_and_std(
-                X, self.n_outputs_, self.estimators_, self.min_variance, self.n_jobs
-            )
-            return mean, std
+            if disentangled_std:
+                mean, std_al, std_ep = _return_mean_and_std_distentangled(
+                    X, self.n_outputs_, self.estimators_, self.min_variance, self.n_jobs
+                )
+                return mean, std_al, std_ep
+            else:
+                mean, std = _return_mean_and_std(
+                    X, self.n_outputs_, self.estimators_, self.min_variance, self.n_jobs
+                )
+                return mean, std
         else:
             mean = super(ExtraTreesRegressor, self).predict(X)
 
             return mean
```

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/gpr.py` & `deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/gpr.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/kernels.py` & `deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/kernels.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/tests/test_gpr.py` & `deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/tests/test_gpr.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/gaussian_process/tests/test_kernels.py` & `deephyper-0.7.0/deephyper/skopt/learning/gaussian_process/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/gbrt.py` & `deephyper-0.7.0/deephyper/skopt/learning/gbrt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from sklearn.base import BaseEstimator, RegressorMixin, clone
-from sklearn.ensemble import GradientBoostingRegressor
+from sklearn.ensemble import GradientBoostingRegressor, HistGradientBoostingRegressor
 from sklearn.utils import check_random_state
 
 from deephyper.core.utils.joblib_utils import Parallel, delayed
 
 
 def _parallel_fit(regressor, X, y):
     return regressor.fit(X, y)
@@ -64,36 +64,44 @@
         rng = check_random_state(self.random_state)
 
         if self.base_estimator is None:
             base_estimator = GradientBoostingRegressor(loss="quantile")
         else:
             base_estimator = self.base_estimator
 
-            if not isinstance(base_estimator, GradientBoostingRegressor):
+            if not isinstance(
+                base_estimator,
+                (GradientBoostingRegressor, HistGradientBoostingRegressor),
+            ):
                 raise ValueError(
-                    "base_estimator has to be of type" " GradientBoostingRegressor."
+                    "base_estimator has to be of type"
+                    " GradientBoostingRegressor or HistGradientBoostingRegressor."
                 )
 
             if not base_estimator.loss == "quantile":
                 raise ValueError(
                     "base_estimator has to use quantile"
                     " loss not %s" % base_estimator.loss
                 )
 
         # The predictions for different quantiles should be sorted.
         # Therefore each of the regressors need the same seed.
         base_estimator.set_params(random_state=rng)
         regressors = []
         for q in self.quantiles:
             regressor = clone(base_estimator)
-            regressor.set_params(alpha=q)
+
+            if isinstance(regressor, GradientBoostingRegressor):
+                regressor.set_params(alpha=q)
+            elif isinstance(regressor, HistGradientBoostingRegressor):
+                regressor.set_params(quantile=q)
 
             regressors.append(regressor)
 
-        self.regressors_ = Parallel(n_jobs=self.n_jobs, backend="threading")(
+        self.regressors_ = Parallel(n_jobs=self.n_jobs, prefer="threads")(
             delayed(_parallel_fit)(regressor, X, y) for regressor in regressors
         )
 
         return self
 
     def predict(self, X, return_std=False, return_quantiles=False):
         """Predict.
@@ -120,11 +128,14 @@
                 raise ValueError(
                     "return_std works only if the quantiles during "
                     "instantiation include 0.16, 0.5 and 0.84"
                 )
             low = self.regressors_[self.quantiles.index(0.16)].predict(X)
             high = self.regressors_[self.quantiles.index(0.84)].predict(X)
             mean = self.regressors_[self.quantiles.index(0.5)].predict(X)
-            return mean, ((high - low) / 2.0)
+            std = (high - low) / 2.0
+            # This avoids NaN when computing the Negative Log-likelihood
+            std[std <= 0.01] = 0.01
+            return mean, std
 
         # return the mean
         return self.regressors_[self.quantiles.index(0.5)].predict(X)
```

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/tests/test_forest.py` & `deephyper-0.7.0/deephyper/skopt/learning/tests/test_forest.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/learning/tests/test_gbrt.py` & `deephyper-0.7.0/deephyper/skopt/learning/tests/test_gbrt.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/moo/__init__.py` & `deephyper-0.7.0/deephyper/skopt/moo/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/moo/_hv.py` & `deephyper-0.7.0/deephyper/skopt/moo/_hv.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/moo/_multiobjective.py` & `deephyper-0.7.0/deephyper/skopt/moo/_multiobjective.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/moo/_pf.py` & `deephyper-0.7.0/deephyper/skopt/moo/_pf.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,41 @@
 
     Returns:
         bool: True if the vector is pareto efficient and false otherwise.
     """
     return np.all(np.any(np.asarray(new_obj) < objvals, axis=1))
 
 
-def pareto_front(y, sort=False):
+def pareto_front(y, sort=False, return_idx=False):
     """Extract the pareto front (actual objective values of the non-dominated set).
 
     Args:
         y (array or list): Array or list of size (n_points, n_objectives).
         sort (bool, optional): Whether to sort the pareto front (practical to plot in 2D or 3D). Defaults to False.
+        return_idx (bool, optional): Whether to return the indices of the pareto front in the original array. Defaults to False.
 
     Returns:
         array: Subarray of y representing the pareto front.
     """
-    nds = non_dominated_set(y, return_mask=False)
-    pf = y[nds]
+    nds_idx = non_dominated_set(y, return_mask=False)
+    pf = y[nds_idx]
 
     if sort:
         n_objectives = y.shape[1]
         pf = np.array(
             [tuple(row) for row in pf],
             dtype=[(f"objective_{i}", float) for i in range(n_objectives)],
         )
-        pf.sort(order=[f"objective_{i}" for i in range(n_objectives)])
+        sorted_idx = pf.argsort(order=[f"objective_{i}" for i in range(n_objectives)])
+        pf = pf[sorted_idx]
         pf = np.array([list(row) for row in pf])
+        nds_idx = nds_idx[sorted_idx]
 
+    if return_idx:
+        return pf, nds_idx
     return pf
 
 
 def non_dominated_set_ranked(y, fraction, return_mask=True):
     """Find the set of top-``fraction x 100%`` of non-dominated points. The number of points returned is ``min(n_points, ceil(fraction * n_points))`` where ``n_points`` is the number of points in the input array. Function assumes minimization.
 
     Args:
```

### Comparing `deephyper-0.6.0/deephyper/skopt/optimizer/base.py` & `deephyper-0.7.0/deephyper/skopt/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/optimizer/dummy.py` & `deephyper-0.7.0/deephyper/skopt/optimizer/dummy.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/optimizer/forest.py` & `deephyper-0.7.0/deephyper/skopt/optimizer/forest.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/optimizer/gbrt.py` & `deephyper-0.7.0/deephyper/skopt/optimizer/gbrt.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/optimizer/gp.py` & `deephyper-0.7.0/deephyper/skopt/optimizer/gp.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/optimizer/optimizer.py` & `deephyper-0.7.0/deephyper/skopt/optimizer/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import numbers
 import sys
 import warnings
 from math import log
-import numbers
 
-import ConfigSpace as CS
 import numpy as np
 import pandas as pd
 from scipy.optimize import fmin_l_bfgs_b
 from sklearn.base import clone, is_regressor
 from sklearn.multioutput import MultiOutputRegressor
 from sklearn.utils import check_random_state
 
@@ -234,25 +233,42 @@
 
         # Configure acquisition function
 
         # Store and creat acquisition function set
         self.acq_func = acq_func
         self.acq_func_kwargs = acq_func_kwargs
 
-        allowed_acq_funcs = ["gp_hedge", "EI", "LCB", "qLCB", "PI", "EIps", "PIps"]
+        allowed_acq_funcs = [
+            "gp_hedge",
+            "EI",
+            "LCB",
+            "PI",
+            "MES",
+            "EIps",
+            "PIps",
+            # TODO: new acquisition functions
+            "gp_hedged",
+            "EId",
+            "LCBd",
+            "PId",
+            "MESd",
+        ]
         if self.acq_func not in allowed_acq_funcs:
             raise ValueError(
                 "expected acq_func to be in %s, got %s"
                 % (",".join(allowed_acq_funcs), self.acq_func)
             )
 
         # treat hedging method separately
-        if self.acq_func == "gp_hedge":
+        if "gp_hedge" in self.acq_func:
             self.cand_acq_funcs_ = ["EI", "LCB", "PI"]
-            self.gains_ = np.zeros(3)
+            if self.acq_func[-1] == "d":
+                # add "d" to the end of the name
+                self.cand_acq_funcs_ = [k + "d" for k in self.cand_acq_funcs_]
+            self.gains_ = np.zeros(len(self.cand_acq_funcs_))
         else:
             self.cand_acq_funcs_ = [self.acq_func]
 
         if acq_func_kwargs is None:
             acq_func_kwargs = dict()
         self.eta = acq_func_kwargs.get("eta", 1.0)
 
@@ -306,83 +322,95 @@
         # decide optimizer based on gradient information
         if acq_optimizer == "auto":
             if has_gradients(self.base_estimator_):
                 acq_optimizer = "lbfgs"
             else:
                 acq_optimizer = "sampling"
 
-        if acq_optimizer not in ["lbfgs", "sampling", "boltzmann_sampling"]:
+        if acq_optimizer not in [
+            "lbfgs",
+            "sampling",
+            "mixedga",
+            "ga",
+            "cobyqa",
+        ]:
             raise ValueError(
                 "Expected acq_optimizer to be 'lbfgs' or "
-                "'sampling' or 'softmax_sampling', got {0}".format(acq_optimizer)
+                "'sampling' or 'ga', got {0}".format(acq_optimizer)
             )
 
-        if not has_gradients(self.base_estimator_) and not (
-            "sampling" in acq_optimizer
-        ):
-            raise ValueError(
-                "The regressor {0} should run with a 'sampling' "
-                "acq_optimizer such as "
-                "'sampling' or 'softmax_sampling'.".format(type(base_estimator))
-            )
         self.acq_optimizer = acq_optimizer
 
         # record other arguments
         if acq_optimizer_kwargs is None:
             acq_optimizer_kwargs = dict()
 
-        self.n_points = acq_optimizer_kwargs.get("n_points", 10000)
+        self.n_points = acq_optimizer_kwargs.get("n_points", 10_000)
         self.n_restarts_optimizer = acq_optimizer_kwargs.get("n_restarts_optimizer", 5)
         self.n_jobs = acq_optimizer_kwargs.get("n_jobs", 1)
+
+        # PyMOO
+        self._pymoo_pop_size = acq_optimizer_kwargs.get("pop_size", 100)
+        self._pymoo_termination_kwargs = {
+            "xtol": acq_optimizer_kwargs.get("xtol", 1e-3),
+            "ftol": acq_optimizer_kwargs.get("ftol", 1e-3),
+            "period": acq_optimizer_kwargs.get("period", 15),
+            "n_max_gen": acq_optimizer_kwargs.get("n_max_gen", 1000),
+        }
+
+        # TODO: "update_prior" to be removed, this mechanism is too prone to "overfitting" (local minima problems)
         self.update_prior = acq_optimizer_kwargs.get("update_prior", False)
         self.update_prior_quantile = acq_optimizer_kwargs.get(
             "update_prior_quantile", 0.9
         )
         self.filter_duplicated = acq_optimizer_kwargs.get("filter_duplicated", True)
-        self.boltzmann_gamma = acq_optimizer_kwargs.get("boltzmann_gamma", 1)
-        self.boltzmann_psucc = acq_optimizer_kwargs.get("boltzmann_psucc", 0)
         self.filter_failures = acq_optimizer_kwargs.get("filter_failures", "mean")
         self.max_failures = acq_optimizer_kwargs.get("max_failures", 100)
+        self.acq_optimizer_freq = acq_optimizer_kwargs.get("acq_optimizer_freq", 1)
         self.acq_optimizer_kwargs = acq_optimizer_kwargs
 
-        # Configure search space
-
-        if type(dimensions) is CS.ConfigurationSpace:
-            # Save the config space to do a real copy of the Optimizer
-            self.config_space = dimensions
-            self.config_space.seed(self.rng.get_state()[1][0])
+        # keep track of the generative model from sdv
+        self.model_sdv = model_sdv
 
-            if isinstance(self.base_estimator_, GaussianProcessRegressor):
-                raise RuntimeError("GP estimator is not available with ConfigSpace!")
+        if isinstance(dimensions, Space):
+            self.space = dimensions
+            self.space.model_sdv = self.model_sdv
+        elif isinstance(dimensions, (list, tuple)):
+            self.space = Space(dimensions, model_sdv=self.model_sdv)
         else:
-            # normalize space if GP regressor
-            if isinstance(self.base_estimator_, GaussianProcessRegressor):
-                dimensions = normalize_dimensions(dimensions)
+            raise ValueError("Dimensions should be a list or an instance of Space.")
 
-        # keep track of the generative model from sdv
-        self.model_sdv = model_sdv
+        transformer = self.space.get_transformer()
+
+        self.space.set_transformer(transformer)
+
+        # normalize space if GP regressor
+        if (
+            isinstance(self.base_estimator_, GaussianProcessRegressor)
+            or type(self.base_estimator_).__name__ == "MondrianForestRegressor"
+        ):
+            self.space.dimensions = normalize_dimensions(self.space.dimensions)
 
-        self.space = Space(dimensions, model_sdv=self.model_sdv)
+        if self.space.config_space:
+            self.space.config_space.seed(self.rng.get_state()[1][0])
 
         self._initial_samples = [] if initial_points is None else initial_points[:]
         self._initial_point_generator = cook_initial_point_generator(
             initial_point_generator
         )
 
         if self._initial_point_generator is not None:
-            transformer = self.space.get_transformer()
             self._initial_samples = (
                 self._initial_samples
                 + self._initial_point_generator.generate(
                     self.space.dimensions,
                     n_initial_points - len(self._initial_samples),
                     random_state=self.rng.randint(0, np.iinfo(np.int32).max),
                 )
             )
-            self.space.set_transformer(transformer)
 
         # record categorical and non-categorical indices
         self._cat_inds = []
         self._non_cat_inds = []
         for ind, dim in enumerate(self.space.dimensions):
             if isinstance(dim, Categorical):
                 self._cat_inds.append(ind)
@@ -443,31 +471,30 @@
         self._min_value = 0
         self._max_value = 0
 
         # parameters to stabilize the size of the dataset used to fit the surrogate model
         self._sample_max_size = sample_max_size
         self._sample_strategy = sample_strategy
 
-        # parameters for multifidelity
-        self._use_multifidelity = False
-        self.bi = []
-        self.bi_count = {}
+        # Count number of surrogate model fittings
+        self._counter_fit = 0
+
+        # TODO: to monitor the BO
+        self._last_est = None
 
     def copy(self, random_state=None):
         """Create a shallow copy of an instance of the optimizer.
 
         Parameters
         ----------
         random_state : int, RandomState instance, or None (default)
             Set the random state of the copy.
         """
         optimizer = Optimizer(
-            dimensions=self.config_space
-            if hasattr(self, "config_space")
-            else self.space.dimensions,
+            dimensions=self.space,
             base_estimator=self.base_estimator_,
             n_initial_points=self.n_initial_points_,
             initial_point_generator=self._initial_point_generator,
             acq_func=self.acq_func,
             acq_optimizer=self.acq_optimizer,
             acq_func_kwargs=self.acq_func_kwargs,
             acq_optimizer_kwargs=self.acq_optimizer_kwargs,
@@ -487,17 +514,19 @@
 
         if hasattr(self, "gains_"):
             optimizer.gains_ = np.copy(self.gains_)
 
         if self.Xi:
             optimizer._tell(self.Xi, self.yi)
 
+        optimizer._counter_fit = self._counter_fit
+
         return optimizer
 
-    def ask(self, n_points=None, strategy="cl_min"):
+    def ask(self, n_points=None, strategy="cl_min", strategy_kwargs=None):
         """Query point or multiple points at which objective should be evaluated.
 
         n_points : int or None, default: None
             Number of points returned by the ask method.
             If the value is None, a single point to evaluate is returned.
             Otherwise a list of points to evaluate is returned of size
             n_points. This is useful if you can evaluate your objective in
@@ -529,30 +558,29 @@
             self.sampled.append(x)
 
             if n_points is None:
                 return x
             else:
                 return [x]
 
+        strategy_kwargs = strategy_kwargs or {}
+
         if n_points > 0 and (
             self._n_initial_points > 0 or self.base_estimator_ is None
         ):
             if len(self._initial_samples) == 0:
                 X = self._ask_random_points(size=n_points)
             else:
                 n = min(len(self._initial_samples), n_points)
                 X = self._initial_samples[:n]
                 self._initial_samples = self._initial_samples[n:]
                 X = X + self._ask_random_points(size=(n_points - n))
             self.sampled.extend(X)
             return X
 
-        if self.acq_func == "qLCB":
-            strategy = "qLCB"
-
         supported_strategies = [
             "cl_min",
             "cl_mean",
             "cl_max",
             "topk",
             "boltzmann",
             "qLCB",
@@ -576,15 +604,17 @@
                 next_samples = self._last_X[idx].tolist()
 
                 # to track sampled values and avoid duplicates
                 self.sampled.extend(next_samples)
 
                 return next_samples
 
-            elif strategy == "boltmann":
+            elif strategy == "boltzmann":
+                gamma = strategy_kwargs.get("gamma", 1.0)
+
                 values = -self._last_values
 
                 self._min_value = (
                     self._min_value
                     if self._min_value is None
                     else min(values.min(), self._min_value)
                 )
@@ -600,15 +630,15 @@
 
                 while len(idx) < n_points:
                     t = len(self.sampled)
                     if t == 0:
                         beta = 0
                     else:
                         beta = (
-                            self.boltzmann_gamma
+                            gamma
                             * np.log(t)
                             / np.abs(self._max_value - self._min_value)
                         )
 
                     probs = boltzmann_distribution(values, beta)
 
                     new_idx = np.argmax(self.rng.multinomial(1, probs))
@@ -627,30 +657,29 @@
             else:
                 raise ValueError(
                     f"'{strategy}' is not a valid multi-point acquisition strategy!"
                 )
 
         # q-ACQ multi point acquisition for centralized setting
         if len(self.models) > 0 and strategy == "qLCB":
-            X_s = self.space.rvs(
+            Xsample = self.space.rvs(
                 n_samples=self.n_points, random_state=self.rng, n_jobs=self.n_jobs
             )
-            X_s = self._filter_duplicated(X_s)
-            X_c = self.space.imp_const.fit_transform(
-                self.space.transform(X_s)
-            )  # candidates
 
-            mu, std = self.models[-1].predict(X_c, return_std=True)
+            Xsample = self._filter_duplicated(Xsample)
+            Xsample_transformed = self.space.transform(Xsample)
+
+            mu, std = self.models[-1].predict(Xsample_transformed, return_std=True)
             kappa = self.acq_func_kwargs.get("kappa", 1.96)
             kappas = self.rng.exponential(kappa, size=n_points - 1)
             X = [self._next_x]
             for kappa in kappas:
                 values = mu - kappa * std
                 idx = np.argmin(values)
-                X.append(X_s[idx])
+                X.append(Xsample[idx])
             return X
 
         # Caching the result with n_points not None. If some new parameters
         # are provided to the ask, the cache_ is not used.
         if (n_points, strategy) in self.cache_:
             return self.cache_[(n_points, strategy)]
 
@@ -680,14 +709,18 @@
             elif strategy == "cl_mean":
                 y_lie = np.mean(opt_yi, axis=0) if opt_yi else 0.0  # CL-mean lie
                 t_lie = np.mean(ti) if ti is not None else log(sys.float_info.max)
             else:
                 y_lie = np.max(opt_yi, axis=0) if opt_yi else 0.0  # CL-max lie
                 t_lie = np.max(ti) if ti is not None else log(sys.float_info.max)
 
+            # Converts both numpy scalar or arrays, it is necessary to avoid y_lie
+            # being an array triggering an issue in _tell
+            y_lie = y_lie.tolist()
+
             # Lie to the optimizer.
             if "ps" in self.acq_func:
                 # Use `_tell()` instead of `tell()` to prevent repeated
                 # log transformations of the computation times.
                 opt._tell(x, (y_lie, t_lie))
             else:
                 opt._tell(x, y_lie)
@@ -705,18 +738,15 @@
         Returns:
             list: the filtered list of samples
         """
 
         if self.filter_duplicated:
             # check duplicated values
 
-            if hasattr(self, "config_space"):
-                hps_names = self.config_space.get_hyperparameter_names()
-            else:
-                hps_names = self.space.dimension_names
+            hps_names = self.space.dimension_names
 
             df_samples = pd.DataFrame(data=samples, columns=hps_names, dtype="O")
             df_samples = df_samples[~df_samples.duplicated(keep="first")]
 
             if len(self.sampled) > 0:
                 df_history = pd.DataFrame(data=self.sampled, columns=hps_names)
                 df_merge = pd.merge(df_samples, df_history, on=None, how="inner")
@@ -785,24 +815,24 @@
                 y = np.concatenate(ys, axis=0)
 
         X = X.tolist()
         y = y.tolist()
         return X, y
 
     def _ask_random_points(self, size=None):
-        samples = self.space.rvs(
+        Xsamples = self.space.rvs(
             n_samples=self.n_points, random_state=self.rng, n_jobs=self.n_jobs
         )
 
-        samples = self._filter_duplicated(samples)
+        Xsamples = self._filter_duplicated(Xsamples)
 
         if size is None:
-            return samples[0]
+            return Xsamples[0]
         else:
-            return samples[:size]
+            return Xsamples[:size]
 
     def _ask(self):
         """Suggest next point at which to evaluate the objective.
 
         Return a random point while not at least `n_initial_points`
         observations have been `tell`ed, after that `base_estimator` is used
         to determine the next point.
@@ -822,22 +852,19 @@
             if not self.models:
                 raise RuntimeError(
                     "Random evaluations exhausted and no " "model has been fit."
                 )
 
             next_x = self._next_x
             if next_x is not None:
-                if not self.space.is_config_space:
-                    min_delta_x = min(
-                        [self.space.distance(next_x, xi) for xi in self.Xi]
+                min_delta_x = min([self.space.distance(next_x, xi) for xi in self.Xi])
+                if abs(min_delta_x) <= 1e-8:
+                    warnings.warn(
+                        "The objective has been evaluated " "at this point before."
                     )
-                    if abs(min_delta_x) <= 1e-8:
-                        warnings.warn(
-                            "The objective has been evaluated " "at this point before."
-                        )
 
             # return point computed from last call to tell()
             return next_x
 
     def tell(self, x, y, fit=True):
         """Record an observation (or several) of the objective function.
 
@@ -861,18 +888,15 @@
             Value of objective at `x`.
 
         fit : bool, default: True
             Fit a model to observed evaluations of the objective. A model will
             only be fitted after `n_initial_points` points have been told to
             the optimizer irrespective of the value of `fit`.
         """
-        if self.space.is_config_space:
-            pass
-        else:
-            check_x_in_space(x, self.space)
+        check_x_in_space(x, self.space)
 
         self._check_y_is_valid(x, y)
 
         # take the logarithm of the computation times
         if "ps" in self.acq_func:
             if is_2Dlistlike(x):
                 y = [[val, log(t)] for (val, t) in y]
@@ -888,43 +912,52 @@
 
         This method exists to give access to the internals of adding points
         by side stepping all input validation and transformation."""
         if "ps" in self.acq_func:
             if is_2Dlistlike(x):
                 self.Xi.extend(x)
                 self.yi.extend(y)
-                self._n_initial_points -= len([v for v in y if v != "F"])
+                n_new_points = len([v for v in y if v != "F"])
+                self._n_initial_points -= n_new_points
             elif is_listlike(x):
                 self.Xi.append(x)
                 self.yi.append(y)
                 if y != "F":
-                    self._n_initial_points -= 1
+                    n_new_points = 1
+                    self._n_initial_points -= n_new_points
+                else:
+                    n_new_points = 0
         # if y isn't a scalar it means we have been handed a batch of points
         elif is_listlike(y) and is_2Dlistlike(x):
             self.Xi.extend(x)
             self.yi.extend(y)
-            self._n_initial_points -= len([v for v in y if v != "F"])
+            n_new_points = len([v for v in y if v != "F"])
+            self._n_initial_points -= n_new_points
         elif is_listlike(x):
             self.Xi.append(x)
             self.yi.append(y)
             if y != "F":
-                self._n_initial_points -= 1
+                n_new_points = 1
+                self._n_initial_points -= n_new_points
+            else:
+                n_new_points = 0
         else:
             raise ValueError(
                 "Type of arguments `x` (%s) and `y` (%s) "
                 "not compatible." % (type(x), type(y))
             )
 
         # optimizer learned something new - discard cache
         self.cache_ = {}
 
         # after being "told" n_initial_points we switch from sampling
         # random points to using a surrogate model
         if fit and self._n_initial_points <= 0 and self.base_estimator_ is not None:
             transformed_bounds = self.space.transformed_bounds
+
             est = clone(self.base_estimator_)
 
             yi = self.yi
 
             # Convert multiple objectives to single scalar
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
@@ -958,156 +991,317 @@
 
             # Handle failures
             yi = self._filter_failures(yi)
 
             # handle size of the sample fit to the estimator
             Xi, yi = self._sample(self.Xi, yi)
 
+            # Preprocessing of input space
+            Xtransformed = np.asarray(self.space.transform(Xi))
+
+            # TODO: feature importance
+            # if len(Xi) % 25 == 0 and len(Xi) >= 25:
+            #     from sklearn.model_selection import train_test_split
+
+            #     Xtransformed, Xval, yi, yval = train_test_split(
+            #         Xtransformed,
+            #         yi,
+            #         test_size=0.2,
+            #         random_state=self.rng.randint(0, np.iinfo(np.int32).max),
+            #     )
+
+            # Fit surrogate model on transformed data
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
 
-                # preprocessing of input space
-                Xtt = self.space.imp_const.fit_transform(self.space.transform(Xi))
-                Xtt = np.asarray(Xtt)
+                self._last_est = est.fit(Xtransformed, yi)
 
-                # fit surrogate model
-                est.fit(Xtt, yi)
+            # TODO: to be removed
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
 
-                # update prior
+                # Update sampling prior
                 if self.update_prior:
-                    self.space.update_prior(Xtt, yi, q=self.update_prior_quantile)
+                    self.space.update_prior(
+                        Xtransformed, yi, q=self.update_prior_quantile
+                    )
+
+            # TODO: feature importance
+            # if len(Xi) % 25 == 0 and len(Xi) >= 25:
+            #     from sklearn.inspection import permutation_importance
+
+            #     est_score = est.score(Xval, yval)
+            #     print(f"Score: {est_score}")
+            #     var_importance = permutation_importance(
+            #         est,
+            #         Xval,
+            #         yval,
+            #         n_repeats=10,
+            #         random_state=self.rng.randint(0, np.iinfo(np.int32).max),
+            #     )
+
+            #     # var_importance_upper_bound = var_importance.importances_mean + 1.96 * var_importance.importances_std
+            #     # var_importance_fraction = var_importance_upper_bound / est_score
+            #     var_importance_fraction = var_importance.importances_mean / est_score
+            #     for i in range(len(var_importance_fraction)):
+            #         # if var_importance_fraction[i] < 0.05:
+            #         print(
+            #             f"dim {self.space.dimension_names[i]}: {var_importance_fraction[i]:.4f}"
+            #         )
+            #     print()
 
             if self.max_model_queue_size is None:
                 self.models.append(est)
             elif len(self.models) < self.max_model_queue_size:
                 self.models.append(est)
             else:
                 # Maximum list size obtained, remove oldest model.
                 self.models.pop(0)
                 self.models.append(est)
 
-            if hasattr(self, "next_xs_") and self.acq_func == "gp_hedge":
+            if hasattr(self, "next_xs_") and "gp_hedge" in self.acq_func:
                 self.gains_ -= est.predict(np.vstack(self.next_xs_))
 
             # even with BFGS as optimizer we want to sample a large number
             # of points and then pick the best ones as starting points
-            X_s = self.space.rvs(
+            Xsample = self.space.rvs(
                 n_samples=self.n_points, random_state=self.rng, n_jobs=self.n_jobs
             )
 
-            X_s = self._filter_duplicated(X_s)
+            Xsample = self._filter_duplicated(Xsample)
 
-            X = self.space.imp_const.fit_transform(self.space.transform(X_s))
+            Xsample_transformed = self.space.transform(Xsample)
 
             self.next_xs_ = []
+
+            do_only_sampling = (self.acq_optimizer == "sampling") or (
+                self._counter_fit % self.acq_optimizer_freq != 0
+            )
+
             for cand_acq_func in self.cand_acq_funcs_:
                 values = _gaussian_acquisition(
-                    X=X,
+                    X=Xsample_transformed,
                     model=est,
                     y_opt=np.min(yi),
                     acq_func=cand_acq_func,
                     acq_func_kwargs=self.acq_func_kwargs,
                 )
 
                 # cache these values in case the strategy of ask is one-shot
-                self._last_X = X
+                self._last_X = Xsample_transformed
                 self._last_values = values
 
                 # Find the minimum of the acquisition function by randomly
                 # sampling points from the space
-                if self.acq_optimizer == "sampling":
-                    next_x = X[np.argmin(values)]
-
-                elif self.acq_optimizer == "boltzmann_sampling":
-                    p = self.rng.uniform()
-                    if p <= self.boltzmann_psucc:
-                        next_x = X[np.argmin(values)]
-                    else:
-                        values = -values
-
-                        self._min_value = (
-                            self._min_value
-                            if self._min_value is None
-                            else min(values.min(), self._min_value)
-                        )
-                        self._max_value = (
-                            self._max_value
-                            if self._max_value is None
-                            else max(values.max(), self._max_value)
-                        )
-
-                        t = len(self.Xi)
-                        if t == 0:
-                            beta = 0
-                        else:
-                            beta = (
-                                self.boltzmann_gamma
-                                * np.log(t)
-                                / np.abs(self._max_value - self._min_value)
-                            )
-
-                        probs = boltzmann_distribution(values, beta)
-
-                        idx = np.argmax(self.rng.multinomial(1, probs))
-
-                        next_x = X[idx]
+                if do_only_sampling:
+                    next_x = Xsample_transformed[np.argmin(values)]
 
                 # Use BFGS to find the mimimum of the acquisition function, the
                 # minimization starts from `n_restarts_optimizer` different
                 # points and the best minimum is used
                 elif self.acq_optimizer == "lbfgs":
-                    x0 = X[np.argsort(values)[: self.n_restarts_optimizer]]
+                    x0 = Xsample_transformed[
+                        np.argsort(values)[: self.n_restarts_optimizer]
+                    ]
 
                     with warnings.catch_warnings():
                         warnings.simplefilter("ignore")
                         results = Parallel(n_jobs=self.n_jobs)(
                             delayed(fmin_l_bfgs_b)(
                                 gaussian_acquisition_1D,
                                 x,
                                 args=(
                                     est,
                                     np.min(yi),
                                     cand_acq_func,
                                     self.acq_func_kwargs,
+                                    has_gradients(self.base_estimator_),
                                 ),
                                 bounds=transformed_bounds,
-                                approx_grad=False,
+                                # TODO: Use approximated gradient when not available
+                                # approx_grad=False,
+                                approx_grad=not (has_gradients(self.base_estimator_)),
                                 maxiter=20,
                             )
                             for x in x0
                         )
 
                     cand_xs = np.array([r[0] for r in results])
                     cand_acqs = np.array([r[1] for r in results])
                     next_x = cand_xs[np.argmin(cand_acqs)]
 
+                elif self.acq_optimizer == "mixedga":
+                    # TODO: vectorized differential evolution
+                    # https://pymoo.org/customization/mixed.html
+                    # https://pymoo.org/interface/problem.html
+
+                    from pymoo.core.mixed import MixedVariableGA
+                    from pymoo.core.population import Population
+                    from pymoo.optimize import minimize
+                    from pymoo.termination.default import (
+                        DefaultSingleObjectiveTermination,
+                    )
+
+                    from deephyper.skopt.optimizer._pymoo import (
+                        DefaultSingleObjectiveMixedTermination,
+                        PyMOOMixedVectorizedProblem,
+                    )
+
+                    pop = self._pymoo_pop_size
+                    idx_sorted = np.argsort(values)
+                    initial_sampling = [Xsample[i] for i in idx_sorted[:pop]]
+                    initial_sampling = list(
+                        map(
+                            lambda x: dict(zip(self.space.dimension_names, x)),
+                            initial_sampling,
+                        )
+                    )
+                    init_pop = Population.new(
+                        "X",
+                        initial_sampling,
+                        "F",
+                        values[idx_sorted[:pop]].reshape(-1),
+                    )
+
+                    args = (est, np.min(yi), cand_acq_func, False, self.acq_func_kwargs)
+                    problem = PyMOOMixedVectorizedProblem(
+                        space=self.space,
+                        acq_func=lambda x: _gaussian_acquisition(
+                            self.space.transform(x), *args
+                        ),
+                    )
+                    algorithm = MixedVariableGA(pop=pop, sampling=init_pop)
+
+                    res_ga = minimize(
+                        problem,
+                        algorithm,
+                        termination=DefaultSingleObjectiveMixedTermination(
+                            **self._pymoo_termination_kwargs
+                        ),
+                        seed=self.rng.randint(0, np.iinfo(np.int32).max),
+                        verbose=False,
+                    )
+
+                    next_x = [res_ga.X[name] for name in self.space.dimension_names]
+                    next_x = self.space.transform([next_x])[0]
+
+                elif self.acq_optimizer == "ga":
+                    from pymoo.algorithms.soo.nonconvex.ga import GA
+                    from pymoo.core.population import Population
+                    from pymoo.optimize import minimize
+                    from pymoo.termination.default import (
+                        DefaultSingleObjectiveTermination,
+                    )
+
+                    from deephyper.skopt.optimizer._pymoo import PyMOORealProblem
+
+                    xl, xu = list(zip(*transformed_bounds))
+                    xl, xu = np.asarray(xl), np.asarray(xu)
+
+                    args = (est, np.min(yi), cand_acq_func, False, self.acq_func_kwargs)
+                    problem = PyMOORealProblem(
+                        n_var=len(xl),
+                        xl=xl,
+                        xu=xu,
+                        acq_func=lambda x: _gaussian_acquisition(x, *args),
+                    )
+
+                    pop = self._pymoo_pop_size
+                    idx_sorted = np.argsort(values)
+                    initial_sampling = Xsample_transformed[idx_sorted[:pop]]
+                    init_pop = Population.new(
+                        "X",
+                        initial_sampling,
+                        "F",
+                        values[idx_sorted[:pop]].reshape(-1),
+                    )
+
+                    algorithm = GA(pop=pop, sampling=init_pop)
+
+                    res = minimize(
+                        problem,
+                        algorithm,
+                        termination=DefaultSingleObjectiveTermination(
+                            **self._pymoo_termination_kwargs
+                        ),
+                        seed=self.rng.randint(0, np.iinfo(np.int32).max),
+                        verbose=False,
+                    )
+
+                    next_x = res.X
+
+                elif self.acq_optimizer == "cobyqa":
+                    import cobyqa
+
+                    x0 = Xsample_transformed[
+                        np.argsort(values)[: self.n_restarts_optimizer]
+                    ]
+                    xl, xu = list(zip(*transformed_bounds))
+                    args = (est, np.min(yi), cand_acq_func, self.acq_func_kwargs, False)
+
+                    # max_evals: defines the maximum budget but the algorithm stops before (possibly)
+                    # depending on the final radius of the trust-region (input by the user) and the current one
+                    # if the current-radius becomes smaller than the user set radius then the procedure stops
+                    # by default this radius is set to 1e-6
+                    # this stopping criteria relates in spirit to a "xtol" (tolerance on input convergence)
+                    # 2n+1 is the initial number of samples required to fit the trust-region optimaly for COBYQA
+                    #   - option 'npt', (n+1)(n+2)/2 > npt > n+1
+                    with warnings.catch_warnings():
+                        warnings.simplefilter("ignore")
+                        results = Parallel(n_jobs=self.n_jobs)(
+                            delayed(cobyqa.minimize)(
+                                gaussian_acquisition_1D,
+                                x0=x,
+                                args=(
+                                    est,
+                                    np.min(yi),
+                                    cand_acq_func,
+                                    self.acq_func_kwargs,
+                                    False,
+                                ),
+                                xl=xl,
+                                xu=xu,
+                                options={
+                                    "max_eval": 2 * len(self.space.dimension_names)
+                                    + 1
+                                    + 100,
+                                    "scale": True,
+                                },
+                            )
+                            for x in x0
+                        )
+
+                    cand_xs = np.array([r.x for r in results])
+                    cand_acqs = np.array([r.fun for r in results])
+                    next_x = cand_xs[np.argmin(cand_acqs)]
+
                 # lbfgs should handle this but just in case there are
                 # precision errors.
                 if not self.space.is_categorical:
-                    if not self.space.is_config_space:
-                        transformed_bounds = np.asarray(transformed_bounds)
-                        next_x = np.clip(
-                            next_x,
-                            transformed_bounds[:, 0],
-                            transformed_bounds[:, 1],
-                        )
+                    transformed_bounds = np.asarray(transformed_bounds)
+                    next_x = np.clip(
+                        next_x,
+                        transformed_bounds[:, 0],
+                        transformed_bounds[:, 1],
+                    )
 
                 self.next_xs_.append(next_x)
 
-            if self.acq_func == "gp_hedge":
+            if "gp_hedge" in self.acq_func:
                 logits = np.array(self.gains_)
                 logits -= np.max(logits)
                 exp_logits = np.exp(self.eta * logits)
                 probs = exp_logits / np.sum(exp_logits)
                 next_x = self.next_xs_[np.argmax(self.rng.multinomial(1, probs))]
             else:
                 next_x = self.next_xs_[0]
 
             # note the need for [0] at the end
-            self._next_x = self.space.inverse_transform(next_x.reshape((1, -1)))[0]
+            self._next_x = self.space.inverse_transform(next_x.reshape(1, -1))[0]
+            self._counter_fit += 1
 
         # Pack results
         result = create_result(
             self.Xi, self.yi, self.space, self.rng, models=self.models
         )
 
         result.specs = self.specs
```

### Comparing `deephyper-0.6.0/deephyper/skopt/plots.py` & `deephyper-0.7.0/deephyper/skopt/plots.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/sampler/base.py` & `deephyper-0.7.0/deephyper/skopt/sampler/base.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/sampler/grid.py` & `deephyper-0.7.0/deephyper/skopt/sampler/grid.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/sampler/halton.py` & `deephyper-0.7.0/deephyper/skopt/sampler/halton.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/sampler/hammersly.py` & `deephyper-0.7.0/deephyper/skopt/sampler/hammersly.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/sampler/lhs.py` & `deephyper-0.7.0/deephyper/skopt/sampler/lhs.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/sampler/sobol.py` & `deephyper-0.7.0/deephyper/skopt/sampler/sobol.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/searchcv.py` & `deephyper-0.7.0/deephyper/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/space/space.py` & `deephyper-0.7.0/deephyper/skopt/space/space.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numbers
 
 import ConfigSpace as CS
 import numpy as np
+import scipy.stats as ss
 import yaml
 from ConfigSpace.util import deactivate_inactive_hyperparameters
 from scipy.stats import gaussian_kde
-from scipy.stats.distributions import randint, rv_discrete, truncnorm, uniform
-from sklearn.impute import SimpleImputer
 from sklearn.utils import check_random_state
 
 from deephyper.core.utils.joblib_utils import Parallel, delayed
 
 from .transformers import (
     CategoricalEncoder,
     Identity,
@@ -148,15 +147,15 @@
 
     raise ValueError(
         "Invalid dimension {}. Read the documentation for "
         "supported types.".format(dimension)
     )
 
 
-class Dimension(object):
+class Dimension:
     """Base class for search space dimensions."""
 
     prior = None
 
     def rvs(self, n_samples=1, random_state=None):
         """Draw random samples.
 
@@ -218,21 +217,21 @@
             raise ValueError("Dimension's name must be either string or None.")
 
 
 def _uniform_inclusive(loc=0.0, scale=1.0):
     # like scipy.stats.distributions but inclusive of `high`
     # XXX scale + 1. might not actually be a float after scale if
     # XXX scale is very large.
-    return uniform(loc=loc, scale=np.nextafter(scale, scale + 1.0))
+    return ss.uniform(loc=loc, scale=np.nextafter(scale, scale + 1.0))
 
 
 def _normal_inclusive(loc=0.0, scale=1.0, lower=-2, upper=2):
     assert lower <= upper
     a, b = (lower - loc) / scale, (upper - loc) / scale
-    return truncnorm(a, b, loc=loc, scale=scale)
+    return ss.truncnorm(a, b, loc=loc, scale=scale)
 
 
 class Real(Dimension):
     """Search space dimension that can take on any real value.
 
     Parameters
     ----------
@@ -402,18 +401,14 @@
         """Inverse transform samples from the warped space back into the
         original space.
         """
         inv_transform = super(Real, self).inverse_transform(Xt)
         if isinstance(inv_transform, list):
             inv_transform = np.array(inv_transform)
 
-        # PB commenting clip
-        # print(inv_transform)
-        # inv_transform = np.clip(inv_transform, self.low, self.high).astype(self.dtype)
-
         if self.dtype == float or self.dtype == "float":
             # necessary, otherwise the type is converted to a numpy type
             return getattr(inv_transform, "tolist")()
         else:
             return inv_transform
 
     @property
@@ -436,15 +431,18 @@
     def transformed_bounds(self):
         if self.transform_ == "normalize":
             return 0.0, 1.0
         else:
             if self.prior == "uniform":
                 return self.low, self.high
             else:
-                return np.log10(self.low), np.log10(self.high)
+                return (
+                    np.log10(self.low) / self.log_base,
+                    np.log10(self.high) / self.log_base,
+                )
 
     def distance(self, a, b):
         """Compute distance between point `a` and `b`.
 
         Parameters
         ----------
         a : float
@@ -650,15 +648,15 @@
                             np.log10(self.low) / self.log_base,
                             np.log10(self.high) / self.log_base,
                         ),
                     ]
                 )
         else:
             if self.prior == "uniform":
-                self._rvs = randint(self.low, self.high + 1)
+                self._rvs = ss.randint(self.low, self.high + 1)
                 self.transformer = Identity()
             elif self.prior == "normal":
                 self._rvs = _normal_inclusive(self.loc, self.scale, self.low, self.high)
                 self.transformer = ToInteger()
             else:
                 self._rvs = _uniform_inclusive(
                     np.log10(self.low) / self.log_base,
@@ -722,15 +720,18 @@
     def transformed_bounds(self):
         if self.transform_ == "normalize":
             return 0.0, 1.0
         else:
             if self.prior == "uniform":
                 return self.low, self.high
             else:
-                return np.log10(self.low), np.log10(self.high)
+                return (
+                    np.log10(self.low) / self.log_base,
+                    np.log10(self.high) / self.log_base,
+                )
 
     def distance(self, a, b):
         """Compute distance between point `a` and `b`.
 
         Parameters
         ----------
         a : int
@@ -830,15 +831,17 @@
             else:
                 self.transformer = Identity()
             self.transformer.fit(self.categories)
         if transform == "normalize":
             self._rvs = _uniform_inclusive(0.0, 1.0)
         else:
             # XXX check that sum(prior) == 1
-            self._rvs = rv_discrete(values=(range(len(self.categories)), self.prior_))
+            self._rvs = ss.rv_discrete(
+                values=(range(len(self.categories)), self.prior_)
+            )
 
     def __eq__(self, other):
         return (
             type(self) is type(other)
             and self.categories == other.categories
             and np.allclose(self.prior_, other.prior_)
         )
@@ -938,15 +941,15 @@
 
 def _sample_dimension(dim, i, n_samples, random_state, out):
     """Wrapper to sample dimension for joblib parallelization."""
 
     out[0][:, i] = dim.rvs(n_samples=n_samples, random_state=random_state)
 
 
-class Space(object):
+class Space:
     """Initialize a search space from given specifications.
 
     Parameters
     ----------
     dimensions : list, shape=(n_dims,)
         List of search space dimensions.
         Each search dimension can be defined either as
@@ -960,111 +963,22 @@
           `Categorical`).
 
         .. note::
             The upper and lower bounds are inclusive for `Integer`
             dimensions.
     """
 
-    def __init__(self, dimensions, model_sdv=None):
-        # attributes used when a ConfigurationSpace from ConfigSpace is given
-        self.is_config_space = False
-        self.config_space_samples = None
-        self.config_space_explored = False
-
-        self.imp_const = SimpleImputer(
-            missing_values=np.nan, strategy="constant", fill_value=-1000
-        )
-        self.imp_const_inv = SimpleImputer(
-            missing_values=-1000, strategy="constant", fill_value=np.nan
-        )
-
+    def __init__(self, dimensions, model_sdv=None, config_space=None):
         # attribute used when a generative model is used to sample
         self.model_sdv = model_sdv
 
-        self.hps_names = []
+        # attribute use when a config space is used to sample
+        assert config_space is None or isinstance(config_space, CS.ConfigurationSpace)
+        self.config_space = config_space
 
-        if isinstance(dimensions, CS.ConfigurationSpace):
-            self.is_config_space = True
-            self.config_space = dimensions
-            self.hps_type = {}
-
-            hps = self.config_space.get_hyperparameters()
-            cond_hps = self.config_space.get_all_conditional_hyperparameters()
-
-            space = []
-            for x in hps:
-                self.hps_names.append(x.name)
-                if isinstance(x, CS.hyperparameters.CategoricalHyperparameter):
-                    categories = list(x.choices)
-
-                    if x.probabilities is None:
-                        prior = np.ones((len(categories),)) / len(categories)
-                    else:
-                        prior = list(x.probabilities)
-
-                    if x.name in cond_hps:
-                        categories.append("NA")
-
-                        # remove p from prior
-                        p = 1 / len(categories)
-                        pi = p / (len(categories) - 1)
-                        prior = [prior_i - pi for prior_i in prior]
-                        prior.append(p)
-                    param = Categorical(categories, prior=prior, name=x.name)
-                    space.append(param)
-                    self.hps_type[x.name] = "Categorical"
-                elif isinstance(x, CS.hyperparameters.OrdinalHyperparameter):
-                    vals = list(x.sequence)
-                    if x.name in cond_hps:
-                        vals.append("NA")
-                    param = Categorical(vals, name=x.name)
-                    space.append(param)
-                    self.hps_type[x.name] = "Categorical"
-                elif isinstance(x, CS.hyperparameters.UniformIntegerHyperparameter):
-                    prior = "uniform"
-                    if x.log:
-                        prior = "log-uniform"
-                    param = Integer(x.lower, x.upper, prior=prior, name=x.name)
-                    space.append(param)
-                    self.hps_type[x.name] = "Integer"
-                elif isinstance(x, CS.hyperparameters.NormalIntegerHyperparameter):
-                    # TODO
-                    prior = "uniform"
-                    if x.log:
-                        prior = "log-uniform"
-                    param = Integer(x.lower, x.upper, prior=prior, name=x.name)
-                    space.append(param)
-                    self.hps_type[x.name] = "Integer"
-                    # raise ValueError("NormalIntegerHyperparameter not implemented")
-                elif isinstance(x, CS.hyperparameters.UniformFloatHyperparameter):
-                    prior = "uniform"
-                    if x.log:
-                        prior = "log-uniform"
-                    param = Real(x.lower, x.upper, prior=prior, name=x.name)
-                    space.append(param)
-                    self.hps_type[x.name] = "Real"
-                elif isinstance(x, CS.hyperparameters.NormalFloatHyperparameter):
-                    prior = "normal"
-                    if x.log:
-                        raise ValueError(
-                            "Unsupported 'log' transformation for NormalFloatHyperparameter."
-                        )
-                    param = Real(
-                        x.lower,
-                        x.upper,
-                        prior=prior,
-                        name=x.name,
-                        loc=x.mu,
-                        scale=x.sigma,
-                    )
-                    space.append(param)
-                    self.hps_type[x.name] = "Real"
-                else:
-                    raise ValueError("Unknown Hyperparameter type.")
-            dimensions = space
         self.dimensions = [check_dimension(dim) for dim in dimensions]
 
     def __eq__(self, other):
         return all([a == b for a, b in zip(self.dimensions, other.dimensions)])
 
     def __repr__(self):
         if len(self.dimensions) > 31:
@@ -1184,15 +1098,15 @@
         Returns
         -------
         points : list of lists, shape=(n_points, n_dims)
            Points sampled from the space.
         """
 
         rng = check_random_state(random_state)
-        if self.is_config_space:
+        if self.config_space:
             req_points = []
 
             hps_names = self.config_space.get_hyperparameter_names()
 
             if self.model_sdv is None:
                 confs = self.config_space.sample_configuration(n_samples)
 
@@ -1221,20 +1135,21 @@
                 confs = confs.to_dict("records")
                 for idx, conf in enumerate(confs):
                     cf = deactivate_inactive_hyperparameters(conf, self.config_space)
                     confs[idx] = cf.get_dictionary()
 
             for idx, conf in enumerate(confs):
                 point = []
-                for hps_name in hps_names:
-                    val = np.nan
-                    if self.hps_type[hps_name] == "Categorical":
-                        val = "NA"
+                for i, hps_name in enumerate(hps_names):
+                    # If the parameter is inactive due to some conditions then we attribute the
+                    # lower bound value to break symmetries and enforce the same representation.
                     if hps_name in conf.keys():
                         val = conf[hps_name]
+                    else:
+                        val = self.dimensions[i].bounds[0]
                     point.append(val)
                 req_points.append(point)
 
             return req_points
         else:
             if self.model_sdv is None:
                 # Regular sampling without transfer learning from flat search space
@@ -1320,35 +1235,27 @@
 
         Returns
         -------
         Xt : array of floats, shape=(n_samples, transformed_n_dims)
             The transformed samples.
         """
         # Pack by dimension
-        columns = []
-        for dim in self.dimensions:
-            columns.append([])
+        columns = [list() for _ in self.dimensions]
 
         for i in range(len(X)):
             for j in range(self.n_dims):
                 columns[j].append(X[i][j])
 
         # Transform
         for j in range(self.n_dims):
             columns[j] = self.dimensions[j].transform(columns[j])
 
         # Repack as an array
         Xt = np.hstack([np.asarray(c).reshape((len(X), -1)) for c in columns])
 
-        # TODO: old code to be removed
-        # if False and self.is_config_space:
-        #     self.imp_const.fit(Xt)
-        #     Xtt = self.imp_const.transform(Xt)
-        #     Xt = Xtt
-
         return Xt
 
     def inverse_transform(self, Xt):
         """Inverse transform samples from the warped space back to the
            original space.
 
         Parameters
@@ -1358,16 +1265,14 @@
 
         Returns
         -------
         X : list of lists, shape=(n_samples, n_dims)
             The original samples.
         """
 
-        Xt = self.imp_const_inv.fit_transform(Xt)
-
         # Inverse transform
         columns = []
         start = 0
         Xt = np.asarray(Xt)
         for j in range(self.n_dims):
             dim = self.dimensions[j]
             offset = dim.transformed_size
```

### Comparing `deephyper-0.6.0/deephyper/skopt/space/transformers.py` & `deephyper-0.7.0/deephyper/skopt/space/transformers.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/skopt/utils.py` & `deephyper-0.7.0/deephyper/skopt/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,14 @@
 def check_x_in_space(x, space):
     if is_2Dlistlike(x):
         if not np.all([p in space for p in x]):
             raise ValueError("Not all points are within the bounds of" " the space.")
         if any([len(p) != len(space.dimensions) for p in x]):
             raise ValueError("Not all points have the same dimensions as" " the space.")
     elif is_listlike(x):
-        print(x)
         if x not in space:
             raise ValueError(
                 "Point (%s) is not within the bounds of"
                 " the space (%s)." % (x, space.bounds)
             )
         if len(x) != len(space.dimensions):
             raise ValueError(
@@ -472,15 +471,15 @@
         elif generator == "halton":
             generator = Halton()
         elif generator == "hammersly":
             generator = Hammersly()
         elif generator == "lhs":
             generator = Lhs()
         elif generator == "grid":
-            generator = Grid()
+            generator = Grid(border="include")
         elif generator == "random":
             return None
     generator.set_params(**kwargs)
     return generator
 
 
 def dimensions_aslist(search_space):
@@ -614,27 +613,26 @@
         - as a list of categories (for `Categorical` dimensions), or
         - an instance of a `Dimension` object (`Real`, `Integer` or
           `Categorical`).
 
          NOTE: The upper and lower bounds are inclusive for `Integer`
          dimensions.
     """
-    space = Space(dimensions)
     transformed_dimensions = []
-    for dimension in space.dimensions:
+    for dimension in dimensions:
         # check if dimension is of a Dimension instance
         if isinstance(dimension, Dimension):
             # Change the transformer to normalize
             # and add it to the new transformed dimensions
             dimension.set_transformer("normalize")
             transformed_dimensions.append(dimension)
         else:
             raise RuntimeError("Unknown dimension type " "(%s)" % type(dimension))
 
-    return Space(transformed_dimensions)
+    return transformed_dimensions
 
 
 def check_list_types(x, types):
     """
     Check whether all elements of a list `x` are of the correct type(s)
     and raise a ValueError if they are not.
```

### Comparing `deephyper-0.6.0/deephyper/stopper/__init__.py` & `deephyper-0.7.0/deephyper/stopper/__init__.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/stopper/_asha_stopper.py` & `deephyper-0.7.0/deephyper/stopper/_asha_stopper.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         competing_objectives = np.sort(self._get_competiting_objectives())
         num_competing = len(competing_objectives)
 
         if num_competing < self._min_competing:
             return True
 
         # Performe Successive Halving
-        k = num_competing // self._reduction_factor
+        k = int(num_competing // self._reduction_factor)
 
         # Promote if best when there is less than reduction_factor competing values
         if k == 0:
             k = 1
 
         top_k_worst_objective = competing_objectives[-k]
```

### Comparing `deephyper-0.6.0/deephyper/stopper/_const_stopper.py` & `deephyper-0.7.0/deephyper/stopper/_const_stopper.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     """
 
     def __init__(self, max_steps: int, stop_step: int) -> None:
         super().__init__(max_steps)
         self.stop_step = stop_step
 
     def stop(self) -> bool:
-        return super().stop() or self.stop_step <= self.stop_step
+        return super().stop() or self.step >= self.stop_step
```

### Comparing `deephyper-0.6.0/deephyper/stopper/_lcmodel_stopper.py` & `deephyper-0.7.0/deephyper/stopper/_lcmodel_stopper.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,194 +3,315 @@
 from numbers import Number
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import numpyro
 import numpyro.distributions as dist
-from numpyro.infer import MCMC, NUTS
+from numpyro.infer import MCMC, NUTS, BarkerMH
 from scipy.optimize import least_squares
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.utils import check_random_state
 from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 
 from deephyper.stopper._stopper import Stopper
 
 
-# Budget allocation models
-def b_lin2(z, nu=[1, 1]):
-    return nu[1] * (z - 1) + nu[0]
-
-
-def b_exp2(z, nu=[1, 2]):
-    return nu[0] * jnp.power(nu[1], z - 1)
-
-
 # Learning curves models
-def f_lin2(z, b, rho):
-    return rho[1] * b(z) + rho[0]
-
-
-def f_loglin2(z, b, rho):
-    Z = jnp.log(b(z))
-    Y = rho[1] * Z + rho[0]
-    y = jnp.exp(Y)
-    return -y
-
-
-def f_loglin3(z, b, rho):
-    Z = jnp.log(b(z))
-    Y = rho[2] * jnp.power(Z, 2) + rho[1] * Z + rho[0]
-    y = jnp.exp(Y)
-    return -y
-
+@jax.jit
+def f_lin2(z, rho):
+    return rho[1] * z + rho[0]
 
-def f_loglin4(z, b, rho):
-    Z = jnp.log(b(z))
-    Y = rho[3] * jnp.power(Z, 3) + rho[2] * jnp.power(Z, 2) + rho[1] * Z + rho[0]
-    y = jnp.exp(Y)
-    return -y
 
+@jax.jit
+def f_pow3(z, rho):
+    return rho[0] - rho[1] * z ** rho[2]
 
-def f_pow3(z, b, rho):
-    return rho[0] - rho[1] * b(z) ** -rho[2]
 
-
-def f_mmf4(z, b, rho):
-    return (rho[0] * rho[1] + rho[2] * jnp.power(b(z), rho[3])) / (
-        rho[1] + jnp.power(b(z), rho[3])
+@jax.jit
+def f_mmf4(z, rho):
+    return (rho[0] * rho[1] + rho[2] * jnp.power(z, rho[3])) / (
+        rho[1] + jnp.power(z, rho[3])
     )
 
 
-def f_vapor3(z, b, rho):
-    return rho[0] + rho[1] / b(z) + rho[2] * np.log(b(z))
+@jax.jit
+def f_vapor3(z, rho):
+    return rho[0] + rho[1] / z + rho[2] * np.log(z)
 
 
-def f_logloglin2(z, b, rho):
-    return jnp.log(rho[0] * jnp.log(b(z)) + rho[1])
+@jax.jit
+def f_logloglin2(z, rho):
+    return jnp.log(rho[0] * jnp.log(z) + rho[1])
 
 
-def f_hill3(z, b, rho):
+@jax.jit
+def f_hill3(z, rho):
     ymax, eta, kappa = rho
-    return ymax * (b(z) ** eta) / (kappa * eta + b(z) ** eta)
+    return ymax * (z**eta) / (kappa * eta + z**eta)
+
+
+@jax.jit
+def f_logpow3(z, rho):
+    return rho[0] / (1 + (z / jnp.exp(rho[1])) ** rho[2])
 
 
-def f_logpow3(z, b, rho):
-    return rho[0] / (1 + (b(z) / jnp.exp(rho[1])) ** rho[2])
+@jax.jit
+def f_pow4(z, rho):
+    return rho[2] - (rho[0] * z + rho[1]) ** (-rho[3])
 
 
-def f_pow4(z, b, rho):
-    return rho[2] - (rho[0] * b(z) + rho[1]) ** (-rho[3])
+@jax.jit
+def f_exp4(z, rho):
+    return rho[2] - jnp.exp(-rho[0] * (z ** rho[3]) + rho[1])
 
 
-def f_exp4(z, b, rho):
-    return rho[2] - jnp.exp(-rho[0] * (b(z) ** rho[3]) + rho[1])
+@jax.jit
+def f_janoschek4(z, rho):
+    return rho[0] - (rho[0] - rho[1]) * jnp.exp(-rho[2] * (z ** rho[3]))
 
 
-def f_janoschek4(z, b, rho):
-    return rho[0] - (rho[0] - rho[1]) * jnp.exp(-rho[2] * (b(z) ** rho[3]))
+@jax.jit
+def f_weibull4(z, rho):
+    return rho[0] - (rho[0] - rho[1]) * jnp.exp(-((rho[2] * z) ** rho[3]))
 
 
-def f_weibull4(z, b, rho):
-    return rho[0] - (rho[0] - rho[1]) * jnp.exp(-((rho[2] * b(z)) ** rho[3]))
+@jax.jit
+def f_ilog2(z, rho):
+    return rho[1] - (rho[0] / jnp.log(z + 1))
 
 
-def f_ilog2(z, b, rho):
-    return rho[1] - (rho[0] / jnp.log(b(z) + 1))
+@jax.jit
+def f_arctan3(z, rho):
+    return 2 / jnp.pi * jnp.arctan(rho[0] * jnp.pi / 2 * z + rho[1]) - rho[2]
 
 
 # Utility to estimate parameters of learning curve model
 # The combination of "partial" and "static_argnums" is necessary
 # with the "f" lambda function passed as argument
 @partial(jax.jit, static_argnums=(1,))
 def residual_least_square(rho, f, z, y):
     """Residual for least squares."""
-    return f(z, rho) - y
+    y_pred = f(z, rho)
+    y_pred = jnp.where(y_pred == 0.0, y_pred, 0.0)
+    return y_pred - y
+
+
+@partial(jax.jit, static_argnums=(1,))
+def jac_residual_least_square(rho, f, z, y):
+    """Jacobian of the residual for least squares."""
+    return jax.jacfwd(residual_least_square, argnums=0)(rho, f, z, y)
+
+
+def fit_learning_curve_model_least_square(
+    z_train,
+    y_train,
+    f_model,
+    f_model_nparams,
+    max_trials_ls_fit=10,
+    random_state=None,
+    verbose=0,
+):
+    """The learning curve model is assumed to be modeled by 'f' with
+    interface f(z, rho).
+    """
+
+    random_state = check_random_state(random_state)
+
+    results = []
+    mse_hist = []
 
+    rho_init = np.zeros((f_model_nparams,))
 
-def prob_model(z=None, y=None, f=None, rho_mu_prior=None, num_obs=None):
-    rho_mu_prior = jnp.array(rho_mu_prior)
-    rho_sigma_prior = 1.0
+    for i in range(max_trials_ls_fit):
+        if verbose:
+            print(f"Least-Square fit - trial {i+1}/{max_trials_ls_fit}: ", end="")
+
+        rho_init[:] = random_state.randn(f_model_nparams)[:]
+
+        try:
+            res_lsq = least_squares(
+                residual_least_square,
+                rho_init,
+                args=(f_model, z_train, y_train),
+                method="lm" if len(z_train) >= f_model_nparams else "trf",
+                jac=jac_residual_least_square,
+            )
+        except ValueError:
+            continue
+
+        mse_res_lsq = np.mean(res_lsq.fun**2)
+        mse_hist.append(mse_res_lsq)
+        results.append(res_lsq.x)
+
+        if verbose:
+            print(f"mse={mse_res_lsq:.3f}")
+
+        if mse_res_lsq < 1e-8:
+            break
+
+    i_best = np.nanargmin(mse_hist)
+    res = results[i_best]
+    return res
+
+
+def prob_model(
+    z,
+    y,
+    f=None,
+    rho_mu_prior=None,
+    rho_sigma_prior=1.0,
+    y_sigma_prior=1.0,
+    num_obs=None,
+):
     rho = numpyro.sample("rho", dist.Normal(rho_mu_prior, rho_sigma_prior))
-    sigma = numpyro.sample("sigma", dist.Exponential(1.0))  # introducing noise
-    # sigma = 0.1
-    mu = f(z[:num_obs], rho)
-    numpyro.sample("obs", dist.Normal(mu, sigma), obs=y[:num_obs])
+    y_sigma = numpyro.sample(
+        "sigma", dist.Exponential(y_sigma_prior)
+    )  # introducing noise
+    y_mu = f(z[:num_obs], rho)
+    numpyro.sample("obs", dist.Normal(y_mu, y_sigma), obs=y[:num_obs])
 
 
 @partial(jax.jit, static_argnums=(0,))
 def predict_moments_from_posterior(f, X, posterior_samples):
     vf_model = jax.vmap(f, in_axes=(None, 0))
     posterior_mu = vf_model(X, posterior_samples)
     mean_mu = jnp.mean(posterior_mu, axis=0)
     std_mu = jnp.std(posterior_mu, axis=0)
     return mean_mu, std_mu
 
 
 class BayesianLearningCurveRegressor(BaseEstimator, RegressorMixin):
+    """Probabilistic model for learning curve regression.
+
+    Args:
+        f_model (callable, optional): The model function to use. Defaults to `f_power3` for a Power-Law with 3 parameters.
+        f_model_nparams (int, optional): The number of parameters of the model. Defaults to `3`.
+        max_trials_ls_fit (int, optional): The number of least-square fits that should be tried. Defaults to `10`.
+        mcmc_kernel (str, optional): The MCMC kernel to use. It should be a string in the following list: `["NUTS", "BarkerMH"]`. Defaults to `"NUTS"`.
+        mcmc_num_warmup (int, optional): The number of warmup steps in MCMC. Defaults to `200`.
+        mcmc_num_samples (int, optional): The number of samples in MCMC. Defaults to `1_000`.
+        random_state (int, optional): A random state. Defaults to `None`.
+        verbose (int, optional): Wether or not to use the verbose mode. Defaults to `0` to deactive it.
+        batch_size (int, optional): The expected maximum length of the X, y arrays (used in the `fit(X, y)` method) in order to preallocate memory and compile the code only once. Defaults to `100`.
+        min_max_scaling (bool, optional): Wether or not to use min-max scaling in [0,1] for `y` values. Defaults to False.
+    """
+
     def __init__(
         self,
-        f_model=f_loglin3,
-        f_model_num_params=3,
-        b_model=b_lin2,
+        f_model=f_pow3,
+        f_model_nparams=3,
         max_trials_ls_fit=10,
+        mcmc_kernel="NUTS",
+        mcmc_num_chains=1,
         mcmc_num_warmup=200,
         mcmc_num_samples=1_000,
-        n_jobs=-1,
         random_state=None,
         verbose=0,
-        batch_size=100,
+        batch_size=1_000,
+        min_max_scaling=False,
     ):
-        self.b_model = b_model
-        self.f_model = lambda z, rho: f_model(z, self.b_model, rho)
-        self.f_nparams = f_model_num_params
+        self.f_model = f_model
+        self.f_model_nparams = f_model_nparams
+        self.mcmc_kernel = mcmc_kernel
+        self.mcmc_num_chains = mcmc_num_chains
         self.mcmc_num_warmup = mcmc_num_warmup
         self.mcmc_num_samples = mcmc_num_samples
         self.max_trials_ls_fit = max_trials_ls_fit
-        self.n_jobs = n_jobs
         self.random_state = check_random_state(random_state)
         self.verbose = verbose
-        self.rho_mu_prior_ = np.zeros((self.f_nparams,))
+        self.rho_mu_prior_ = np.zeros((self.f_model_nparams,))
 
         self.batch_size = batch_size
         self.X_ = np.zeros((self.batch_size,))
         self.y_ = np.zeros((self.batch_size,))
 
+        self.min_max_scaling = min_max_scaling
+
     def fit(self, X, y, update_prior=True):
         check_X_y(X, y, ensure_2d=False)
 
         # !Trick for performance to avoid performign JIT again and again
         # !This will fix the shape of inputs of the model for numpyro
         # !see https://github.com/pyro-ppl/numpyro/issues/441
         num_samples = len(X)
         assert num_samples <= self.batch_size
         self.X_[:num_samples] = X[:]
         self.y_[:num_samples] = y[:]
+        self.X_[num_samples:] = 0.0
+        self.y_[num_samples:] = 0.0
+
+        # Min-Max Scaling
+        if not (self.min_max_scaling):
+            self.y_min_ = 0
+            self.y_max_ = 1
+        else:
+            self.y_min_ = self.y_[:num_samples].min()
+            self.y_max_ = self.y_[:num_samples].max()
+            if abs(self.y_min_ - self.y_max_) <= 1e-8:  # avoid division by zero
+                self.y_max_ = self.y_min_ + 1
+            self.y_[:num_samples] = (self.y_[:num_samples] - self.y_min_) / (
+                self.y_max_ - self.y_min_
+            )
 
         if update_prior:
-            self.rho_mu_prior_[:] = self._fit_learning_curve_model_least_square(X, y)[:]
+            self.rho_mu_prior_[:] = fit_learning_curve_model_least_square(
+                self.X_,
+                self.y_,
+                f_model=self.f_model,
+                f_model_nparams=self.f_model_nparams,
+                max_trials_ls_fit=self.max_trials_ls_fit,
+                random_state=self.random_state,
+                verbose=self.verbose,
+            )[:]
+
+            if self.verbose:
+                print(f"rho_mu_prior: {self.rho_mu_prior_}")
 
         if not (hasattr(self, "kernel_")):
-            self.kernel_ = NUTS(
-                model=lambda z, y, rho_mu_prior: prob_model(
-                    z, y, self.f_model, rho_mu_prior, num_obs=num_samples
-                ),
-            )
+            target_accept_prob = 0.8
+            step_size = 0.05
+            if self.mcmc_kernel == "NUTS":
+                self.kernel_ = NUTS(
+                    model=lambda z, y: prob_model(
+                        z,
+                        y,
+                        f=self.f_model,
+                        rho_mu_prior=self.rho_mu_prior_,
+                        num_obs=num_samples,
+                    ),
+                    target_accept_prob=target_accept_prob,
+                    step_size=step_size,
+                )
+            elif self.mcmc_kernel == "BarkerMH":
+                self.kernel_ = BarkerMH(
+                    model=lambda z, y: prob_model(
+                        z,
+                        y,
+                        f=self.f_model,
+                        rho_mu_prior=self.rho_mu_prior_,
+                        num_obs=num_samples,
+                    ),
+                    target_accept_prob=target_accept_prob,
+                    step_size=step_size,
+                )
+            else:
+                raise ValueError(f"Unknown MCMC kernel: {self.mcmc_kernel}")
 
             self.mcmc_ = MCMC(
                 self.kernel_,
+                num_chains=self.mcmc_num_chains,
                 num_warmup=self.mcmc_num_warmup,
                 num_samples=self.mcmc_num_samples,
                 progress_bar=self.verbose,
-                jit_model_args=True,
             )
 
         seed = self.random_state.randint(low=0, high=2**31)
         rng_key = jax.random.PRNGKey(seed)
-        self.mcmc_.run(rng_key, z=self.X_, y=self.y_, rho_mu_prior=self.rho_mu_prior_)
+        self.mcmc_.run(rng_key, z=self.X_, y=self.y_)
 
         if self.verbose:
             self.mcmc_.print_summary()
 
         return self
 
     def predict(self, X, return_std=True):
@@ -211,97 +332,36 @@
         # Input validation
         X = check_array(X, ensure_2d=False)
 
         posterior_samples = self.mcmc_.get_samples()
         vf_model = jax.vmap(self.f_model, in_axes=(None, 0))
         posterior_mu = vf_model(X, posterior_samples["rho"])
 
+        # Inverse Min-Max Scaling
+        posterior_mu = posterior_mu * (self.y_max_ - self.y_min_) + self.y_min_
+
         return posterior_mu
 
     def prob(self, X, condition):
         """Compute the approximate probability of P(cond(m(X_i), y_i))
         where m is the current fitted model and cond a condition.
 
         Args:
             X (np.array): An array of inputs.
             condition (callable): A function defining the condition to test.
 
         Returns:
             array: an array of shape X.
         """
-
-        # Check if fit has been called
-        check_is_fitted(self)
-
-        # Input validation
-        X = check_array(X, ensure_2d=False)
-
-        posterior_samples = self.mcmc_.get_samples()
-        vf_model = jax.vmap(self.f_model, in_axes=(None, 0))
-        posterior_mu = vf_model(X, posterior_samples["rho"])
+        posterior_mu = self.predict_posterior_samples(X)
 
         prob = jnp.mean(condition(posterior_mu), axis=0)
 
         return prob
 
-    def _fit_learning_curve_model_least_square(
-        self,
-        z_train,
-        y_train,
-    ):
-        """The learning curve model is assumed to be modeled by 'f' with
-        interface f(z, rho).
-        """
-
-        seed = self.random_state.randint(low=0, high=2**31)
-        random_state = check_random_state(seed)
-
-        z_train = np.asarray(z_train)
-        y_train = np.asarray(y_train)
-
-        # compute the jacobian
-        # using the true jacobian is important to avoid problems
-        # with numerical errors and approximations! indeed the scale matters
-        # a lot when approximating with finite differences
-        def fun_wrapper(rho, f, z, y):
-            return np.array(residual_least_square(rho, f, z, y))
-
-        if not (hasattr(self, "jac_residual_ls_")):
-            self.jac_residual_ls_ = partial(jax.jit, static_argnums=(1,))(
-                jax.jacfwd(residual_least_square, argnums=0)
-            )
-
-        def jac_wrapper(rho, f, z, y):
-            return np.array(self.jac_residual_ls_(rho, f, z, y))
-
-        results = []
-        mse_hist = []
-
-        for _ in range(self.max_trials_ls_fit):
-            rho_init = random_state.randn(self.f_nparams)
-
-            try:
-                res_lsq = least_squares(
-                    fun_wrapper,
-                    rho_init,
-                    args=(self.f_model, z_train, y_train),
-                    method="lm",
-                    jac=jac_wrapper,
-                )
-            except ValueError:
-                continue
-
-            mse_res_lsq = np.mean(res_lsq.fun**2)
-            mse_hist.append(mse_res_lsq)
-            results.append(res_lsq.x)
-
-        i_best = np.nanargmin(mse_hist)
-        res = results[i_best]
-        return res
-
 
 def area_learning_curve(z, f, z_max) -> float:
     assert len(z) == len(f)
     assert z[-1] <= z_max
     area = 0
     for i in range(1, len(z)):
         # z: is always monotinic increasing but not f!
@@ -339,15 +399,15 @@
     .. code-block:: bash
 
         $ jax>=0.3.25
         $ numpyro
 
     Args:
         max_steps (int): The maximum number of training steps which can be performed.
-        min_steps (int, optional): The minimum number of training steps which can be performed. Defaults to ``1``.
+        min_steps (int, optional): The minimum number of training steps which can be performed. Defaults to ``4``. It is better to have at least as many steps as the number of parameters of the fitted learning curve model. For example, if ``lc_model="mmf4"`` then ``min_steps`` should be at least ``4``.
         lc_model (str, optional): The parameteric learning model to use. It should be a string in the following list: ``["lin2", "loglin2", "loglin3", "loglin4", "pow3","mmf4", "vapor3", "logloglin2", "hill3", "logpow3", "pow4", "exp4", "janoschek4", "weibull4", "ilog2"]``. The number in the name corresponds to the number of parameters of the parametric model. Defaults to ``"mmf4"``.
         min_done_for_outlier_detection (int, optional): The minimum number of observed scores at the same step to check for if it is a lower-bound outlier. Defaults to ``10``.
         iqr_factor_for_outlier_detection (float, optional): The IQR factor for outlier detection. The higher it is the more inclusive the condition will be (i.e. if set very large it is likely not going to detect any outliers). Defaults to ``1.5``.
         prob_promotion (float, optional): The threshold probabily to stop the iterations. If the current learning curve has a probability greater than ``prob_promotion`` to be worse that the best observed score accross all evaluations then the current iterations are stopped. Defaults to ``0.9`` (i.e. probability of 0.9 of being worse).
         early_stopping_patience (float, optional): The patience of the early stopping condition. If it is an ``int`` it is directly corresponding to a number of iterations. If it is a ``float`` then it is corresponding to a proportion between [0,1] w.r.t. ``max_steps``. Defaults to ``0.25`` (i.e. 25% of ``max_steps``).
         objective_returned (str, optional): The returned objective. It can be a value in ``["last", "max", "alc"]`` where ``"last"`` corresponds to the last observed score, ``"max"`` corresponds to the maximum observed score and ``"alc"`` corresponds to the area under the learning curve. Defaults to "last".
         random_state (int or np.RandomState, optional): The random state of estimation process. Defaults to ``None``.
@@ -357,28 +417,31 @@
     """
 
     def __init__(
         self,
         max_steps: int,
         min_steps: int = 1,
         lc_model="mmf4",
+        min_obs_to_fit_lc_model=4,
         min_done_for_outlier_detection=10,
         iqr_factor_for_outlier_detection=1.5,
         prob_promotion=0.9,
         early_stopping_patience=0.25,
+        reduction_factor=3,
         objective_returned="last",
         random_state=None,
     ) -> None:
         super().__init__(max_steps=max_steps)
         self.min_steps = min_steps
 
         lc_model = "f_" + lc_model
-        lc_model_num_params = int(lc_model[-1])
-        lc_model = getattr(sys.modules[__name__], lc_model)
-        self.min_obs_to_fit = lc_model_num_params
+        self._f_model = getattr(sys.modules[__name__], lc_model)
+        self._f_model_nparams = int(lc_model[-1])
+        self._min_obs_to_fit_lc_model = min_obs_to_fit_lc_model
+        self._reduction_factor = reduction_factor
 
         self.min_done_for_outlier_detection = min_done_for_outlier_detection
         self.iqr_factor_for_outlier_detection = iqr_factor_for_outlier_detection
 
         self.prob_promotion = prob_promotion
         if type(early_stopping_patience) is int:
             self.early_stopping_patience = early_stopping_patience
@@ -386,31 +449,36 @@
             self.early_stopping_patience = int(early_stopping_patience * self.max_steps)
         else:
             raise ValueError("early_stopping_patience must be int or float")
         self.objective_returned = objective_returned
 
         self._rung = 0
 
-        # compute the step at which to stop based on steps allocation policy
-        max_rung = np.floor(
-            np.log(self.max_steps / self.min_steps) / np.log(self.min_obs_to_fit)
-        )
-        self.max_steps_ = int(self.min_steps * self.min_obs_to_fit**max_rung)
-
-        self.lc_model = BayesianLearningCurveRegressor(
-            f_model=lc_model,
-            f_model_num_params=lc_model_num_params,
-            random_state=random_state,
-            batch_size=self.max_steps_,
-        )
+        self._random_state = random_state
+        self._batch_size = 100
+        self.lc_model = None
 
         self._lc_objectives = []
 
+    def _refresh_lc_model(self):
+        batch_has_increased = False
+        if self._batch_size < len(self.observed_budgets):
+            self._batch_size += 100
+            batch_has_increased = True
+
+        if self.lc_model is None or batch_has_increased:
+            self.lc_model = BayesianLearningCurveRegressor(
+                f_model=self._f_model,
+                f_model_nparams=self._f_model_nparams,
+                random_state=self._random_state,
+                batch_size=self._batch_size,
+            )
+
     def _compute_halting_step(self):
-        return self.min_steps * self.min_obs_to_fit**self._rung
+        return (self.min_steps - 1) * self._reduction_factor**self._rung
 
     def _retrieve_best_objective(self) -> float:
         search_id, _ = self.job.id.split(".")
         objectives = []
 
         for obj in self.job.storage.load_out_from_all_jobs(search_id):
             if isinstance(obj, Number):
@@ -462,15 +530,21 @@
 
         # This condition will enforce the stopper to stop the evaluation at the first step
         # for the first evaluation (The FABOLAS method does the same, bias the first samples with
         # small budgets)
         self.best_objective = self._retrieve_best_objective()
 
         halting_step = self._compute_halting_step()
-        if self.step < max(self.min_steps, self.min_obs_to_fit):
+
+        if self.step < self.min_steps:
+            if self.step >= halting_step:
+                self._rung += 1
+            return False
+
+        if self.step < self._min_obs_to_fit_lc_model:
             if self.step >= halting_step:
                 competing_objectives = self._get_competiting_objectives(self._rung)
                 if len(competing_objectives) > self.min_done_for_outlier_detection:
                     q1 = np.quantile(
                         competing_objectives,
                         q=0.25,
                     )
@@ -493,14 +567,16 @@
         # Check if the halting budget condition is met
         if self.step < halting_step:
             return False
 
         # Check if the evaluation should be stopped based on LC-Model
 
         # Fit and predict the performance of the learning curve model
+        self._refresh_lc_model()
+
         z_train = self.observed_budgets
         y_train = self._lc_objectives
         z_train, y_train = np.asarray(z_train), np.asarray(y_train)
         self.lc_model.fit(z_train, y_train, update_prior=True)
 
         # Check if the configuration is promotable based on its predicted objective value
         p = self.lc_model.prob(
@@ -522,7 +598,58 @@
         elif self.objective_returned == "max":
             return max(self.observations[-1])
         elif self.objective_returned == "alc":
             z, y = self.observations
             return area_learning_curve(z, y, z_max=self.max_steps)
         else:
             raise ValueError("objective_returned must be one of 'last', 'best', 'alc'")
+
+
+def test_bayesian_lce_model():
+    import cProfile
+    from pstats import SortKey
+
+    import time
+    import matplotlib.pyplot as plt
+    import numpy as np
+
+    def f(z):
+        return f_pow3(z, [1, -1, 0.125])
+
+    z = np.arange(1, 1000)
+
+    y = f(z)
+    # y = y + rng.normal(0, 0.01, size=y.shape)
+
+    t_start = time.time()
+    with cProfile.Profile() as pr:
+        for r in range(20):
+            model = BayesianLearningCurveRegressor(batch_size=100, verbose=0)
+            for i in range(1, 20):
+                model.fit(z[:i], y[:i])
+                y_pred, y_std = model.predict(z)
+                y_min, y_max = y_pred - y_std, y_pred + y_std
+
+        pr.print_stats(SortKey.TIME)
+
+    t_end = time.time()
+    duration = t_end - t_start
+
+    print(f"duration: {duration:.3f} sec")
+
+    plt.figure()
+    plt.plot(z, y, label="f_pow3")
+    plt.plot(z, y_pred, label="$\\hat{y}$", color="C2")
+    plt.fill_between(z, y_min, y_max, color="C2", alpha=0.5)
+    plt.legend()
+    plt.show()
+
+
+# if __name__ == "__main__":
+#     test_bayesian_lce_model()
+#     rho = np.ones((3,))
+#     z = np.arange(1000)
+#     y = np.zeros((1000,))
+
+#     out = jac_residual_least_square(rho, f_pow3, z, y)
+#     out = jac_residual_least_square(rho, f_pow3, z, y)
+#     out = jac_residual_least_square(rho, f_pow3, z, y)
```

### Comparing `deephyper-0.6.0/deephyper/stopper/_median_stopper.py` & `deephyper-0.7.0/deephyper/stopper/_median_stopper.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/stopper/_stopper.py` & `deephyper-0.7.0/deephyper/stopper/_stopper.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/stopper/integration/deepxde.py` & `deephyper-0.7.0/deephyper/stopper/integration/deepxde.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/stopper/integration/tensorflow.py` & `deephyper-0.7.0/deephyper/stopper/integration/tensorflow.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/_command.py` & `deephyper-0.7.0/deephyper/test/_command.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearReg/load_data.py` & `deephyper-0.7.0/deephyper/test/nas/linearReg/load_data.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearReg/problem.py` & `deephyper-0.7.0/deephyper/test/nas/linearReg/problem.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearRegHybrid/load_data.py` & `deephyper-0.7.0/deephyper/test/nas/linearRegHybrid/load_data.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearRegHybrid/problem.py` & `deephyper-0.7.0/deephyper/test/nas/linearRegHybrid/problem.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputs/load_data.py` & `deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputs/load_data.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputs/problem.py` & `deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputs/problem.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputsGen/load_data.py` & `deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputsGen/load_data.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper/test/nas/linearRegMultiInputsGen/problem.py` & `deephyper-0.7.0/deephyper/test/nas/linearRegMultiInputsGen/problem.py`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/deephyper.egg-info/SOURCES.txt` & `deephyper-0.7.0/deephyper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 deephyper.egg-info/PKG-INFO
 deephyper.egg-info/SOURCES.txt
 deephyper.egg-info/dependency_links.txt
 deephyper.egg-info/entry_points.txt
 deephyper.egg-info/requires.txt
 deephyper.egg-info/top_level.txt
 deephyper/analysis/__init__.py
+deephyper/analysis/_matplotlib.py
+deephyper/analysis/_paxplot.py
 deephyper/analysis/_rank.py
 deephyper/analysis/hpo.py
 deephyper/core/__init__.py
 deephyper/core/parser.py
 deephyper/core/analytics/__init__.py
 deephyper/core/analytics/_analytics.py
 deephyper/core/analytics/_dashboard.py
@@ -126,14 +128,15 @@
 deephyper/problem/__init__.py
 deephyper/problem/_hyperparameter.py
 deephyper/problem/_neuralarchitecture.py
 deephyper/search/__init__.py
 deephyper/search/_search.py
 deephyper/search/hps/__init__.py
 deephyper/search/hps/_cbo.py
+deephyper/search/hps/_eds.py
 deephyper/search/hps/_mpi_dbo.py
 deephyper/search/nas/__init__.py
 deephyper/search/nas/_agebo.py
 deephyper/search/nas/_ambsmixed.py
 deephyper/search/nas/_base.py
 deephyper/search/nas/_random.py
 deephyper/search/nas/_regevo.py
@@ -163,14 +166,15 @@
 deephyper/skopt/learning/tests/test_forest.py
 deephyper/skopt/learning/tests/test_gbrt.py
 deephyper/skopt/moo/__init__.py
 deephyper/skopt/moo/_hv.py
 deephyper/skopt/moo/_multiobjective.py
 deephyper/skopt/moo/_pf.py
 deephyper/skopt/optimizer/__init__.py
+deephyper/skopt/optimizer/_pymoo.py
 deephyper/skopt/optimizer/base.py
 deephyper/skopt/optimizer/dummy.py
 deephyper/skopt/optimizer/forest.py
 deephyper/skopt/optimizer/gbrt.py
 deephyper/skopt/optimizer/gp.py
 deephyper/skopt/optimizer/optimizer.py
 deephyper/skopt/sampler/__init__.py
```

### Comparing `deephyper-0.6.0/deephyper.egg-info/requires.txt` & `deephyper-0.7.0/deephyper.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 dm-tree
 Jinja2<3.1
 numpy>=1.20
 pandas>=0.24.2
 packaging
 parse
 scikit-learn>=0.23.1
-scipy>=1.7
+scipy>=1.10
 tqdm>=4.64.0
+pymoo>=0.6.0
 pyyaml
 
 [analytics]
 altair
 jupyter
 jupyter_contrib_nbextensions>=0.5.1
 nbconvert<6
@@ -34,16 +35,17 @@
 dm-tree
 Jinja2<3.1
 numpy>=1.20
 pandas>=0.24.2
 packaging
 parse
 scikit-learn>=0.23.1
-scipy>=1.7
+scipy>=1.10
 tqdm>=4.64.0
+pymoo>=0.6.0
 pyyaml
 networkx
 pydot
 tensorflow>=2.0.0
 tensorflow_probability
 ray[default]>=1.3.0
 sdv>=0.17.1
@@ -94,8 +96,11 @@
 tensorflow>=2.0.0
 tensorflow_probability
 
 [ray]
 ray[default]>=1.3.0
 
 [redis]
+redis
+
+[redis-hiredis]
 redis[hiredis]
```

### Comparing `deephyper-0.6.0/setup.cfg` & `deephyper-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `deephyper-0.6.0/setup.py` & `deephyper-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 platform_infos = platform.platform()
 
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "ConfigSpace>=0.4.20",
     "dm-tree",
-    "Jinja2<3.1",
-    "numpy>=1.20",  # ==1.19.4",  # working with 1.20.1
+    "Jinja2<3.1",  # TODO: Check vulnerability issue
+    "numpy>=1.20",
     "pandas>=0.24.2",
     "packaging",
     "parse",
     "scikit-learn>=0.23.1",
-    "scipy>=1.7",
+    "scipy>=1.10",
     "tqdm>=4.64.0",
+    "pymoo>=0.6.0",
     "pyyaml",
 ]
 
 
 # !Requirements for Neural Architecture Search (NAS)
 REQUIRED_NAS = ["networkx", "pydot"]
 
@@ -63,15 +64,16 @@
     "jax-cpu": ["jax[cpu]>=0.3.25", "numpyro[cpu]"],
     "jax-cuda": ["jax[cuda]>=0.3.25", "numpyro[cuda]"],
     "hps": [],  # hyperparameter search (already the base requirements)
     "nas": REQUIRED_NAS,  # neural architecture search
     "hps-tl": REQUIRED_TL_SDV,  # transfer learning for bayesian optimization,
     "mpi": ["mpi4py>=3.1.3"],
     "ray": ["ray[default]>=1.3.0"],
-    "redis": ["redis[hiredis]"],
+    "redis": ["redis"],
+    "redis-hiredis": ["redis[hiredis]"],
     "dev": [
         # Test
         "pytest",
         # Packaging
         "twine",
         # Formatter and Linter
         "black==22.6.0",
```

### Comparing `deephyper-0.6.0/tests/test_quickstart.py` & `deephyper-0.7.0/tests/test_quickstart.py`

 * *Files identical despite different names*

