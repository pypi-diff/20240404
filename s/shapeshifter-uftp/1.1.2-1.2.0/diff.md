# Comparing `tmp/shapeshifter-uftp-1.1.2.tar.gz` & `tmp/shapeshifter-uftp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapeshifter-uftp-1.1.2.tar", last modified: Tue Mar 12 06:53:29 2024, max compression
+gzip compressed data, was "shapeshifter-uftp-1.2.0.tar", last modified: Thu Apr  4 08:39:50 2024, max compression
```

## Comparing `shapeshifter-uftp-1.1.2.tar` & `shapeshifter-uftp-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 06:53:29.353380 shapeshifter-uftp-1.1.2/
--rw-rw-rw-   0        0        0      204 2024-03-12 06:53:29.353380 shapeshifter-uftp-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2024-03-12 06:50:44.000000 shapeshifter-uftp-1.1.2/README.rst
--rw-rw-rw-   0        0        0      285 2023-10-13 19:00:00.000000 shapeshifter-uftp-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-12 06:53:29.353380 shapeshifter-uftp-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1041 2024-03-12 06:52:39.000000 shapeshifter-uftp-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-12 06:53:29.237584 shapeshifter-uftp-1.1.2/shapeshifter_uftp/
--rw-rw-rw-   0        0        0     3774 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/__init__.py
--rw-rw-rw-   0        0        0     2077 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/cli.py
-drwxrwxrwx   0        0        0        0 2024-03-12 06:53:29.281058 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/
--rw-rw-rw-   0        0        0      654 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/__init__.py
--rw-rw-rw-   0        0        0      879 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/agr_cro_client.py
--rw-rw-rw-   0        0        0     3880 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/agr_dso_client.py
--rw-rw-rw-   0        0        0     9377 2023-08-23 09:48:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/base_client.py
--rw-rw-rw-   0        0        0      882 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/cro_agr_client.py
--rw-rw-rw-   0        0        0     1123 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/cro_dso_client.py
--rw-rw-rw-   0        0        0     3729 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/dso_agr_client.py
--rw-rw-rw-   0        0        0      825 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/dso_cro_client.py
--rw-rw-rw-   0        0        0     7419 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/exceptions.py
--rw-rw-rw-   0        0        0      831 2023-08-28 07:27:04.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/logging.py
-drwxrwxrwx   0        0        0        0 2024-03-12 06:53:29.297071 shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/
--rw-rw-rw-   0        0        0      286 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/__init__.py
--rw-rw-rw-   0        0        0    15747 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/agr_service.py
--rw-rw-rw-   0        0        0    12009 2024-03-12 06:50:04.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/base_service.py
--rw-rw-rw-   0        0        0     5006 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/cro_service.py
--rw-rw-rw-   0        0        0    13232 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/dso_service.py
--rw-rw-rw-   0        0        0     8967 2023-08-23 09:18:17.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/transport.py
-drwxrwxrwx   0        0        0        0 2024-03-12 06:53:29.313485 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/
--rw-rw-rw-   0        0        0     4606 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/__init__.py
--rw-rw-rw-   0        0        0    10206 2023-08-30 08:06:54.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/agr_cro.py
--rw-rw-rw-   0        0        0    37597 2023-08-30 08:06:56.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/agr_dso.py
--rw-rw-rw-   0        0        0     6941 2024-03-12 06:50:04.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/common.py
--rw-rw-rw-   0        0        0    10762 2023-09-04 05:47:45.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/cro_dso.py
--rw-rw-rw-   0        0        0       39 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/defaults.py
--rw-rw-rw-   0        0        0     6546 2023-08-30 08:02:20.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/metering.py
--rw-rw-rw-   0        0        0      193 2023-09-07 13:45:24.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/parsing.py
--rw-rw-rw-   0        0        0     1332 2023-09-04 05:52:17.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/validations.py
-drwxrwxrwx   0        0        0        0 2024-03-12 06:53:29.265943 shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/
--rw-rw-rw-   0        0        0      204 2024-03-12 06:53:29.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1764 2024-03-12 06:53:29.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 06:53:29.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2024-03-12 06:53:29.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      180 2024-03-12 06:53:29.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-12 06:53:29.000000 shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-12 06:53:29.351544 shapeshifter-uftp-1.1.2/test/
--rw-rw-rw-   0        0        0     1487 2023-08-23 09:03:59.000000 shapeshifter-uftp-1.1.2/test/test_cli.py
--rw-rw-rw-   0        0        0     1104 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_client_errors.py
--rw-rw-rw-   0        0        0     4060 2023-08-23 09:58:01.000000 shapeshifter-uftp-1.1.2/test/test_client_with_workers.py
--rw-rw-rw-   0        0        0     1112 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_clients_from_service.py
--rw-rw-rw-   0        0        0     2162 2023-09-04 05:48:02.000000 shapeshifter-uftp-1.1.2/test/test_communications.py
--rw-rw-rw-   0        0        0     1714 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_default_responses.py
--rw-rw-rw-   0        0        0     1229 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_message_destination.py
--rw-rw-rw-   0        0        0      547 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_presence_of_client_methods.py
--rw-rw-rw-   0        0        0      819 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_presence_of_service_methods.py
--rw-rw-rw-   0        0        0      630 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_roundtrip_serialization.py
--rw-rw-rw-   0        0        0     1966 2023-08-23 09:06:01.000000 shapeshifter-uftp-1.1.2/test/test_seal_and_unseal.py
--rw-rw-rw-   0        0        0     3604 2023-08-23 09:13:41.000000 shapeshifter-uftp-1.1.2/test/test_service_errors.py
--rw-rw-rw-   0        0        0      331 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_snake_case.py
--rw-rw-rw-   0        0        0     1228 2023-08-23 09:22:13.000000 shapeshifter-uftp-1.1.2/test/test_ttl_cache.py
--rw-rw-rw-   0        0        0     1228 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_validations.py
--rw-rw-rw-   0        0        0      719 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.1.2/test/test_xml_schema_compliance.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:39:50.399742 shapeshifter-uftp-1.2.0/
+-rw-rw-rw-   0        0        0      204 2024-04-04 08:39:50.399742 shapeshifter-uftp-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2871 2024-04-04 07:32:19.000000 shapeshifter-uftp-1.2.0/README.rst
+-rw-rw-rw-   0        0        0      285 2023-10-13 19:00:00.000000 shapeshifter-uftp-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 08:39:50.399742 shapeshifter-uftp-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2024-04-04 07:33:22.000000 shapeshifter-uftp-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:39:49.919780 shapeshifter-uftp-1.2.0/shapeshifter_uftp/
+-rw-rw-rw-   0        0        0     3774 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/__init__.py
+-rw-rw-rw-   0        0        0     2077 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:39:50.041098 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/
+-rw-rw-rw-   0        0        0      654 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/__init__.py
+-rw-rw-rw-   0        0        0      879 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/agr_cro_client.py
+-rw-rw-rw-   0        0        0     3880 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/agr_dso_client.py
+-rw-rw-rw-   0        0        0     9379 2024-04-04 07:28:23.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/base_client.py
+-rw-rw-rw-   0        0        0      882 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/cro_agr_client.py
+-rw-rw-rw-   0        0        0     1123 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/cro_dso_client.py
+-rw-rw-rw-   0        0        0     3750 2024-04-04 07:28:29.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/dso_agr_client.py
+-rw-rw-rw-   0        0        0      825 2024-04-04 07:28:32.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/dso_cro_client.py
+-rw-rw-rw-   0        0        0     7419 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/exceptions.py
+-rw-rw-rw-   0        0        0      831 2023-08-28 07:27:04.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/logging.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:39:50.100369 shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/
+-rw-rw-rw-   0        0        0      286 2024-04-04 07:28:49.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/__init__.py
+-rw-rw-rw-   0        0        0    15747 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/agr_service.py
+-rw-rw-rw-   0        0        0    12001 2024-04-04 07:26:21.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/base_service.py
+-rw-rw-rw-   0        0        0     5006 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/cro_service.py
+-rw-rw-rw-   0        0        0    13232 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/dso_service.py
+-rw-rw-rw-   0        0        0     8967 2023-08-23 09:18:17.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/transport.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:39:50.205587 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/
+-rw-rw-rw-   0        0        0     4606 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/__init__.py
+-rw-rw-rw-   0        0        0    10206 2023-08-30 08:06:54.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/agr_cro.py
+-rw-rw-rw-   0        0        0    37597 2023-08-30 08:06:56.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/agr_dso.py
+-rw-rw-rw-   0        0        0     6941 2024-03-12 06:50:04.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/common.py
+-rw-rw-rw-   0        0        0    10762 2023-09-04 05:47:45.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/cro_dso.py
+-rw-rw-rw-   0        0        0       39 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/defaults.py
+-rw-rw-rw-   0        0        0     6546 2023-08-30 08:02:20.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/metering.py
+-rw-rw-rw-   0        0        0      193 2023-09-07 13:45:24.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/parsing.py
+-rw-rw-rw-   0        0        0     1332 2023-09-04 05:52:17.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-04 08:39:49.956346 shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/
+-rw-rw-rw-   0        0        0      204 2024-04-04 08:39:49.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1764 2024-04-04 08:39:49.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 08:39:49.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2024-04-04 08:39:49.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      177 2024-04-04 08:39:49.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-04 08:39:49.000000 shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 08:39:50.399742 shapeshifter-uftp-1.2.0/test/
+-rw-rw-rw-   0        0        0     1487 2023-08-23 09:03:59.000000 shapeshifter-uftp-1.2.0/test/test_cli.py
+-rw-rw-rw-   0        0        0     1104 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_client_errors.py
+-rw-rw-rw-   0        0        0     4060 2023-08-23 09:58:01.000000 shapeshifter-uftp-1.2.0/test/test_client_with_workers.py
+-rw-rw-rw-   0        0        0     1112 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_clients_from_service.py
+-rw-rw-rw-   0        0        0     2162 2023-09-04 05:48:02.000000 shapeshifter-uftp-1.2.0/test/test_communications.py
+-rw-rw-rw-   0        0        0     1714 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_default_responses.py
+-rw-rw-rw-   0        0        0     1229 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_message_destination.py
+-rw-rw-rw-   0        0        0      547 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_presence_of_client_methods.py
+-rw-rw-rw-   0        0        0      819 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_presence_of_service_methods.py
+-rw-rw-rw-   0        0        0      630 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_roundtrip_serialization.py
+-rw-rw-rw-   0        0        0     1966 2023-08-23 09:06:01.000000 shapeshifter-uftp-1.2.0/test/test_seal_and_unseal.py
+-rw-rw-rw-   0        0        0     3604 2023-08-23 09:13:41.000000 shapeshifter-uftp-1.2.0/test/test_service_errors.py
+-rw-rw-rw-   0        0        0      331 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_snake_case.py
+-rw-rw-rw-   0        0        0     1228 2023-08-23 09:22:13.000000 shapeshifter-uftp-1.2.0/test/test_ttl_cache.py
+-rw-rw-rw-   0        0        0     1228 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_validations.py
+-rw-rw-rw-   0        0        0      719 2023-08-23 07:52:19.000000 shapeshifter-uftp-1.2.0/test/test_xml_schema_compliance.py
```

### Comparing `shapeshifter-uftp-1.1.2/README.rst` & `shapeshifter-uftp-1.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 Version History
 ---------------
 
 +-------------+-------------------+----------------------------------+
 | Version     | Release Date      | Release Notes                    |
 +=============+===================+==================================+
+| 1.2.0       | 2024-04-04        | Upgrade to latest FastAPI and    |
+|             |                   | Pydantic.                        |
++-------------+-------------------+----------------------------------+
 | 1.1.2       | 2024-03-12        | Pinned dependencies after a      |
 |             |                   | breaking update to fastapi-xml   |
 |             |                   | was released.                    |
 +-------------+-------------------+----------------------------------+
 | 1.1.0       | 2023-08-30        | Use the published 3.0.0 spec     |
 |             |                   | for the XSD validation and       |
 |             |                   | objects.                         |
```

### Comparing `shapeshifter-uftp-1.1.2/setup.py` & `shapeshifter-uftp-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
 
 setup(
     name="shapeshifter-uftp",
-    version="1.1.2",
+    version="1.2.0",
     python_requires=">=3.10",
     description="Allows connections between DSO, AGR and CRO using the Shapeshifter (UFTP) protocol.",
     packages=[
         "shapeshifter_uftp",
         "shapeshifter_uftp.uftp",
         "shapeshifter_uftp.client",
         "shapeshifter_uftp.service",
     ],
     install_requires=[
-        "xsdata[lxml]==24.3.1",
+        "xsdata[lxml]==24.4",
         "pynacl==1.5.0",
         "dnspython==2.6.1",
-        "fastapi<0.100",
-        "fastapi-xml==1.0.0b1",
+        "fastapi==0.110",
+        "fastapi-xml==1.1.0",
         "requests",
         "uvicorn",
         "termcolor",
     ],
     extras_require={
         "dev": [
             "xmlschema",
```

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/__init__.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/__init__.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/cli.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/cli.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/__init__.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/__init__.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/agr_cro_client.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/agr_cro_client.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/agr_dso_client.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/agr_dso_client.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/base_client.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from datetime import datetime, timezone
 import sched
 import time
+from datetime import datetime, timezone
 from queue import Queue
-from threading import Thread, Event
+from threading import Event, Thread
 from uuid import uuid4
+
 import requests
-from ..uftp import PayloadMessage, PayloadMessageResponse, SignedMessage
-from ..logging import logger
-from ..exceptions import ClientTransportException
+
 from .. import transport
+from ..exceptions import ClientTransportException
+from ..logging import logger
+from ..uftp import PayloadMessage, PayloadMessageResponse, SignedMessage
 
 
 class ShapeshifterClient():
     """
     Basis for all Shapeshifter client.
     """
```

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/cro_agr_client.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/cro_agr_client.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/cro_dso_client.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/cro_dso_client.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/dso_agr_client.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/dso_agr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,12 @@
+from ..uftp import (DPrognosisResponse, FlexOfferResponse,
+                    FlexOfferRevocationResponse, FlexOrder, FlexRequest,
+                    FlexReservationUpdate, FlexSettlement, MeteringResponse,
+                    PayloadMessageResponse)
 from .base_client import ShapeshifterClient
-from ..uftp import (
-    DPrognosisResponse,
-    FlexRequest,
-    FlexOfferResponse,
-    FlexOrder,
-    FlexReservationUpdate,
-    FlexOfferRevocationResponse,
-    FlexSettlement,
-    PayloadMessageResponse,
-    MeteringResponse,
-)
 
 
 class ShapeshifterDsoAgrClient(ShapeshifterClient):
     """
     Client that allows the DSO to connect to the Aggregator.
     """
```

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/client/dso_cro_client.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/client/dso_cro_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from ..uftp import DsoPortfolioQuery, DsoPortfolioUpdate
 from .base_client import ShapeshifterClient
-from ..uftp import DsoPortfolioUpdate, DsoPortfolioQuery
 
 
 class ShapeshifterDsoCroClient(ShapeshifterClient):
     """
     Client that allows the DSO to connect to the CRO.
     """
```

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/exceptions.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/logging.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/logging.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/agr_service.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/agr_service.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/base_service.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/base_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,26 @@
+import re
 from datetime import datetime, timezone
 from queue import Queue
-from uuid import uuid4
-from time import sleep
 from threading import Thread
-import re
+from time import sleep
+from uuid import uuid4
 
+import uvicorn
 from fastapi import FastAPI
 from fastapi.exceptions import HTTPException
-from fastapi_xml import XmlAppResponse, NonJsonRoute
-import uvicorn
+from fastapi_xml import XmlAppResponse, XmlRoute
 
+from .. import transport
 from ..client import client_map
-from ..uftp import (
-    SignedMessage,
-    PayloadMessage,
-    PayloadMessageResponse,
-    AcceptedRejected,
-)
-from ..exceptions import (
-    FunctionalException,
-    TransportException,
-    InvalidSenderException,
-    InvalidMessageException,
-)
+from ..exceptions import (FunctionalException, InvalidMessageException,
+                          InvalidSenderException, TransportException)
 from ..logging import logger
-from .. import transport
+from ..uftp import (AcceptedRejected, PayloadMessage, PayloadMessageResponse,
+                    SignedMessage)
 
 
 class ShapeshifterService():
     """
     Basis for all Shapeshifter Services. Defines the web service, the
     message ingestion, the post-processing queue mechanics, and
     threading and context options.
@@ -84,15 +76,15 @@
         # using well-known DNS names.
         self.endpoint_lookup_function = endpoint_lookup_function or transport.get_endpoint
 
         # The FastAPI web app takes care of routing messages to the
         # (one) endpoint, and by virtue of FastAPI-XML convert the
         # python-friendly objects into XML and vice versa.
         self.app = FastAPI(default_response_class=XmlAppResponse)
-        self.app.router.route_class = NonJsonRoute
+        self.app.router.route_class = XmlRoute
         self.app.router.add_api_route(
             path,
             endpoint=self._receive_message,
             response_model=SignedMessage,
             methods=["POST"],
             status_code=200,
         )
```

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/cro_service.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/cro_service.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/service/dso_service.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/service/dso_service.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/transport.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/transport.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/__init__.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/__init__.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/agr_cro.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/agr_cro.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/agr_dso.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/agr_dso.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/common.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/common.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/cro_dso.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/cro_dso.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/metering.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/metering.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp/uftp/validations.py` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp/uftp/validations.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/shapeshifter_uftp.egg-info/SOURCES.txt` & `shapeshifter-uftp-1.2.0/shapeshifter_uftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_cli.py` & `shapeshifter-uftp-1.2.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_client_errors.py` & `shapeshifter-uftp-1.2.0/test/test_client_errors.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_client_with_workers.py` & `shapeshifter-uftp-1.2.0/test/test_client_with_workers.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_clients_from_service.py` & `shapeshifter-uftp-1.2.0/test/test_clients_from_service.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_communications.py` & `shapeshifter-uftp-1.2.0/test/test_communications.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_default_responses.py` & `shapeshifter-uftp-1.2.0/test/test_default_responses.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_message_destination.py` & `shapeshifter-uftp-1.2.0/test/test_message_destination.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_presence_of_client_methods.py` & `shapeshifter-uftp-1.2.0/test/test_presence_of_client_methods.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_presence_of_service_methods.py` & `shapeshifter-uftp-1.2.0/test/test_presence_of_service_methods.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_roundtrip_serialization.py` & `shapeshifter-uftp-1.2.0/test/test_roundtrip_serialization.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_seal_and_unseal.py` & `shapeshifter-uftp-1.2.0/test/test_seal_and_unseal.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_service_errors.py` & `shapeshifter-uftp-1.2.0/test/test_service_errors.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_ttl_cache.py` & `shapeshifter-uftp-1.2.0/test/test_ttl_cache.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_validations.py` & `shapeshifter-uftp-1.2.0/test/test_validations.py`

 * *Files identical despite different names*

### Comparing `shapeshifter-uftp-1.1.2/test/test_xml_schema_compliance.py` & `shapeshifter-uftp-1.2.0/test/test_xml_schema_compliance.py`

 * *Files identical despite different names*

