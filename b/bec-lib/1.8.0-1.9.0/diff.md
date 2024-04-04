# Comparing `tmp/bec_lib-1.8.0.tar.gz` & `tmp/bec_lib-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_lib-1.8.0.tar", last modified: Tue Feb 20 20:19:27 2024, max compression
+gzip compressed data, was "bec_lib-1.9.0.tar", last modified: Thu Feb 22 19:50:20 2024, max compression
```

## Comparing `bec_lib-1.8.0.tar` & `bec_lib-1.9.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.173408 bec_lib-1.8.0/
--rw-r--r--   0 root         (0) root         (0)     3049 2024-02-20 20:19:27.173408 bec_lib-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-02-20 11:03:23.000000 bec_lib-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.172408 bec_lib-1.8.0/bec_lib/
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3958 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/alarm_handler.py
--rw-r--r--   0 root         (0) root         (0)     3509 2024-02-20 20:19:16.000000 bec_lib-1.8.0/bec_lib/async_data.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/bec_errors.py
--rw-rw-rw-   0 root         (0) root         (0)    16512 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/bec_plotter.py
--rw-rw-rw-   0 root         (0) root         (0)    10495 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/bec_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7079 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/bl_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/bl_conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     5703 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/callback_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/channel_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     8133 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/client.py
--rw-rw-rw-   0 root         (0) root         (0)     5809 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/config_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.172408 bec_lib-1.8.0/bec_lib/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_lib-1.8.0/bec_lib/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41026 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/configs/demo_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)   289604 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/configs/openapi_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     5686 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/connector.py
--rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/dap_plugin_objects.py
--rw-rw-rw-   0 root         (0) root         (0)     3831 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/dap_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    27973 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/device.py
--rw-rw-rw-   0 root         (0) root         (0)    24298 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)    28839 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)     2723 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/file_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/lmfit_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/logbook_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     4888 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    21506 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     2976 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/numpy_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     4942 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/observer.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-02-20 20:19:16.000000 bec_lib-1.8.0/bec_lib/pdf_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/queue_items.py
--rw-r--r--   0 root         (0) root         (0)    23835 2024-02-20 20:19:16.000000 bec_lib-1.8.0/bec_lib/redis_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     5453 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/request_items.py
--rw-r--r--   0 root         (0) root         (0)     6441 2024-02-20 20:19:16.000000 bec_lib-1.8.0/bec_lib/scan_data.py
--rw-r--r--   0 root         (0) root         (0)    10615 2024-02-20 20:19:16.000000 bec_lib-1.8.0/bec_lib/scan_items.py
--rw-rw-rw-   0 root         (0) root         (0)     8772 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/scan_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/scan_report.py
--rw-rw-rw-   0 root         (0) root         (0)    14757 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/scibec_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     8593 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     2778 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/service_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/signature_serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.172408 bec_lib-1.8.0/bec_lib/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_lib-1.8.0/bec_lib/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42385 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/tests/test_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/tests/test_service_config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    23885 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4640 2024-02-20 11:03:23.000000 bec_lib-1.8.0/bec_lib/user_scripts_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7081 2024-02-20 17:20:48.000000 bec_lib-1.8.0/bec_lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.173408 bec_lib-1.8.0/bec_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3049 2024-02-20 20:19:27.000000 bec_lib-1.8.0/bec_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1467 2024-02-20 20:19:27.000000 bec_lib-1.8.0/bec_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:27.000000 bec_lib-1.8.0/bec_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-02-20 20:19:27.000000 bec_lib-1.8.0/bec_lib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      174 2024-02-20 20:19:27.000000 bec_lib-1.8.0/bec_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-02-20 20:19:27.000000 bec_lib-1.8.0/bec_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-02-20 20:19:27.174408 bec_lib-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-02-20 20:19:24.000000 bec_lib-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.723886 bec_lib-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)     3049 2024-02-22 19:50:20.723886 bec_lib-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2024-02-22 18:57:01.000000 bec_lib-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.721886 bec_lib-1.9.0/bec_lib/
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/alarm_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3509 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/async_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bec_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    16512 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bec_plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10495 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bec_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7079 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bl_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/bl_conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/callback_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/channel_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8133 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     5809 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/config_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.721886 bec_lib-1.9.0/bec_lib/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_lib-1.9.0/bec_lib/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41026 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/configs/demo_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   289604 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/configs/openapi_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/dap_plugin_objects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3831 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/dap_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)    27973 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/device.py
+-rw-rw-rw-   0 root         (0) root         (0)    24298 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)    28839 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/file_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/lmfit_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/logbook_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    21506 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/numpy_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/pdf_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7448 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/queue_items.py
+-rw-rw-rw-   0 root         (0) root         (0)    23835 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/redis_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     5453 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/request_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     6441 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scan_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10615 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scan_items.py
+-rw-rw-rw-   0 root         (0) root         (0)     8772 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scan_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/scan_report.py
+-rw-rw-rw-   0 root         (0) root         (0)    14757 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/scibec_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10181 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2778 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/service_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/signature_serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.722886 bec_lib-1.9.0/bec_lib/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_lib-1.9.0/bec_lib/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42385 2024-02-22 19:40:05.000000 bec_lib-1.9.0/bec_lib/tests/test_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/tests/test_service_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    23885 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/tests/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4640 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/user_scripts_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7081 2024-02-22 18:57:01.000000 bec_lib-1.9.0/bec_lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:20.722886 bec_lib-1.9.0/bec_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3049 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      174 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-02-22 19:50:20.000000 bec_lib-1.9.0/bec_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-02-22 19:50:20.724886 bec_lib-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-02-22 19:50:16.000000 bec_lib-1.9.0/setup.py
```

### Comparing `bec_lib-1.8.0/PKG-INFO` & `bec_lib-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_lib
-Version: 1.8.0
+Version: 1.9.0
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_lib-1.8.0/README.md` & `bec_lib-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/__init__.py` & `bec_lib-1.9.0/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/alarm_handler.py` & `bec_lib-1.9.0/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/async_data.py` & `bec_lib-1.9.0/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/bec_plotter.py` & `bec_lib-1.9.0/bec_lib/bec_plotter.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/bec_service.py` & `bec_lib-1.9.0/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/bl_checks.py` & `bec_lib-1.9.0/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/bl_conditions.py` & `bec_lib-1.9.0/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/callback_handler.py` & `bec_lib-1.9.0/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/channel_monitor.py` & `bec_lib-1.9.0/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/client.py` & `bec_lib-1.9.0/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/config_helper.py` & `bec_lib-1.9.0/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/configs/demo_config.yaml` & `bec_lib-1.9.0/bec_lib/configs/demo_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/configs/openapi_schema.json` & `bec_lib-1.9.0/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/connector.py` & `bec_lib-1.9.0/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/dap_plugin_objects.py` & `bec_lib-1.9.0/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/dap_plugins.py` & `bec_lib-1.9.0/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/device.py` & `bec_lib-1.9.0/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/devicemanager.py` & `bec_lib-1.9.0/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/endpoints.py` & `bec_lib-1.9.0/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/file_utils.py` & `bec_lib-1.9.0/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/lmfit_serializer.py` & `bec_lib-1.9.0/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/logbook_connector.py` & `bec_lib-1.9.0/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/logger.py` & `bec_lib-1.9.0/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/messages.py` & `bec_lib-1.9.0/bec_lib/messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/observer.py` & `bec_lib-1.9.0/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/pdf_writer.py` & `bec_lib-1.9.0/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/queue_items.py` & `bec_lib-1.9.0/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/redis_connector.py` & `bec_lib-1.9.0/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/request_items.py` & `bec_lib-1.9.0/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/scan_data.py` & `bec_lib-1.9.0/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/scan_items.py` & `bec_lib-1.9.0/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/scan_manager.py` & `bec_lib-1.9.0/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/scan_report.py` & `bec_lib-1.9.0/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/scans.py` & `bec_lib-1.9.0/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/scibec_validator.py` & `bec_lib-1.9.0/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/serialization.py` & `bec_lib-1.9.0/bec_lib/serialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
 def decode_set(obj):
     if isinstance(obj, dict) and "__msgpack__" in obj and obj["__msgpack__"]["type"] == "set":
         return set(obj["__msgpack__"]["data"])
     return obj
 
 
-class MsgpackExt:
-    """Encapsulates msgpack dumps/loads with extensions"""
+class SerializationRegistry:
+    """Registry for serialization codecs"""
 
     def __init__(self):
         self._encoder = []
         self._ext_decoder = {}
         self._object_hook_decoder = []
 
     def register_ext_type(self, encoder, decoder):
@@ -94,15 +94,15 @@
 
         Args:
             encoder: Function encoding a data into a serializable data.
             decoder: Function decoding a serialized data into a usable data.
         """
         exttype = len(self._ext_decoder)
         if exttype in self._ext_decoder:
-            ValueError("ExtType %d already used" % exttype)
+            raise ValueError("ExtType %d already used" % exttype)
         self._encoder.append((encoder, exttype))
         self._ext_decoder[exttype] = decoder
 
     def register_object_hook(self, encoder, decoder):
         """Register an encoder and a decoder that can convert a python object
         into data which can be serialized by msgpack.
 
@@ -110,19 +110,24 @@
             encoder: Function encoding a data into a data serializable by msgpack
             decoder: Function decoding a python structure provided by msgpack
             into an usable data.
         """
         self._encoder.append((encoder, None))
         self._object_hook_decoder.append(decoder)
 
-    def register_numpy(self):
+    def register_numpy(self, use_list=False):
         """
         Register BEC custom numpy encoder as a codec.
         """
-        self.register_object_hook(numpy_encoder.numpy_encode, numpy_encoder.numpy_decode)
+        if use_list:
+            self.register_object_hook(
+                numpy_encoder.numpy_encode_list, numpy_encoder.numpy_decode_list
+            )
+        else:
+            self.register_object_hook(numpy_encoder.numpy_encode, numpy_encoder.numpy_decode)
 
     def register_bec_message(self):
         """
         Register codec for BECMessage
         """
         # order matters
         self.register_ext_type(encode_bec_status, decode_bec_status)
@@ -130,14 +135,18 @@
 
     def register_set_encoder(self):
         """
         Register codec for set
         """
         self.register_object_hook(encode_set, decode_set)
 
+
+class MsgpackExt(SerializationRegistry):
+    """Encapsulates msgpack dumps/loads with extensions"""
+
     def _default(self, obj):
         for encoder, exttype in self._encoder:
             result = encoder(obj)
             if result is obj:
                 # Nothing was done, assume this encoder do not support this
                 # object kind
                 continue
@@ -178,14 +187,54 @@
             object_hook=self._object_hook,
             ext_hook=self._ext_hooks,
             raw=raw,
             strict_map_key=strict_map_key,
         )
 
 
+class JsonExt(SerializationRegistry):
+    """Encapsulates JSON dumps/loads with extensions"""
+
+    def _default(self, obj):
+        for encoder, _ in self._encoder:
+            result = encoder(obj)
+            if result is obj:
+                # Nothing was done, assume this encoder does not support this
+                # object kind
+                continue
+            return result
+
+    def _ext_hooks(self, data):
+        for decoder in self._object_hook_decoder:
+            try:
+                result = decoder(data)
+            except TypeError:
+                continue
+            if data is not result:
+                # In case the input is not the same as the output,
+                # consider it found the good decoder and it worked
+                break
+        else:
+            return data
+        return result
+
+    def dumps(self, obj):
+        """Serialize object `obj` and return serialized JSON string."""
+        return json.dumps(obj, default=self._default)
+
+    def loads(self, json_str):
+        """Deserialize JSON string `json_str` and return the deserialized object."""
+        return json.loads(json_str, object_hook=self._ext_hooks)
+
+
+json_ext = JsonExt()
+json_ext.register_numpy(use_list=True)
+json_ext.register_bec_message()
+json_ext.register_set_encoder()
+
 msgpack = MsgpackExt()
 msgpack.register_numpy()
 msgpack.register_bec_message()
 msgpack.register_set_encoder()
 
 
 class SerializationInterface:
```

### Comparing `bec_lib-1.8.0/bec_lib/service_config.py` & `bec_lib-1.9.0/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/signature_serializer.py` & `bec_lib-1.9.0/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/tests/test_config.yaml` & `bec_lib-1.9.0/bec_lib/tests/test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/tests/utils.py` & `bec_lib-1.9.0/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/user_scripts_mixin.py` & `bec_lib-1.9.0/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib/utils.py` & `bec_lib-1.9.0/bec_lib/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/bec_lib.egg-info/PKG-INFO` & `bec_lib-1.9.0/bec_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-lib
-Version: 1.8.0
+Version: 1.9.0
 Summary: BEC library
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_lib-1.8.0/bec_lib.egg-info/SOURCES.txt` & `bec_lib-1.9.0/bec_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_lib-1.8.0/setup.py` & `bec_lib-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 if __name__ == "__main__":
     setup(
         install_requires=[
             "numpy",
             "msgpack",
             "requests",
```

