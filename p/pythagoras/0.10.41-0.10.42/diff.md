# Comparing `tmp/pythagoras-0.10.41.tar.gz` & `tmp/pythagoras-0.10.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythagoras-0.10.41.tar", last modified: Thu Apr  4 04:20:51 2024, max compression
+gzip compressed data, was "pythagoras-0.10.42.tar", last modified: Thu Apr  4 05:18:43 2024, max compression
```

## Comparing `pythagoras-0.10.41.tar` & `pythagoras-0.10.42.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.983433 pythagoras-0.10.41/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1114 2023-12-24 04:46:00.000000 pythagoras-0.10.41/LICENSE
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-04 04:20:51.982951 pythagoras-0.10.41/PKG-INFO
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-04-04 02:44:15.000000 pythagoras-0.10.41/README.md
--rw-r--r--   0 Pythagoras   (504) staff       (20)       80 2023-12-24 04:46:00.000000 pythagoras-0.10.41/pyproject.toml
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.959276 pythagoras-0.10.41/pythagoras/
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.962273 pythagoras-0.10.41/pythagoras/_01_foundational_objects/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      792 2024-03-23 20:14:41.000000 pythagoras-0.10.41/pythagoras/_01_foundational_objects/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1239 2024-02-22 05:34:39.000000 pythagoras-0.10.41/pythagoras/_01_foundational_objects/base_16_32_convertors.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3341 2024-03-17 06:20:02.000000 pythagoras-0.10.41/pythagoras/_01_foundational_objects/hash_addresses.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1510 2024-03-10 05:40:41.000000 pythagoras-0.10.41/pythagoras/_01_foundational_objects/hash_and_random_signatures.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      720 2024-03-10 19:35:01.000000 pythagoras-0.10.41/pythagoras/_01_foundational_objects/multipersidict.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2611 2024-03-17 06:40:19.000000 pythagoras-0.10.41/pythagoras/_01_foundational_objects/value_addresses.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.964701 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      908 2024-03-17 06:16:19.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1894 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/assert_ordinarity.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      815 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/check_n_positional_args.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      723 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/code_normalizer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4595 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      400 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/function_name.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      288 2024-03-16 20:40:58.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/ordinary_decorator.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1469 2024-03-17 05:40:33.000000 pythagoras-0.10.41/pythagoras/_02_ordinary_functions/ordinary_funcs.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.968026 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2518 2024-03-23 20:14:41.000000 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      978 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/autonomicity_checks.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4986 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/autonomous_decorators.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     9725 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/autonomous_funcs.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3575 2024-03-17 06:16:19.000000 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/call_graph_explorer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     8286 2024-03-17 06:16:19.000000 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/names_usage_analyzer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      404 2024-03-16 05:00:28.000000 pythagoras-0.10.41/pythagoras/_03_autonomous_functions/pth_available_names_retriever.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.972414 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2385 2024-03-23 20:14:41.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      936 2024-02-27 05:38:18.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      200 2024-03-16 20:57:07.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/idempotency_checks.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      824 2024-03-16 20:57:07.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/idempotent_decorator.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)    24423 2024-04-04 04:18:43.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2266 2024-03-17 06:20:02.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/kw_args.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4280 2024-03-19 06:32:05.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/output_capturer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      569 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/persidict_to_timeline.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1398 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_04_idempotent_functions/process_augmented_func_src.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.977108 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      192 2024-03-09 06:54:01.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      411 2024-03-01 23:23:38.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/current_date_gmt_str.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2691 2024-03-16 20:59:15.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/event_posters.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1748 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/execution_environment_summary.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1800 2024-03-17 06:16:39.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/find_in_callstack.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1051 2024-03-16 05:20:24.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/global_event_loggers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      540 2024-03-02 05:43:58.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/notebook_checker.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1066 2024-03-17 06:18:06.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/type_retrievers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2132 2024-03-08 04:41:55.000000 pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.978466 pythagoras-0.10.41/pythagoras/_06_swarming/
--rw-r--r--   0 Pythagoras   (504) staff       (20)       87 2024-03-13 04:53:14.000000 pythagoras-0.10.41/pythagoras/_06_swarming/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2776 2024-04-03 22:38:19.000000 pythagoras-0.10.41/pythagoras/_06_swarming/background_workers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      626 2024-03-10 22:12:16.000000 pythagoras-0.10.41/pythagoras/_06_swarming/output_suppressor.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.980374 pythagoras-0.10.41/pythagoras/_07_mission_control/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      352 2024-03-10 21:01:51.000000 pythagoras-0.10.41/pythagoras/_07_mission_control/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     9883 2024-04-03 22:38:19.000000 pythagoras-0.10.41/pythagoras/_07_mission_control/global_state_management.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3463 2024-04-04 00:39:27.000000 pythagoras-0.10.41/pythagoras/_07_mission_control/summary.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.982171 pythagoras-0.10.41/pythagoras/_99_misc_utils/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      175 2024-03-10 05:49:40.000000 pythagoras-0.10.41/pythagoras/_99_misc_utils/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      451 2024-03-16 04:14:22.000000 pythagoras-0.10.41/pythagoras/_99_misc_utils/id_examiner.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      650 2024-02-22 18:42:45.000000 pythagoras-0.10.41/pythagoras/_99_misc_utils/long_infoname.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1116 2024-02-27 01:25:58.000000 pythagoras-0.10.41/pythagoras/_99_misc_utils/package_manager.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1648 2024-03-23 20:14:41.000000 pythagoras-0.10.41/pythagoras/__init__.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 04:20:51.960632 pythagoras-0.10.41/pythagoras.egg-info/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-04 04:20:51.000000 pythagoras-0.10.41/pythagoras.egg-info/PKG-INFO
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2929 2024-04-04 04:20:51.000000 pythagoras-0.10.41/pythagoras.egg-info/SOURCES.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)        1 2024-04-04 04:20:51.000000 pythagoras-0.10.41/pythagoras.egg-info/dependency_links.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)      121 2024-04-04 04:20:51.000000 pythagoras-0.10.41/pythagoras.egg-info/requires.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)       11 2024-04-04 04:20:51.000000 pythagoras-0.10.41/pythagoras.egg-info/top_level.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)       38 2024-04-04 04:20:51.983558 pythagoras-0.10.41/setup.cfg
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1964 2024-04-04 04:20:21.000000 pythagoras-0.10.41/setup.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.843285 pythagoras-0.10.42/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1114 2023-12-24 04:46:00.000000 pythagoras-0.10.42/LICENSE
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-04 05:18:43.842733 pythagoras-0.10.42/PKG-INFO
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-04-04 02:44:15.000000 pythagoras-0.10.42/README.md
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       80 2023-12-24 04:46:00.000000 pythagoras-0.10.42/pyproject.toml
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.819375 pythagoras-0.10.42/pythagoras/
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.822376 pythagoras-0.10.42/pythagoras/_01_foundational_objects/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      792 2024-03-23 20:14:41.000000 pythagoras-0.10.42/pythagoras/_01_foundational_objects/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1239 2024-02-22 05:34:39.000000 pythagoras-0.10.42/pythagoras/_01_foundational_objects/base_16_32_convertors.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3341 2024-03-17 06:20:02.000000 pythagoras-0.10.42/pythagoras/_01_foundational_objects/hash_addresses.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1510 2024-03-10 05:40:41.000000 pythagoras-0.10.42/pythagoras/_01_foundational_objects/hash_and_random_signatures.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      720 2024-03-10 19:35:01.000000 pythagoras-0.10.42/pythagoras/_01_foundational_objects/multipersidict.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2611 2024-03-17 06:40:19.000000 pythagoras-0.10.42/pythagoras/_01_foundational_objects/value_addresses.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.824556 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      908 2024-03-17 06:16:19.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1894 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/assert_ordinarity.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      815 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/check_n_positional_args.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      723 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/code_normalizer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4595 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      400 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/function_name.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      288 2024-03-16 20:40:58.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/ordinary_decorator.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1469 2024-03-17 05:40:33.000000 pythagoras-0.10.42/pythagoras/_02_ordinary_functions/ordinary_funcs.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.827179 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2518 2024-03-23 20:14:41.000000 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      978 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/autonomicity_checks.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4986 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/autonomous_decorators.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     9725 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/autonomous_funcs.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3575 2024-03-17 06:16:19.000000 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/call_graph_explorer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     8286 2024-03-17 06:16:19.000000 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/names_usage_analyzer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      404 2024-03-16 05:00:28.000000 pythagoras-0.10.42/pythagoras/_03_autonomous_functions/pth_available_names_retriever.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.831477 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2385 2024-03-23 20:14:41.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      936 2024-02-27 05:38:18.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      200 2024-03-16 20:57:07.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/idempotency_checks.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      824 2024-03-16 20:57:07.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/idempotent_decorator.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)    24578 2024-04-04 05:08:10.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2266 2024-03-17 06:20:02.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/kw_args.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4280 2024-03-19 06:32:05.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/output_capturer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      569 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/persidict_to_timeline.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1398 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_04_idempotent_functions/process_augmented_func_src.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.836193 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      192 2024-03-09 06:54:01.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      411 2024-03-01 23:23:38.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/current_date_gmt_str.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2691 2024-03-16 20:59:15.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/event_posters.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1748 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/execution_environment_summary.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1800 2024-03-17 06:16:39.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/find_in_callstack.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1051 2024-03-16 05:20:24.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/global_event_loggers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      540 2024-03-02 05:43:58.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/notebook_checker.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1066 2024-03-17 06:18:06.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/type_retrievers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2132 2024-03-08 04:41:55.000000 pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.837931 pythagoras-0.10.42/pythagoras/_06_swarming/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       87 2024-03-13 04:53:14.000000 pythagoras-0.10.42/pythagoras/_06_swarming/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2776 2024-04-03 22:38:19.000000 pythagoras-0.10.42/pythagoras/_06_swarming/background_workers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      626 2024-03-10 22:12:16.000000 pythagoras-0.10.42/pythagoras/_06_swarming/output_suppressor.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.839950 pythagoras-0.10.42/pythagoras/_07_mission_control/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      352 2024-03-10 21:01:51.000000 pythagoras-0.10.42/pythagoras/_07_mission_control/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     9883 2024-04-03 22:38:19.000000 pythagoras-0.10.42/pythagoras/_07_mission_control/global_state_management.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3463 2024-04-04 00:39:27.000000 pythagoras-0.10.42/pythagoras/_07_mission_control/summary.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.841932 pythagoras-0.10.42/pythagoras/_99_misc_utils/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      175 2024-03-10 05:49:40.000000 pythagoras-0.10.42/pythagoras/_99_misc_utils/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      451 2024-03-16 04:14:22.000000 pythagoras-0.10.42/pythagoras/_99_misc_utils/id_examiner.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      650 2024-02-22 18:42:45.000000 pythagoras-0.10.42/pythagoras/_99_misc_utils/long_infoname.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1116 2024-02-27 01:25:58.000000 pythagoras-0.10.42/pythagoras/_99_misc_utils/package_manager.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1648 2024-03-23 20:14:41.000000 pythagoras-0.10.42/pythagoras/__init__.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 05:18:43.820698 pythagoras-0.10.42/pythagoras.egg-info/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-04 05:18:43.000000 pythagoras-0.10.42/pythagoras.egg-info/PKG-INFO
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2929 2024-04-04 05:18:43.000000 pythagoras-0.10.42/pythagoras.egg-info/SOURCES.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)        1 2024-04-04 05:18:43.000000 pythagoras-0.10.42/pythagoras.egg-info/dependency_links.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      121 2024-04-04 05:18:43.000000 pythagoras-0.10.42/pythagoras.egg-info/requires.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       11 2024-04-04 05:18:43.000000 pythagoras-0.10.42/pythagoras.egg-info/top_level.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       38 2024-04-04 05:18:43.843437 pythagoras-0.10.42/setup.cfg
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1964 2024-04-04 05:18:10.000000 pythagoras-0.10.42/setup.py
```

### Comparing `pythagoras-0.10.41/LICENSE` & `pythagoras-0.10.42/LICENSE`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/PKG-INFO` & `pythagoras-0.10.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythagoras
-Version: 0.10.41
+Version: 0.10.42
 Summary: Simple framework for planet-scale idempotent computations in Python.
 Home-page: https://github.com/vladlpavlov/pythagoras
 Author: Volodymyr (Vlad) Pavlov
 Author-email: vlpavlov@ieee.org
 Keywords: cloud,ML,AI,serverless,distributed,parallel,machine-learning,deep-learning,pythagoras
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pythagoras-0.10.41/README.md` & `pythagoras-0.10.42/README.md`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_01_foundational_objects/__init__.py` & `pythagoras-0.10.42/pythagoras/_01_foundational_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_01_foundational_objects/base_16_32_convertors.py` & `pythagoras-0.10.42/pythagoras/_01_foundational_objects/base_16_32_convertors.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_01_foundational_objects/hash_addresses.py` & `pythagoras-0.10.42/pythagoras/_01_foundational_objects/hash_addresses.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_01_foundational_objects/hash_and_random_signatures.py` & `pythagoras-0.10.42/pythagoras/_01_foundational_objects/hash_and_random_signatures.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_01_foundational_objects/multipersidict.py` & `pythagoras-0.10.42/pythagoras/_01_foundational_objects/multipersidict.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_01_foundational_objects/value_addresses.py` & `pythagoras-0.10.42/pythagoras/_01_foundational_objects/value_addresses.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_02_ordinary_functions/__init__.py` & `pythagoras-0.10.42/pythagoras/_02_ordinary_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_02_ordinary_functions/assert_ordinarity.py` & `pythagoras-0.10.42/pythagoras/_02_ordinary_functions/assert_ordinarity.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_02_ordinary_functions/check_n_positional_args.py` & `pythagoras-0.10.42/pythagoras/_02_ordinary_functions/check_n_positional_args.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_02_ordinary_functions/code_normalizer.py` & `pythagoras-0.10.42/pythagoras/_02_ordinary_functions/code_normalizer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py` & `pythagoras-0.10.42/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_02_ordinary_functions/ordinary_funcs.py` & `pythagoras-0.10.42/pythagoras/_02_ordinary_functions/ordinary_funcs.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_03_autonomous_functions/__init__.py` & `pythagoras-0.10.42/pythagoras/_03_autonomous_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_03_autonomous_functions/autonomicity_checks.py` & `pythagoras-0.10.42/pythagoras/_03_autonomous_functions/autonomicity_checks.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_03_autonomous_functions/autonomous_decorators.py` & `pythagoras-0.10.42/pythagoras/_03_autonomous_functions/autonomous_decorators.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_03_autonomous_functions/autonomous_funcs.py` & `pythagoras-0.10.42/pythagoras/_03_autonomous_functions/autonomous_funcs.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_03_autonomous_functions/call_graph_explorer.py` & `pythagoras-0.10.42/pythagoras/_03_autonomous_functions/call_graph_explorer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_03_autonomous_functions/names_usage_analyzer.py` & `pythagoras-0.10.42/pythagoras/_03_autonomous_functions/names_usage_analyzer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/__init__.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/idempotent_decorator.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/idempotent_decorator.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,16 +234,21 @@
             pth.run_history.py[
                 output_address + ["augmented_source"]] = (
                 self.augmented_fn_source_code)
             assert output_address.can_be_executed
             unpacked_kwargs = UnpackedKwArgs(**packed_kwargs)
             result = super().execute(**unpacked_kwargs)
             result_addr = ValueAddr(result)
-            if output_address not in pth.execution_results: #TODO: refactor
-                pth.execution_results[output_address] = result_addr
+            try: #TODO: refactor this
+                if output_address not in pth.execution_results:
+                    pth.execution_results[output_address] = result_addr
+            except:
+                pass
+            finally:
+                assert output_address in pth.execution_results
             pth.run_history.pkl[
                 output_address + ["results",_pth_ec.session_id]] = result_addr
             output_address.drop_execution_request()
             return result
 
     def swarm_list(
             self
```

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/kw_args.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/kw_args.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/output_capturer.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/output_capturer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/persidict_to_timeline.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/persidict_to_timeline.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_04_idempotent_functions/process_augmented_func_src.py` & `pythagoras-0.10.42/pythagoras/_04_idempotent_functions/process_augmented_func_src.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/event_posters.py` & `pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/event_posters.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/execution_environment_summary.py` & `pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/execution_environment_summary.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/find_in_callstack.py` & `pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/find_in_callstack.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/global_event_loggers.py` & `pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/global_event_loggers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/notebook_checker.py` & `pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/notebook_checker.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/type_retrievers.py` & `pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/type_retrievers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py` & `pythagoras-0.10.42/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_06_swarming/background_workers.py` & `pythagoras-0.10.42/pythagoras/_06_swarming/background_workers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_06_swarming/output_suppressor.py` & `pythagoras-0.10.42/pythagoras/_06_swarming/output_suppressor.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_07_mission_control/global_state_management.py` & `pythagoras-0.10.42/pythagoras/_07_mission_control/global_state_management.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_07_mission_control/summary.py` & `pythagoras-0.10.42/pythagoras/_07_mission_control/summary.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_99_misc_utils/long_infoname.py` & `pythagoras-0.10.42/pythagoras/_99_misc_utils/long_infoname.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/_99_misc_utils/package_manager.py` & `pythagoras-0.10.42/pythagoras/_99_misc_utils/package_manager.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras/__init__.py` & `pythagoras-0.10.42/pythagoras/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/pythagoras.egg-info/PKG-INFO` & `pythagoras-0.10.42/pythagoras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythagoras
-Version: 0.10.41
+Version: 0.10.42
 Summary: Simple framework for planet-scale idempotent computations in Python.
 Home-page: https://github.com/vladlpavlov/pythagoras
 Author: Volodymyr (Vlad) Pavlov
 Author-email: vlpavlov@ieee.org
 Keywords: cloud,ML,AI,serverless,distributed,parallel,machine-learning,deep-learning,pythagoras
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pythagoras-0.10.41/pythagoras.egg-info/SOURCES.txt` & `pythagoras-0.10.42/pythagoras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.41/setup.py` & `pythagoras-0.10.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pythagoras"
-    ,version="0.10.41"
+    ,version="0.10.42"
     ,author="Volodymyr (Vlad) Pavlov"
     ,author_email="vlpavlov@ieee.org"
     ,description= "Simple framework for planet-scale "
                   + "idempotent computations in Python."
     ,long_description=long_description
     ,long_description_content_type="text/markdown"
     ,url="https://github.com/vladlpavlov/pythagoras"
```

