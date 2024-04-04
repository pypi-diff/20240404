# Comparing `tmp/pythagoras-0.10.37.tar.gz` & `tmp/pythagoras-0.10.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythagoras-0.10.37.tar", last modified: Wed Apr  3 06:27:26 2024, max compression
+gzip compressed data, was "pythagoras-0.10.38.tar", last modified: Thu Apr  4 00:14:52 2024, max compression
```

## Comparing `pythagoras-0.10.37.tar` & `pythagoras-0.10.38.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.882055 pythagoras-0.10.37/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1114 2023-12-24 04:46:00.000000 pythagoras-0.10.37/LICENSE
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-03 06:27:26.881543 pythagoras-0.10.37/PKG-INFO
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-03-24 05:25:36.000000 pythagoras-0.10.37/README.md
--rw-r--r--   0 Pythagoras   (504) staff       (20)       80 2023-12-24 04:46:00.000000 pythagoras-0.10.37/pyproject.toml
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.857629 pythagoras-0.10.37/pythagoras/
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.860616 pythagoras-0.10.37/pythagoras/_01_foundational_objects/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      792 2024-03-23 20:14:41.000000 pythagoras-0.10.37/pythagoras/_01_foundational_objects/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1239 2024-02-22 05:34:39.000000 pythagoras-0.10.37/pythagoras/_01_foundational_objects/base_16_32_convertors.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3341 2024-03-17 06:20:02.000000 pythagoras-0.10.37/pythagoras/_01_foundational_objects/hash_addresses.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1510 2024-03-10 05:40:41.000000 pythagoras-0.10.37/pythagoras/_01_foundational_objects/hash_and_random_signatures.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      720 2024-03-10 19:35:01.000000 pythagoras-0.10.37/pythagoras/_01_foundational_objects/multipersidict.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2611 2024-03-17 06:40:19.000000 pythagoras-0.10.37/pythagoras/_01_foundational_objects/value_addresses.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.863058 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      908 2024-03-17 06:16:19.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1894 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/assert_ordinarity.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      815 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/check_n_positional_args.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      723 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/code_normalizer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4595 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      400 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/function_name.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      288 2024-03-16 20:40:58.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/ordinary_decorator.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1469 2024-03-17 05:40:33.000000 pythagoras-0.10.37/pythagoras/_02_ordinary_functions/ordinary_funcs.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.866519 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2518 2024-03-23 20:14:41.000000 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      978 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/autonomicity_checks.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4986 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/autonomous_decorators.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     9725 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/autonomous_funcs.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3575 2024-03-17 06:16:19.000000 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/call_graph_explorer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     8286 2024-03-17 06:16:19.000000 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/names_usage_analyzer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      404 2024-03-16 05:00:28.000000 pythagoras-0.10.37/pythagoras/_03_autonomous_functions/pth_available_names_retriever.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.870670 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2385 2024-03-23 20:14:41.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      936 2024-02-27 05:38:18.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      200 2024-03-16 20:57:07.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/idempotency_checks.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      824 2024-03-16 20:57:07.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/idempotent_decorator.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)    23549 2024-03-24 03:13:32.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2266 2024-03-17 06:20:02.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/kw_args.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     4280 2024-03-19 06:32:05.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/output_capturer.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      569 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/persidict_to_timeline.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1398 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_04_idempotent_functions/process_augmented_func_src.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.875565 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      192 2024-03-09 06:54:01.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      411 2024-03-01 23:23:38.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/current_date_gmt_str.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2691 2024-03-16 20:59:15.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/event_posters.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1748 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/execution_environment_summary.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1800 2024-03-17 06:16:39.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/find_in_callstack.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1051 2024-03-16 05:20:24.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/global_event_loggers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      540 2024-03-02 05:43:58.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/notebook_checker.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1066 2024-03-17 06:18:06.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/type_retrievers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2132 2024-03-08 04:41:55.000000 pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.876809 pythagoras-0.10.37/pythagoras/_06_swarming/
--rw-r--r--   0 Pythagoras   (504) staff       (20)       87 2024-03-13 04:53:14.000000 pythagoras-0.10.37/pythagoras/_06_swarming/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2664 2024-03-17 06:12:34.000000 pythagoras-0.10.37/pythagoras/_06_swarming/background_workers.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      626 2024-03-10 22:12:16.000000 pythagoras-0.10.37/pythagoras/_06_swarming/output_suppressor.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.878752 pythagoras-0.10.37/pythagoras/_07_mission_control/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      352 2024-03-10 21:01:51.000000 pythagoras-0.10.37/pythagoras/_07_mission_control/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     9573 2024-04-03 06:01:25.000000 pythagoras-0.10.37/pythagoras/_07_mission_control/global_state_management.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-04-03 06:26:21.000000 pythagoras-0.10.37/pythagoras/_07_mission_control/summary.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.880757 pythagoras-0.10.37/pythagoras/_99_misc_utils/
--rw-r--r--   0 Pythagoras   (504) staff       (20)      175 2024-03-10 05:49:40.000000 pythagoras-0.10.37/pythagoras/_99_misc_utils/__init__.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      451 2024-03-16 04:14:22.000000 pythagoras-0.10.37/pythagoras/_99_misc_utils/id_examiner.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)      650 2024-02-22 18:42:45.000000 pythagoras-0.10.37/pythagoras/_99_misc_utils/long_infoname.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1116 2024-02-27 01:25:58.000000 pythagoras-0.10.37/pythagoras/_99_misc_utils/package_manager.py
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1648 2024-03-23 20:14:41.000000 pythagoras-0.10.37/pythagoras/__init__.py
-drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-03 06:27:26.858916 pythagoras-0.10.37/pythagoras.egg-info/
--rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-03 06:27:26.000000 pythagoras-0.10.37/pythagoras.egg-info/PKG-INFO
--rw-r--r--   0 Pythagoras   (504) staff       (20)     2929 2024-04-03 06:27:26.000000 pythagoras-0.10.37/pythagoras.egg-info/SOURCES.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)        1 2024-04-03 06:27:26.000000 pythagoras-0.10.37/pythagoras.egg-info/dependency_links.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)      121 2024-04-03 06:27:26.000000 pythagoras-0.10.37/pythagoras.egg-info/requires.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)       11 2024-04-03 06:27:26.000000 pythagoras-0.10.37/pythagoras.egg-info/top_level.txt
--rw-r--r--   0 Pythagoras   (504) staff       (20)       38 2024-04-03 06:27:26.882179 pythagoras-0.10.37/setup.cfg
--rw-r--r--   0 Pythagoras   (504) staff       (20)     1964 2024-04-03 06:27:02.000000 pythagoras-0.10.37/setup.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.896781 pythagoras-0.10.38/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1114 2023-12-24 04:46:00.000000 pythagoras-0.10.38/LICENSE
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-04 00:14:52.896102 pythagoras-0.10.38/PKG-INFO
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2195 2024-03-24 05:25:36.000000 pythagoras-0.10.38/README.md
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       80 2023-12-24 04:46:00.000000 pythagoras-0.10.38/pyproject.toml
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.858796 pythagoras-0.10.38/pythagoras/
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.863717 pythagoras-0.10.38/pythagoras/_01_foundational_objects/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      792 2024-03-23 20:14:41.000000 pythagoras-0.10.38/pythagoras/_01_foundational_objects/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1239 2024-02-22 05:34:39.000000 pythagoras-0.10.38/pythagoras/_01_foundational_objects/base_16_32_convertors.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3341 2024-03-17 06:20:02.000000 pythagoras-0.10.38/pythagoras/_01_foundational_objects/hash_addresses.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1510 2024-03-10 05:40:41.000000 pythagoras-0.10.38/pythagoras/_01_foundational_objects/hash_and_random_signatures.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      720 2024-03-10 19:35:01.000000 pythagoras-0.10.38/pythagoras/_01_foundational_objects/multipersidict.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2611 2024-03-17 06:40:19.000000 pythagoras-0.10.38/pythagoras/_01_foundational_objects/value_addresses.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.868854 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      908 2024-03-17 06:16:19.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1894 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/assert_ordinarity.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      815 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/check_n_positional_args.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      723 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/code_normalizer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4595 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      400 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/function_name.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      288 2024-03-16 20:40:58.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/ordinary_decorator.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1469 2024-03-17 05:40:33.000000 pythagoras-0.10.38/pythagoras/_02_ordinary_functions/ordinary_funcs.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.873479 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2518 2024-03-23 20:14:41.000000 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      978 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/autonomicity_checks.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4986 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/autonomous_decorators.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     9725 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/autonomous_funcs.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3575 2024-03-17 06:16:19.000000 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/call_graph_explorer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     8286 2024-03-17 06:16:19.000000 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/names_usage_analyzer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      404 2024-03-16 05:00:28.000000 pythagoras-0.10.38/pythagoras/_03_autonomous_functions/pth_available_names_retriever.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.880828 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2385 2024-03-23 20:14:41.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      936 2024-02-27 05:38:18.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      200 2024-03-16 20:57:07.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/idempotency_checks.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      824 2024-03-16 20:57:07.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/idempotent_decorator.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)    23549 2024-03-24 03:13:32.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2266 2024-03-17 06:20:02.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/kw_args.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     4280 2024-03-19 06:32:05.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/output_capturer.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      569 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/persidict_to_timeline.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1398 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_04_idempotent_functions/process_augmented_func_src.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.888496 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      192 2024-03-09 06:54:01.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      411 2024-03-01 23:23:38.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/current_date_gmt_str.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2691 2024-03-16 20:59:15.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/event_posters.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1748 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/execution_environment_summary.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1800 2024-03-17 06:16:39.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/find_in_callstack.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1051 2024-03-16 05:20:24.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/global_event_loggers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      540 2024-03-02 05:43:58.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/notebook_checker.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1066 2024-03-17 06:18:06.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/type_retrievers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2132 2024-03-08 04:41:55.000000 pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.890422 pythagoras-0.10.38/pythagoras/_06_swarming/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       87 2024-03-13 04:53:14.000000 pythagoras-0.10.38/pythagoras/_06_swarming/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2776 2024-04-03 22:38:19.000000 pythagoras-0.10.38/pythagoras/_06_swarming/background_workers.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      626 2024-03-10 22:12:16.000000 pythagoras-0.10.38/pythagoras/_06_swarming/output_suppressor.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.892289 pythagoras-0.10.38/pythagoras/_07_mission_control/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      352 2024-03-10 21:01:51.000000 pythagoras-0.10.38/pythagoras/_07_mission_control/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     9883 2024-04-03 22:38:19.000000 pythagoras-0.10.38/pythagoras/_07_mission_control/global_state_management.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3083 2024-04-03 22:23:44.000000 pythagoras-0.10.38/pythagoras/_07_mission_control/summary.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.894803 pythagoras-0.10.38/pythagoras/_99_misc_utils/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      175 2024-03-10 05:49:40.000000 pythagoras-0.10.38/pythagoras/_99_misc_utils/__init__.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      451 2024-03-16 04:14:22.000000 pythagoras-0.10.38/pythagoras/_99_misc_utils/id_examiner.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      650 2024-02-22 18:42:45.000000 pythagoras-0.10.38/pythagoras/_99_misc_utils/long_infoname.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1116 2024-02-27 01:25:58.000000 pythagoras-0.10.38/pythagoras/_99_misc_utils/package_manager.py
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1648 2024-03-23 20:14:41.000000 pythagoras-0.10.38/pythagoras/__init__.py
+drwxr-xr-x   0 Pythagoras   (504) staff       (20)        0 2024-04-04 00:14:52.860423 pythagoras-0.10.38/pythagoras.egg-info/
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     3558 2024-04-04 00:14:52.000000 pythagoras-0.10.38/pythagoras.egg-info/PKG-INFO
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     2929 2024-04-04 00:14:52.000000 pythagoras-0.10.38/pythagoras.egg-info/SOURCES.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)        1 2024-04-04 00:14:52.000000 pythagoras-0.10.38/pythagoras.egg-info/dependency_links.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)      121 2024-04-04 00:14:52.000000 pythagoras-0.10.38/pythagoras.egg-info/requires.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       11 2024-04-04 00:14:52.000000 pythagoras-0.10.38/pythagoras.egg-info/top_level.txt
+-rw-r--r--   0 Pythagoras   (504) staff       (20)       38 2024-04-04 00:14:52.896914 pythagoras-0.10.38/setup.cfg
+-rw-r--r--   0 Pythagoras   (504) staff       (20)     1964 2024-04-04 00:14:28.000000 pythagoras-0.10.38/setup.py
```

### Comparing `pythagoras-0.10.37/LICENSE` & `pythagoras-0.10.38/LICENSE`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/PKG-INFO` & `pythagoras-0.10.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythagoras
-Version: 0.10.37
+Version: 0.10.38
 Summary: Simple framework for planet-scale idempotent computations in Python.
 Home-page: https://github.com/vladlpavlov/pythagoras
 Author: Volodymyr (Vlad) Pavlov
 Author-email: vlpavlov@ieee.org
 Keywords: cloud,ML,AI,serverless,distributed,parallel,machine-learning,deep-learning,pythagoras
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pythagoras-0.10.37/README.md` & `pythagoras-0.10.38/README.md`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_01_foundational_objects/__init__.py` & `pythagoras-0.10.38/pythagoras/_01_foundational_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_01_foundational_objects/base_16_32_convertors.py` & `pythagoras-0.10.38/pythagoras/_01_foundational_objects/base_16_32_convertors.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_01_foundational_objects/hash_addresses.py` & `pythagoras-0.10.38/pythagoras/_01_foundational_objects/hash_addresses.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_01_foundational_objects/hash_and_random_signatures.py` & `pythagoras-0.10.38/pythagoras/_01_foundational_objects/hash_and_random_signatures.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_01_foundational_objects/multipersidict.py` & `pythagoras-0.10.38/pythagoras/_01_foundational_objects/multipersidict.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_01_foundational_objects/value_addresses.py` & `pythagoras-0.10.38/pythagoras/_01_foundational_objects/value_addresses.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_02_ordinary_functions/__init__.py` & `pythagoras-0.10.38/pythagoras/_02_ordinary_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_02_ordinary_functions/assert_ordinarity.py` & `pythagoras-0.10.38/pythagoras/_02_ordinary_functions/assert_ordinarity.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_02_ordinary_functions/check_n_positional_args.py` & `pythagoras-0.10.38/pythagoras/_02_ordinary_functions/check_n_positional_args.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_02_ordinary_functions/code_normalizer.py` & `pythagoras-0.10.38/pythagoras/_02_ordinary_functions/code_normalizer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py` & `pythagoras-0.10.38/pythagoras/_02_ordinary_functions/code_normalizer_implementation.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_02_ordinary_functions/ordinary_funcs.py` & `pythagoras-0.10.38/pythagoras/_02_ordinary_functions/ordinary_funcs.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_03_autonomous_functions/__init__.py` & `pythagoras-0.10.38/pythagoras/_03_autonomous_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_03_autonomous_functions/autonomicity_checks.py` & `pythagoras-0.10.38/pythagoras/_03_autonomous_functions/autonomicity_checks.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_03_autonomous_functions/autonomous_decorators.py` & `pythagoras-0.10.38/pythagoras/_03_autonomous_functions/autonomous_decorators.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_03_autonomous_functions/autonomous_funcs.py` & `pythagoras-0.10.38/pythagoras/_03_autonomous_functions/autonomous_funcs.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_03_autonomous_functions/call_graph_explorer.py` & `pythagoras-0.10.38/pythagoras/_03_autonomous_functions/call_graph_explorer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_03_autonomous_functions/names_usage_analyzer.py` & `pythagoras-0.10.38/pythagoras/_03_autonomous_functions/names_usage_analyzer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/__init__.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/astkeywords_dict_convertors.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/idempotent_decorator.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/idempotent_decorator.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/idempotent_func_address_context.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/kw_args.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/kw_args.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/output_capturer.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/output_capturer.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/persidict_to_timeline.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/persidict_to_timeline.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_04_idempotent_functions/process_augmented_func_src.py` & `pythagoras-0.10.38/pythagoras/_04_idempotent_functions/process_augmented_func_src.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/event_posters.py` & `pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/event_posters.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/execution_environment_summary.py` & `pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/execution_environment_summary.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/find_in_callstack.py` & `pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/find_in_callstack.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/global_event_loggers.py` & `pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/global_event_loggers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/notebook_checker.py` & `pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/notebook_checker.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/type_retrievers.py` & `pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/type_retrievers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py` & `pythagoras-0.10.38/pythagoras/_05_events_and_exceptions/uncaught_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_06_swarming/background_workers.py` & `pythagoras-0.10.38/pythagoras/_06_swarming/background_workers.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             return False
     except:
         return False
 
 
 def process_random_execution_request(pth_init_params:dict):
     pth_init_params["n_background_workers"] = 0
+    pth_init_params["return_summary_dataframe"] = False
     pth.initialize(**pth_init_params)
 
     with OutputSuppressor():
 
         candidate_addresses = []
         while len(candidate_addresses) == 0:
             random_delay = pth.entropy_infuser.uniform(0.5, 1.5)
@@ -47,14 +48,15 @@
 
         random_address = pth.entropy_infuser.choice(candidate_addresses)
         random_address.execute()
 
 
 def background_worker(pth_init_params:dict):
     pth_init_params["n_background_workers"] = 0
+    pth_init_params["return_summary_dataframe"] = False
     pth.initialize(**pth_init_params)
     subpr_kwargs = dict(pth_init_params=pth_init_params)
 
     ctx = get_context("spawn")
 
     with OutputSuppressor():
         while True:
```

### Comparing `pythagoras-0.10.37/pythagoras/_06_swarming/output_suppressor.py` & `pythagoras-0.10.38/pythagoras/_06_swarming/output_suppressor.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_07_mission_control/global_state_management.py` & `pythagoras-0.10.38/pythagoras/_07_mission_control/global_state_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     _clean_global_state()
     return initialize(*args, **kwargs)
 
 def initialize(base_dir:str
                , n_background_workers:int = 3
                , cloud_type:str = "local"
                , default_island_name:str = "Samos"
-               , runtime_id: str|None = None):
+               , runtime_id: str|None = None
+               , return_summary_dataframe:bool = True):
     """ Initialize Pythagoras.
     """
     assert pth.is_fully_unitialized(), (
         "You can only initialize pythagoras once.")
 
     cloud_type = cloud_type.lower()
 
@@ -130,15 +131,18 @@
     pth.initialization_parameters = parameters
 
     register_exception_handlers()
 
     for n in range(n_background_workers):
         pth.launch_background_worker()
 
-    return PythagorasContext()
+    if return_summary_dataframe:
+        return PythagorasContextWithSummary()
+    else:
+        return PythagorasContext()
 
 
 def is_fully_unitialized():
     """ Check if Pythagoras is uninitialized."""
     result = True
     result &= pth.value_store is None
     result &= pth.execution_results is None
@@ -236,15 +240,23 @@
     pth.entropy_infuser = None
     pth.n_background_workers = None
     pth.runtime_id = None
     unregister_exception_handlers()
     assert pth.is_fully_unitialized()
     assert pth.is_global_state_correct()
 
-class PythagorasContext(pd.DataFrame):
+
+class PythagorasContext:
+    def __enter__(self):
+        pass
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        _clean_global_state()
+
+class PythagorasContextWithSummary(pd.DataFrame):
 
     def __init__(self):
         super().__init__(summary(include_current_session=False))
 
     def __enter__(self):
         pass
```

### Comparing `pythagoras-0.10.37/pythagoras/_07_mission_control/summary.py` & `pythagoras-0.10.38/pythagoras/_07_mission_control/summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # from pythagoras._07_mission_control.global_state_management import (
 #   is_fully_unitialized, is_correctly_initialized)
 import pythagoras as pth
 import pandas as pd
 
+from pythagoras._05_events_and_exceptions.current_date_gmt_str import \
+    current_date_gmt_string
+
+
 def persistent(param, val) -> pd.DataFrame:
   d = dict(
-      parameter = [param]
-      ,value = [val]
-      ,type = "persistent")
+      type="persistent"
+      ,parameter = [param]
+      ,value = [val])
   return pd.DataFrame(d)
 
 
 def runtime(param, val) -> pd.DataFrame:
   d = dict(
-      parameter = [param]
-      ,value = [val]
-      ,type = "runtime")
+      type = "runtime"
+      ,parameter = [param]
+      ,value = [val])
   return pd.DataFrame(d)
 
 def summary(include_current_session:bool = True, print_result:bool = False):
     """ Get summary of Pythagoras' current state ."""
 
     # if is_fully_unitialized():
     #     return "Pythagoras is not initialized."
@@ -34,23 +38,42 @@
         "Total # of values stored", len(pth.value_store)))
     all_params.append(persistent(
         "Total # of function execution results cached"
         ,len(pth.execution_results)))
     all_params.append(persistent(
         "Total # of exceptions recorded", len(pth.crash_history)))
     all_params.append(persistent(
+        "    # of exceptions recorded today"
+        , len(pth.crash_history.get_subdict(current_date_gmt_string()))))
+    all_params.append(persistent(
         "Total # of events recorded", len(pth.event_log)))
     all_params.append(persistent(
+        "    # of exceptions recorded today"
+        , len(pth.event_log.get_subdict(current_date_gmt_string()))))
+    all_params.append(persistent(
         "Execution queue size", len(pth.execution_requests)))
     all_params.append(persistent(
         "# of currently active nodes", len(pth.compute_nodes.pkl)))
 
+    all_params.append(runtime(
+        "# of background workers on the current node"
+        , pth.n_background_workers))
+    all_params.append(runtime(
+        "Total # of available islands"
+        , len(pth.all_autonomous_functions)))
+    all_params.append(runtime(
+        "Default island name", pth.default_island_name))
+    all_params.append(runtime(
+        "All available islands"
+        , ", ".join(list(pth.all_autonomous_functions))))
+
 
     result = pd.concat(all_params)
     result.reset_index(drop=True, inplace=True)
+    # result.style.hide(axis="index")
 
 
     #
     # if include_current_session:
     #
     #     result += 21*"~" +  " CURRENT SESSION: " + 21*"~" + "\n"
     #     result += f"{len(pth.all_autonomous_functions)=} \n"
```

### Comparing `pythagoras-0.10.37/pythagoras/_99_misc_utils/long_infoname.py` & `pythagoras-0.10.38/pythagoras/_99_misc_utils/long_infoname.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/_99_misc_utils/package_manager.py` & `pythagoras-0.10.38/pythagoras/_99_misc_utils/package_manager.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras/__init__.py` & `pythagoras-0.10.38/pythagoras/__init__.py`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/pythagoras.egg-info/PKG-INFO` & `pythagoras-0.10.38/pythagoras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythagoras
-Version: 0.10.37
+Version: 0.10.38
 Summary: Simple framework for planet-scale idempotent computations in Python.
 Home-page: https://github.com/vladlpavlov/pythagoras
 Author: Volodymyr (Vlad) Pavlov
 Author-email: vlpavlov@ieee.org
 Keywords: cloud,ML,AI,serverless,distributed,parallel,machine-learning,deep-learning,pythagoras
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pythagoras-0.10.37/pythagoras.egg-info/SOURCES.txt` & `pythagoras-0.10.38/pythagoras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythagoras-0.10.37/setup.py` & `pythagoras-0.10.38/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pythagoras"
-    ,version="0.10.37"
+    ,version="0.10.38"
     ,author="Volodymyr (Vlad) Pavlov"
     ,author_email="vlpavlov@ieee.org"
     ,description= "Simple framework for planet-scale "
                   + "idempotent computations in Python."
     ,long_description=long_description
     ,long_description_content_type="text/markdown"
     ,url="https://github.com/vladlpavlov/pythagoras"
```

