# Comparing `tmp/cgcsdk-1.0.6.tar.gz` & `tmp/cgcsdk-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-1.0.6.tar", last modified: Wed Mar 13 09:42:23 2024, max compression
+gzip compressed data, was "cgcsdk-1.0.7.tar", last modified: Thu Apr  4 10:27:22 2024, max compression
```

## Comparing `cgcsdk-1.0.6.tar` & `cgcsdk-1.0.7.tar`

### file list

```diff
@@ -1,103 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.640251 cgcsdk-1.0.6/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1417 2024-03-13 09:42:23.637853 cgcsdk-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.388346 cgcsdk-1.0.6/cgc/
--rw-rw-rw-   0        0        0      209 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/.env
--rw-rw-rw-   0        0        0     7487 2024-03-13 09:39:15.000000 cgcsdk-1.0.6/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-1.0.6/cgc/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-1.0.6/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.402754 cgcsdk-1.0.6/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.415909 cgcsdk-1.0.6/cgc/commands/auth/
--rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-1.0.6/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-10-30 10:28:44.000000 cgcsdk-1.0.6/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1839 2023-10-30 10:06:10.000000 cgcsdk-1.0.6/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     5359 2023-10-30 10:06:10.000000 cgcsdk-1.0.6/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.428703 cgcsdk-1.0.6/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-1.0.6/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     4140 2023-11-15 10:46:21.000000 cgcsdk-1.0.6/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-1.0.6/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4711 2023-06-14 08:36:45.000000 cgcsdk-1.0.6/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     4326 2024-03-13 09:33:01.000000 cgcsdk-1.0.6/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-1.0.6/cgc/commands/cgc_cmd_responses.py
--rw-rw-rw-   0        0        0     1174 2024-03-13 09:33:01.000000 cgcsdk-1.0.6/cgc/commands/cgc_helpers.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.444503 cgcsdk-1.0.6/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-1.0.6/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0    15490 2024-03-13 09:36:12.000000 cgcsdk-1.0.6/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0     1139 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5807 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     8615 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.451370 cgcsdk-1.0.6/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.6/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3309 2024-03-13 09:33:01.000000 cgcsdk-1.0.6/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.458164 cgcsdk-1.0.6/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-1.0.6/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-1.0.6/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-1.0.6/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.468598 cgcsdk-1.0.6/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.6/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     4053 2024-03-13 09:33:01.000000 cgcsdk-1.0.6/cgc/commands/resource/resource_cmd.py
--rw-rw-rw-   0        0        0      197 2023-11-21 14:55:48.000000 cgcsdk-1.0.6/cgc/commands/resource/resource_responses.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.485490 cgcsdk-1.0.6/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-1.0.6/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-10-30 10:06:10.000000 cgcsdk-1.0.6/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     7673 2024-03-13 09:33:01.000000 cgcsdk-1.0.6/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-1.0.6/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-1.0.6/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/config.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.506883 cgcsdk-1.0.6/cgc/sdk/
--rw-rw-rw-   0        0        0      271 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      214 2024-03-08 13:51:26.000000 cgcsdk-1.0.6/cgc/sdk/exceptions.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-1.0.6/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-1.0.6/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-1.0.6/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     2844 2023-07-17 12:07:43.000000 cgcsdk-1.0.6/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0    13528 2024-03-13 09:33:01.000000 cgcsdk-1.0.6/cgc/sdk/resource.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-1.0.6/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.511895 cgcsdk-1.0.6/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-1.0.6/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.517946 cgcsdk-1.0.6/cgc/tests/
--rw-rw-rw-   0        0        0   102743 2023-07-17 12:07:43.000000 cgcsdk-1.0.6/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.541957 cgcsdk-1.0.6/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-1.0.6/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-1.0.6/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.574882 cgcsdk-1.0.6/cgc/utils/
--rw-rw-rw-   0        0        0     3466 2023-06-13 12:13:50.000000 cgcsdk-1.0.6/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-1.0.6/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-1.0.6/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.586095 cgcsdk-1.0.6/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1286 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-1.0.6/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.600314 cgcsdk-1.0.6/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-1.0.6/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2148 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1766 2023-10-30 10:18:38.000000 cgcsdk-1.0.6/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2561 2024-03-13 09:33:01.000000 cgcsdk-1.0.6/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     2050 2023-06-13 11:20:10.000000 cgcsdk-1.0.6/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     7374 2024-03-08 11:15:19.000000 cgcsdk-1.0.6/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-1.0.6/cgc/utils/update.py
--rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-1.0.6/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2024-03-13 09:42:23.635043 cgcsdk-1.0.6/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1417 2024-03-13 09:42:23.000000 cgcsdk-1.0.6/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2532 2024-03-13 09:42:23.000000 cgcsdk-1.0.6/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 09:42:23.000000 cgcsdk-1.0.6/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-03-13 09:42:23.000000 cgcsdk-1.0.6/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2024-03-13 09:42:23.000000 cgcsdk-1.0.6/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-13 09:42:23.000000 cgcsdk-1.0.6/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-13 09:42:23.640251 cgcsdk-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2096 2023-06-13 11:20:10.000000 cgcsdk-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.598588 cgcsdk-1.0.7/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3173 2024-04-04 10:27:22.578670 cgcsdk-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2024-03-27 14:48:25.000000 cgcsdk-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.606882 cgcsdk-1.0.7/cgc/
+-rw-rw-rw-   0        0        0      209 2024-04-04 10:26:20.000000 cgcsdk-1.0.7/cgc/.env
+-rw-rw-rw-   0        0        0     7808 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-1.0.7/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1493 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.656354 cgcsdk-1.0.7/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.703998 cgcsdk-1.0.7/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-1.0.7/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     3856 2023-10-30 10:28:44.000000 cgcsdk-1.0.7/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1839 2023-10-30 10:06:10.000000 cgcsdk-1.0.7/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     5359 2023-10-30 10:06:10.000000 cgcsdk-1.0.7/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.744462 cgcsdk-1.0.7/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     4140 2023-11-15 10:46:21.000000 cgcsdk-1.0.7/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4711 2023-06-14 08:36:45.000000 cgcsdk-1.0.7/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     4956 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2245 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/cgc_cmd_responses.py
+-rw-rw-rw-   0        0        0     1174 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/cgc_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.805689 cgcsdk-1.0.7/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0    15490 2024-03-13 09:36:12.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0     1173 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5807 2024-03-08 11:15:19.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     8812 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.826492 cgcsdk-1.0.7/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3309 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.846858 cgcsdk-1.0.7/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-1.0.7/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-1.0.7/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.890910 cgcsdk-1.0.7/cgc/commands/jobs/
+-rw-rw-rw-   0        0        0      231 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/__init__.py
+-rw-rw-rw-   0        0        0     5952 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/job_utils.py
+-rw-rw-rw-   0        0        0     6555 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/jobs_cmd.py
+-rw-rw-rw-   0        0        0     1771 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/jobs_responses.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.922278 cgcsdk-1.0.7/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     4053 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/resource/resource_cmd.py
+-rw-rw-rw-   0        0        0      197 2023-11-21 14:55:48.000000 cgcsdk-1.0.7/cgc/commands/resource/resource_responses.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.983915 cgcsdk-1.0.7/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-10-30 10:06:10.000000 cgcsdk-1.0.7/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     7673 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/config.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.081126 cgcsdk-1.0.7/cgc/sdk/
+-rw-rw-rw-   0        0        0      297 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      214 2024-03-08 13:51:26.000000 cgcsdk-1.0.7/cgc/sdk/exceptions.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-1.0.7/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     5332 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/sdk/job.py
+-rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-1.0.7/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-1.0.7/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     2844 2023-07-17 12:07:43.000000 cgcsdk-1.0.7/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0    13544 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/sdk/resource.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-1.0.7/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.118981 cgcsdk-1.0.7/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-1.0.7/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.160856 cgcsdk-1.0.7/cgc/tests/
+-rw-rw-rw-   0        0        0   102743 2023-07-17 12:07:43.000000 cgcsdk-1.0.7/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.474480 cgcsdk-1.0.7/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.936790 cgcsdk-1.0.7/cgc/utils/
+-rw-rw-rw-   0        0        0     3466 2023-06-13 12:13:50.000000 cgcsdk-1.0.7/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-1.0.7/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-1.0.7/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.076793 cgcsdk-1.0.7/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-03-08 11:15:19.000000 cgcsdk-1.0.7/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-1.0.7/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.235438 cgcsdk-1.0.7/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2432 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1766 2023-10-30 10:18:38.000000 cgcsdk-1.0.7/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2561 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     2050 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     7374 2024-03-08 11:15:19.000000 cgcsdk-1.0.7/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-1.0.7/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.444849 cgcsdk-1.0.7/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     3173 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2674 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:27:22.600011 cgcsdk-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2096 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/setup.py
```

### Comparing `cgcsdk-1.0.6/cgc/CHANGELOG.md` & `cgcsdk-1.0.7/cgc/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Change Log
 
+## 1.0.7
+
+Release on April 04, 2024
+
+* speed of resource creation with volumes / shared memory, has been improved
+* added jobs creation: cgc job create
+* added jobs list: cgc job list
+* added jobs delete: cgc job delete
+* added logs (STDOUT, STDERR) reader for spawned applications: cgc logs
+* added SDK for logs & jobs
+
 ## 1.0.6
 
 Release on March 13, 2024
 
 * updated exception handling for SDK
 * fix for cgc CLI command: compute create
 * ensure encode("utf-8") for all payloads generated by CLI/SDK
```

### Comparing `cgcsdk-1.0.6/cgc/cgc.py` & `cgcsdk-1.0.7/cgc/cgc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import click
 from cgc.commands.volume.volume_cmd import volume_group
 from cgc.commands.compute.compute_cmd import compute_group
 from cgc.commands.billing.billing_cmd import billing_group
 from cgc.commands.db.db_cmd import db_group
 from cgc.commands.resource.resource_cmd import resource_group
+from cgc.commands.jobs.jobs_cmd import job_group
 from cgc.commands.auth.auth_cmd import (
     api_keys_group,
     auth_register,
 )
 
 from cgc.commands.debug.debug_cmd import debug_group
 from cgc.commands.cgc_cmd import (
     cgc_rm,
     cgc_status,
+    cgc_logs,
     sending_telemetry_permission,
     resource_events,
     context_group,
 )
+
 from cgc.utils.version_control import check_version, _get_version
 from cgc.utils.click_group import CustomGroup
 
 
 @click.group(cls=CustomGroup)
 @click.version_option(_get_version())
 def cli():
@@ -37,13 +40,14 @@
 cli.add_command(db_group)
 cli.add_command(cgc_rm)
 cli.add_command(resource_events)
 cli.add_command(resource_group)
 cli.add_command(billing_group)
 cli.add_command(cgc_status)
 cli.add_command(sending_telemetry_permission)
-
+cli.add_command(cgc_logs)
+cli.add_command(job_group)
 
 if __name__ == "__main__" or __name__ == "cgc.cgc":
     cli()
 else:
     raise Exception("This program is not intended for importing!")
```

### Comparing `cgcsdk-1.0.6/cgc/commands/auth/auth_cmd.py` & `cgcsdk-1.0.7/cgc/commands/auth/auth_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/auth/auth_responses.py` & `cgcsdk-1.0.7/cgc/commands/auth/auth_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/auth/auth_utils.py` & `cgcsdk-1.0.7/cgc/commands/auth/auth_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/billing/__init__.py` & `cgcsdk-1.0.7/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/billing/billing_cmd.py` & `cgcsdk-1.0.7/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/billing/billing_responses.py` & `cgcsdk-1.0.7/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/billing/billing_utils.py` & `cgcsdk-1.0.7/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/cgc_cmd.py` & `cgcsdk-1.0.7/cgc/commands/cgc_cmd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import click
 import json
 
-from cgc.commands.cgc_cmd_responses import cgc_status_response
+from cgc.commands.cgc_cmd_responses import (
+    cgc_logs_response,
+    cgc_status_response,
+)
 from cgc.commands.resource.resource_cmd import resource_delete
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.click_group import CustomCommand, CustomGroup
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.telemetry.basic import telemetry_permission_set
 from cgc.commands.compute.compute_responses import compute_logs_response
-from cgc.commands.auth.auth_cmd import auth_register
+# from cgc.commands.auth.auth_cmd import auth_register
 from cgc.utils import set_environment_data, check_if_config_exist, list_all_config_files
 from cgc.commands.cgc_helpers import table_of_user_context_files
 from cgc.utils.config_utils import config_path
 from cgc.utils.consts.env_consts import ENV_FILE_PATH
 
 
 @click.command("rm", cls=CustomCommand)
@@ -33,15 +36,15 @@
     url = f"{api_url}/v1/api/resource/get_pod_events"
     metric = "resource.events"
     __payload = {"name": app_name}
     __res = call_api(
         request=EndpointTypes.get,
         url=url,
         headers=headers,
-        data=json.dumps(__payload).encode('utf-8'),
+        data=json.dumps(__payload).encode("utf-8"),
     )
     click.echo(
         compute_logs_response(retrieve_and_validate_response_send_metric(__res, metric))
     )
 
 
 @click.command("status", cls=CustomCommand)
@@ -118,7 +121,29 @@
     )
 
 
 @context_group.command("get-env-path", cls=CustomCommand)
 def get_env_path():
     """Displays current environment file path"""
     click.echo(f"Current environment file path: {ENV_FILE_PATH}")
+
+
+@click.command("logs", cls=CustomCommand)
+@click.argument("app_name", type=click.STRING)
+def cgc_logs(app_name):
+    """Displays logs of a given app"""
+
+    if not app_name:
+        raise click.ClickException("Please provide a non-empty name")
+
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/logs/{app_name}"
+    metric = "logs.get"
+    __res = call_api(
+        request=EndpointTypes.get,
+        url=url,
+        headers=headers,
+    )
+
+    click.echo(
+        cgc_logs_response(retrieve_and_validate_response_send_metric(__res, metric))
+    )
```

### Comparing `cgcsdk-1.0.6/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-1.0.7/cgc/commands/cgc_cmd_responses.py`

 * *Files 22% similar despite different names*

```diff
@@ -68,7 +68,15 @@
 
     return tabulate(
         list(
             zip(resource_names, types, resources_available_list, resources_limits_list)
         ),
         headers=list_headers,
     )
+
+
+def cgc_logs_response(data: dict):
+    return "\n".join(
+        "==> %s/%s <==\n%s" % (pod, cont, log)
+        for pod, containers in data["details"]["logs"].items()
+        for cont, log in containers.items()
+    )
```

### Comparing `cgcsdk-1.0.6/cgc/commands/cgc_helpers.py` & `cgcsdk-1.0.7/cgc/commands/cgc_helpers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/compute/compute_cmd.py` & `cgcsdk-1.0.7/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/compute/compute_models.py` & `cgcsdk-1.0.7/cgc/commands/compute/compute_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,7 +50,9 @@
     :type Enum: str
     """
 
     V100 = "V100"
     A100 = "A100"
     A5000 = "A5000"
     H100 = "H100"
+    P40 = "P40"
+    P100 = "P100"
```

### Comparing `cgcsdk-1.0.6/cgc/commands/compute/compute_responses.py` & `cgcsdk-1.0.7/cgc/commands/compute/compute_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/compute/compute_utills.py` & `cgcsdk-1.0.7/cgc/commands/compute/compute_utills.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ast import main
 import cgc.utils.consts.env_consts as env_consts
 
+
 def list_get_mounted_volumes_paths(volume_list: list) -> str:
     """Formats and returns list of PVC volumes mounted to an app.
 
     :param volume_list: list of all volumes mounted to an app
     :type volume_list: list
     :return: list of volume paths
     :rtype: str
@@ -16,14 +16,15 @@
             volume_mount_path = volume.get("mount_path")
             volume_name_list.append(volume_mount_path)
     volumes_mounted = (
         ", ".join(volume_name_list) if len(volume_name_list) != 0 else None
     )
     return volumes_mounted
 
+
 def list_get_mounted_volumes(volume_list: list) -> str:
     """Formats and returns list of PVC volumes mounted to an app.
 
     :param volume_list: list of all volumes mounted to an app
     :type volume_list: list
     :return: list of PVC volumes
     :rtype: str
@@ -35,38 +36,44 @@
             volume_name = volume.get("name")
             volume_name_list.append(volume_name)
     volumes_mounted = (
         ", ".join(volume_name_list) if len(volume_name_list) != 0 else None
     )
     return volumes_mounted
 
-def get_app_mounts(pod_list:list) -> list:
+
+def get_app_mounts(pod_list: list) -> list:
     output_data = []
-    
+
     for pod in pod_list:
         try:
-            main_container_name = pod["labels"]["entity"]   
+            main_container_name = pod["labels"]["entity"]
             try:
-                main_container = [x for x in pod["containers"] if x["name"] == main_container_name][0]
+                main_container = [
+                    x for x in pod["containers"] if x["name"] == main_container_name
+                ][0]
             except IndexError:
-                raise Exception("Parser was unable to find main container in server output in container list")
+                raise Exception(
+                    "Parser was unable to find main container in server output in container list"
+                )
             volumes_mounted = list_get_mounted_volumes(main_container["mounts"])
             volumes_paths = list_get_mounted_volumes_paths(main_container["mounts"])
             pod_data = {
                 "name": pod["labels"]["app-name"],
                 "type": pod["labels"]["entity"],
                 "status": pod["status"],
                 "volumes_mounted": volumes_mounted,
                 "volumes_paths": volumes_paths,
             }
             output_data.append(pod_data)
         except KeyError:
             pass
     return output_data
 
+
 def get_app_list(pod_list: list, detailed: bool) -> list:
     """Formats and returns list of apps to print.
 
     :param pod_list: list of pods
     :type pod_list: list
     :return: formatted list of apps
     :rtype: list
@@ -106,14 +113,17 @@
                 pod["labels"]["url"] = pod["labels"]["pod_url"]
                 if pod_data["type"] != "filebrowser":
                     pod["labels"]["url"] += f"""/?token={pod["labels"]['app-token']}"""
             else:
                 pod["labels"]["url"] = pod["labels"]["pod_url"]
                 pod["labels"].pop("app-token")
             pod["labels"].pop("pod_url")
+            pod["labels"].pop("resource-type")
+            pod["labels"].pop("api-key-id", None)
+            pod["labels"].pop("user-id", None)
 
             # appending the rest of labels
             pod_data.update(pod["labels"])
             output_data.append(pod_data)
         except KeyError:
             pass
```

### Comparing `cgcsdk-1.0.6/cgc/commands/db/db_cmd.py` & `cgcsdk-1.0.7/cgc/commands/db/db_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/resource/resource_cmd.py` & `cgcsdk-1.0.7/cgc/commands/resource/resource_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/volume/data_model.py` & `cgcsdk-1.0.7/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/volume/volume_cmd.py` & `cgcsdk-1.0.7/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/volume/volume_responses.py` & `cgcsdk-1.0.7/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/commands/volume/volume_utils.py` & `cgcsdk-1.0.7/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/sdk/handlers.py` & `cgcsdk-1.0.7/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/sdk/mongodb.py` & `cgcsdk-1.0.7/cgc/sdk/mongodb.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/sdk/postgresql.py` & `cgcsdk-1.0.7/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/sdk/redis.py` & `cgcsdk-1.0.7/cgc/sdk/redis.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/sdk/resource.py` & `cgcsdk-1.0.7/cgc/sdk/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
         __res, metric
     )
 
 
 class ResourceTypes(_Enum):
     compute = "compute"
     db = "db"
+    job = "job"
 
 
 def _resource_status_ready(name: str, response: dict):
     """
     Check if a resource is ready.
 
     Args:
```

### Comparing `cgcsdk-1.0.6/cgc/server.crt` & `cgcsdk-1.0.7/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/telemetry/basic.py` & `cgcsdk-1.0.7/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/tests/__init__.py` & `cgcsdk-1.0.7/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-1.0.7/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-1.0.7/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/tests/responses_tests.py` & `cgcsdk-1.0.7/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/__init__.py` & `cgcsdk-1.0.7/cgc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/click_group.py` & `cgcsdk-1.0.7/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/config_utils.py` & `cgcsdk-1.0.7/cgc/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/consts/env_consts.py` & `cgcsdk-1.0.7/cgc/utils/consts/env_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/consts/message_consts.py` & `cgcsdk-1.0.7/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-1.0.7/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-1.0.7/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-1.0.7/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/custom_exceptions.py` & `cgcsdk-1.0.7/cgc/utils/custom_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,34 @@
         "REQUEST_RESOURCE_LIMIT_EXCEEDED": "This request exceeds your resources limit",
         "RESOURCES_NOT_AVAILABLE_IN_CLUSTER": "Requested resources not available",
     },
     409: {
         "PVC_NAME_ALREADY_EXISTS": "Volume with this name already exists.",
         "PVC_DELETE_EXCEPTION": "Can't delete mounted volume, try with force",
         "RESOURCE_PORTS_ALREADY_EXISTS": "Port with this name already exists.",
-        "RESOURCE_TEMPLATE_NAME_ALREADY_EXISTS": "Template with this name already exists.",
+        "RESOURCE_TEMPLATE_NAME_ALREADY_EXISTS": "Resource with this name already exists.",
+        "JOB_CREATE_ALREADY_EXISTS": "Job with this name already exists.",
     },
     404: {
         "PVC_CREATE_NO_SC": "Selected disk type and access mode unavailable",
         "BILLING_STATUS_NO_DATA": "No data to print.",
         "NOT_DELETED_ANYTHING_IN_COMPUTE_DELETE": "No app with this name to delete.",
         "API_KEY_DELETE_ERROR": "No api key with this id to delete",
         "PVC_MOUNT_NOT_FOUND_TEMPLATE": "No app with this name to mount.",
         "PVC_UNMOUNT_NOT_MOUNTED": "Volume with this name is not mounted.",
         "PVC_NOT_FOUND": "Volume with this name not found.",
         "PVC_DELETE_NOT_FOUND": "App with this name not found.",
         "COMPUTE_RESTART_TEMPLATE_NOT_FOUND": "App with this name not found.",
         "COMPUTE_CREATE_TEMPLATE_NOT_FOUND": "There is no template with this name.",
         "COMPUTE_TEMPLATE_NAME_NOT_FOUND": "No app with this name.",
         "COMPUTE_RESOURCE_QUOTA_NOT_FOUND": "You do not have enforced limits on your namespace.",
+        "JOB_NOT_FOUND": "Job with this name not found.",
+        "RESOURCE_NOT_FOUND": "Resource with this name not found.",
     },
     400: {
         "WRONG_DATE_FORMAT": "Wrong date format.",
         "ENTITY_NOT_ALLOWED": "You can't create this entity.",
         "PVC_MOUNT_ALREADY_MOUNTED": "This volume is already mounted.",
         "TEMPLATE_NAME_SYSTEM_RESERVED": "You can't create app with this name.",
+        "JOB_LACKS_REQUIRED_PARAMETER": "Job requires container image parameter.",
     },
 }
```

### Comparing `cgcsdk-1.0.6/cgc/utils/message_utils.py` & `cgcsdk-1.0.7/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/prepare_headers.py` & `cgcsdk-1.0.7/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/requests_helper.py` & `cgcsdk-1.0.7/cgc/utils/requests_helper.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/response_utils.py` & `cgcsdk-1.0.7/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgc/utils/version_control.py` & `cgcsdk-1.0.7/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.6/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-1.0.7/cgcsdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,30 @@
 cgc/commands/compute/compute_models.py
 cgc/commands/compute/compute_responses.py
 cgc/commands/compute/compute_utills.py
 cgc/commands/db/__init__.py
 cgc/commands/db/db_cmd.py
 cgc/commands/debug/__init__.py
 cgc/commands/debug/debug_cmd.py
+cgc/commands/jobs/__init__.py
+cgc/commands/jobs/job_utils.py
+cgc/commands/jobs/jobs_cmd.py
+cgc/commands/jobs/jobs_responses.py
 cgc/commands/resource/__init__.py
 cgc/commands/resource/resource_cmd.py
 cgc/commands/resource/resource_responses.py
 cgc/commands/volume/__init__.py
 cgc/commands/volume/data_model.py
 cgc/commands/volume/volume_cmd.py
 cgc/commands/volume/volume_responses.py
 cgc/commands/volume/volume_utils.py
 cgc/sdk/__init__.py
 cgc/sdk/exceptions.py
 cgc/sdk/handlers.py
+cgc/sdk/job.py
 cgc/sdk/mongodb.py
 cgc/sdk/postgresql.py
 cgc/sdk/redis.py
 cgc/sdk/resource.py
 cgc/telemetry/__init__.py
 cgc/telemetry/basic.py
 cgc/tests/__init__.py
```

### Comparing `cgcsdk-1.0.6/setup.py` & `cgcsdk-1.0.7/setup.py`

 * *Files identical despite different names*

