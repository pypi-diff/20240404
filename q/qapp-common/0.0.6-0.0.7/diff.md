# Comparing `tmp/qapp-common-0.0.6.tar.gz` & `tmp/qapp-common-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qapp-common-0.0.6.tar", last modified: Wed Apr  3 03:10:33 2024, max compression
+gzip compressed data, was "qapp-common-0.0.7.tar", last modified: Thu Apr  4 06:48:23 2024, max compression
```

## Comparing `qapp-common-0.0.6.tar` & `qapp-common-0.0.7.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.196951 qapp-common-0.0.6/
--rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1988 2024-04-03 03:10:33.195952 qapp-common-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.6/README.md
--rw-rw-rw-   0        0        0      805 2024-04-03 03:10:27.000000 qapp-common-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.115951 qapp-common-0.0.6/qapp_common/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.125983 qapp-common-0.0.6/qapp_common/async_tasks/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/async_tasks/__init__.py
--rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/async_tasks/async_task.py
--rw-rw-rw-   0        0        0     3914 2024-04-02 16:46:45.000000 qapp-common-0.0.6/qapp_common/async_tasks/export_circuit_task.py
--rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/async_tasks/post_processing_task.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.126951 qapp-common-0.0.6/qapp_common/component/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.129951 qapp-common-0.0.6/qapp_common/component/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/component/backend/__init__.py
--rw-rw-rw-   0        0        0     8374 2024-04-02 04:55:37.000000 qapp-common-0.0.6/qapp_common/component/backend/invocation.py
--rw-rw-rw-   0        0        0     9371 2024-04-02 07:36:54.000000 qapp-common-0.0.6/qapp_common/component/backend/job_fetching.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.132951 qapp-common-0.0.6/qapp_common/component/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/component/callback/__init__.py
--rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/component/callback/update_job_metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.136952 qapp-common-0.0.6/qapp_common/component/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/component/device/__init__.py
--rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/component/device/device_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.139952 qapp-common-0.0.6/qapp_common/config/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/config/__init__.py
--rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/config/logging_config.py
--rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/config/thread_config.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.140951 qapp-common-0.0.6/qapp_common/data/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.141951 qapp-common-0.0.6/qapp_common/data/async_task/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/async_task/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.144951 qapp-common-0.0.6/qapp_common/data/async_task/circuit_export/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/async_task/circuit_export/__init__.py
--rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/async_task/circuit_export/backend_holder.py
--rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/async_task/circuit_export/circuit_holder.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.146952 qapp-common-0.0.6/qapp_common/data/backend/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/backend/__init__.py
--rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/backend/backend_information.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.148951 qapp-common-0.0.6/qapp_common/data/callback/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/callback/__init__.py
--rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/callback/callback_url.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.150953 qapp-common-0.0.6/qapp_common/data/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/device/__init__.py
--rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/device/circuit_running_option.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.154951 qapp-common-0.0.6/qapp_common/data/promise/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/promise/__init__.py
--rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/promise/post_processing_promise.py
--rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/promise/promise.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.159951 qapp-common-0.0.6/qapp_common/data/request/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/request/__init__.py
--rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/request/invocation_request.py
--rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/request/job_fetching_request.py
--rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/request/request.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.163951 qapp-common-0.0.6/qapp_common/data/response/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/response/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/response/authentication.py
--rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/response/job_response.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/data/response/project_header.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.172951 qapp-common-0.0.6/qapp_common/enum/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/base_enum.py
--rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/http_header.py
--rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/invocation_step.py
--rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/media_type.py
--rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/processing_unit.py
--rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/provider_tag.py
--rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.175951 qapp-common-0.0.6/qapp_common/enum/status/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/status/__init__.py
--rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/status/job_status.py
--rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/status/status_code.py
--rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/enum/token_type.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.179951 qapp-common-0.0.6/qapp_common/factory/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/factory/__init__.py
--rw-rw-rw-   0        0        0      615 2024-04-02 16:16:18.000000 qapp-common-0.0.6/qapp_common/factory/device_factory.py
--rw-rw-rw-   0        0        0      541 2024-04-02 08:08:09.000000 qapp-common-0.0.6/qapp_common/factory/handler_factory.py
--rw-rw-rw-   0        0        0      572 2024-04-02 16:14:46.000000 qapp-common-0.0.6/qapp_common/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.181951 qapp-common-0.0.6/qapp_common/handler/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/handler/__init__.py
--rw-rw-rw-   0        0        0      513 2024-04-02 08:21:18.000000 qapp-common-0.0.6/qapp_common/handler/handler.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.182952 qapp-common-0.0.6/qapp_common/model/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.184951 qapp-common-0.0.6/qapp_common/model/device/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/model/device/__init__.py
--rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/model/device/device.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.186952 qapp-common-0.0.6/qapp_common/model/provider/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/model/provider/__init__.py
--rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/model/provider/provider.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.192951 qapp-common-0.0.6/qapp_common/util/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/util/__init__.py
--rw-rw-rw-   0        0        0      564 2024-04-02 08:10:23.000000 qapp-common-0.0.6/qapp_common/util/circuit_utils.py
--rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/util/file_utils.py
--rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/util/http_utils.py
--rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/util/json_parser_utils.py
--rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.6/qapp_common/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:10:33.194951 qapp-common-0.0.6/qapp_common.egg-info/
--rw-rw-rw-   0        0        0     1988 2024-04-03 03:10:33.000000 qapp-common-0.0.6/qapp_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2800 2024-04-03 03:10:33.000000 qapp-common-0.0.6/qapp_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:10:33.000000 qapp-common-0.0.6/qapp_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-04-03 03:10:33.000000 qapp-common-0.0.6/qapp_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 03:10:33.000000 qapp-common-0.0.6/qapp_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 03:10:33.196951 qapp-common-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.119854 qapp-common-0.0.7/
+-rw-rw-rw-   0        0        0     1111 2024-03-27 03:03:06.000000 qapp-common-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1988 2024-04-04 06:48:23.117855 qapp-common-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-04-01 07:05:10.000000 qapp-common-0.0.7/README.md
+-rw-rw-rw-   0        0        0      805 2024-04-04 06:45:20.000000 qapp-common-0.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.889853 qapp-common-0.0.7/qapp_common/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.914856 qapp-common-0.0.7/qapp_common/async_tasks/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/async_tasks/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/async_tasks/async_task.py
+-rw-rw-rw-   0        0        0     3914 2024-04-02 16:46:45.000000 qapp-common-0.0.7/qapp_common/async_tasks/export_circuit_task.py
+-rw-rw-rw-   0        0        0     2298 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/async_tasks/post_processing_task.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.918856 qapp-common-0.0.7/qapp_common/component/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.926856 qapp-common-0.0.7/qapp_common/component/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/component/backend/__init__.py
+-rw-rw-rw-   0        0        0     8591 2024-04-04 06:35:37.000000 qapp-common-0.0.7/qapp_common/component/backend/invocation.py
+-rw-rw-rw-   0        0        0     9371 2024-04-02 07:36:54.000000 qapp-common-0.0.7/qapp_common/component/backend/job_fetching.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.934857 qapp-common-0.0.7/qapp_common/component/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/component/callback/__init__.py
+-rw-rw-rw-   0        0        0     1241 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/component/callback/update_job_metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.940856 qapp-common-0.0.7/qapp_common/component/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/component/device/__init__.py
+-rw-rw-rw-   0        0        0     2228 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/component/device/device_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.952857 qapp-common-0.0.7/qapp_common/config/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/config/__init__.py
+-rw-rw-rw-   0        0        0      243 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/config/logging_config.py
+-rw-rw-rw-   0        0        0      458 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/config/thread_config.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.956213 qapp-common-0.0.7/qapp_common/data/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.958855 qapp-common-0.0.7/qapp_common/data/async_task/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/async_task/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.967858 qapp-common-0.0.7/qapp_common/data/async_task/circuit_export/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/async_task/circuit_export/__init__.py
+-rw-rw-rw-   0        0        0      412 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/async_task/circuit_export/backend_holder.py
+-rw-rw-rw-   0        0        0      293 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/async_task/circuit_export/circuit_holder.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.973855 qapp-common-0.0.7/qapp_common/data/backend/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/backend/__init__.py
+-rw-rw-rw-   0        0        0      462 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/backend/backend_information.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.979856 qapp-common-0.0.7/qapp_common/data/callback/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/callback/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/callback/callback_url.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.984853 qapp-common-0.0.7/qapp_common/data/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/device/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/device/circuit_running_option.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:22.991856 qapp-common-0.0.7/qapp_common/data/promise/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/promise/__init__.py
+-rw-rw-rw-   0        0        0      698 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/promise/post_processing_promise.py
+-rw-rw-rw-   0        0        0      413 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/promise/promise.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.002853 qapp-common-0.0.7/qapp_common/data/request/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/request/__init__.py
+-rw-rw-rw-   0        0        0     1024 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/request/invocation_request.py
+-rw-rw-rw-   0        0        0      346 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/request/job_fetching_request.py
+-rw-rw-rw-   0        0        0     1187 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/request/request.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.014854 qapp-common-0.0.7/qapp_common/data/response/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/response/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/response/authentication.py
+-rw-rw-rw-   0        0        0     1221 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/response/job_response.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/data/response/project_header.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.044855 qapp-common-0.0.7/qapp_common/enum/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/base_enum.py
+-rw-rw-rw-   0        0        0      270 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/http_header.py
+-rw-rw-rw-   0        0        0      357 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/invocation_step.py
+-rw-rw-rw-   0        0        0      359 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/media_type.py
+-rw-rw-rw-   0        0        0      234 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      587 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/provider_tag.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.053857 qapp-common-0.0.7/qapp_common/enum/status/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/status/__init__.py
+-rw-rw-rw-   0        0        0      222 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/status/job_status.py
+-rw-rw-rw-   0        0        0      201 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/status/status_code.py
+-rw-rw-rw-   0        0        0      196 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/enum/token_type.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.073861 qapp-common-0.0.7/qapp_common/factory/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/factory/__init__.py
+-rw-rw-rw-   0        0        0      615 2024-04-02 16:16:18.000000 qapp-common-0.0.7/qapp_common/factory/device_factory.py
+-rw-rw-rw-   0        0        0      541 2024-04-02 08:08:09.000000 qapp-common-0.0.7/qapp_common/factory/handler_factory.py
+-rw-rw-rw-   0        0        0      572 2024-04-02 16:14:46.000000 qapp-common-0.0.7/qapp_common/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.079854 qapp-common-0.0.7/qapp_common/handler/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/handler/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-04-02 08:21:18.000000 qapp-common-0.0.7/qapp_common/handler/handler.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.083857 qapp-common-0.0.7/qapp_common/model/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.088854 qapp-common-0.0.7/qapp_common/model/device/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/model/device/__init__.py
+-rw-rw-rw-   0        0        0     9546 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/model/device/device.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.093854 qapp-common-0.0.7/qapp_common/model/provider/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/model/provider/__init__.py
+-rw-rw-rw-   0        0        0      882 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/model/provider/provider.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.109855 qapp-common-0.0.7/qapp_common/util/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/util/__init__.py
+-rw-rw-rw-   0        0        0      564 2024-04-02 08:10:23.000000 qapp-common-0.0.7/qapp_common/util/circuit_utils.py
+-rw-rw-rw-   0        0        0      553 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/util/file_utils.py
+-rw-rw-rw-   0        0        0     1071 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/util/http_utils.py
+-rw-rw-rw-   0        0        0     2504 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/util/json_parser_utils.py
+-rw-rw-rw-   0        0        0     1167 2024-04-01 07:10:10.000000 qapp-common-0.0.7/qapp_common/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:48:23.112856 qapp-common-0.0.7/qapp_common.egg-info/
+-rw-rw-rw-   0        0        0     1988 2024-04-04 06:48:22.000000 qapp-common-0.0.7/qapp_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2800 2024-04-04 06:48:22.000000 qapp-common-0.0.7/qapp_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 06:48:22.000000 qapp-common-0.0.7/qapp_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-04-04 06:48:22.000000 qapp-common-0.0.7/qapp_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 06:48:22.000000 qapp-common-0.0.7/qapp_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 06:48:23.119854 qapp-common-0.0.7/setup.cfg
```

### Comparing `qapp-common-0.0.6/LICENSE` & `qapp-common-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/PKG-INFO` & `qapp-common-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.6
+Version: 0.0.7
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.6/pyproject.toml` & `qapp-common-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qapp-common"
-version = "0.0.6"
+version = "0.0.7"
 description = "QApp common library supporting QApp Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `qapp-common-0.0.6/qapp_common/async_tasks/export_circuit_task.py` & `qapp-common-0.0.7/qapp_common/async_tasks/export_circuit_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/async_tasks/post_processing_task.py` & `qapp-common-0.0.7/qapp_common/async_tasks/post_processing_task.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/component/backend/invocation.py` & `qapp-common-0.0.7/qapp_common/component/backend/invocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
     def __prepare_backend_data(self, circuit):
         """
 
         @param circuit: Circuit was run
         """
 
-        required_qubit_amount = CircuitUtils.get_qubit_amount(circuit)
+        required_qubit_amount = self._get_qubit_amount(circuit)
 
         device_selection = DeviceSelection(
             required_qubit_amount,
             self.device_id,
             self.authentication.user_token,
             self.device_selection_url,
         )
@@ -236,7 +236,15 @@
     @abstractmethod
     def _create_device(self, provider: Provider):
         """
         Create device with DeviceFactory
         """
 
         raise NotImplemented('[Invocation] _create_device() method must be implemented')
+
+    @abstractmethod
+    def _get_qubit_amount(self, circuit):
+        """
+        Get number qubit of circuit
+        """
+
+        raise NotImplemented('[Invocation] _get_qubit_amount() method must be implemented')
```

### Comparing `qapp-common-0.0.6/qapp_common/component/backend/job_fetching.py` & `qapp-common-0.0.7/qapp_common/component/backend/job_fetching.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/component/callback/update_job_metadata.py` & `qapp-common-0.0.7/qapp_common/component/callback/update_job_metadata.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/component/device/device_selection.py` & `qapp-common-0.0.7/qapp_common/component/device/device_selection.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/data/device/circuit_running_option.py` & `qapp-common-0.0.7/qapp_common/data/device/circuit_running_option.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/data/promise/post_processing_promise.py` & `qapp-common-0.0.7/qapp_common/data/promise/post_processing_promise.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/data/request/invocation_request.py` & `qapp-common-0.0.7/qapp_common/data/request/invocation_request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/data/request/request.py` & `qapp-common-0.0.7/qapp_common/data/request/request.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/data/response/job_response.py` & `qapp-common-0.0.7/qapp_common/data/response/job_response.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/enum/provider_tag.py` & `qapp-common-0.0.7/qapp_common/enum/provider_tag.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/factory/device_factory.py` & `qapp-common-0.0.7/qapp_common/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/factory/handler_factory.py` & `qapp-common-0.0.7/qapp_common/factory/handler_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/factory/provider_factory.py` & `qapp-common-0.0.7/qapp_common/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/handler/handler.py` & `qapp-common-0.0.7/qapp_common/handler/handler.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/model/device/device.py` & `qapp-common-0.0.7/qapp_common/model/device/device.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/model/provider/provider.py` & `qapp-common-0.0.7/qapp_common/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/util/circuit_utils.py` & `qapp-common-0.0.7/qapp_common/util/circuit_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/util/file_utils.py` & `qapp-common-0.0.7/qapp_common/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/util/http_utils.py` & `qapp-common-0.0.7/qapp_common/util/http_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/util/json_parser_utils.py` & `qapp-common-0.0.7/qapp_common/util/json_parser_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common/util/response_utils.py` & `qapp-common-0.0.7/qapp_common/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `qapp-common-0.0.6/qapp_common.egg-info/PKG-INFO` & `qapp-common-0.0.7/qapp_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qapp-common
-Version: 0.0.6
+Version: 0.0.7
 Summary: QApp common library supporting QApp Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `qapp-common-0.0.6/qapp_common.egg-info/SOURCES.txt` & `qapp-common-0.0.7/qapp_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

