# Comparing `tmp/finbourne_insights_sdk-2.0.8.tar.gz` & `tmp/finbourne_insights_sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_insights_sdk-2.0.8.tar", max compression
+gzip compressed data, was "finbourne_insights_sdk-2.0.9.tar", max compression
```

## Comparing `finbourne_insights_sdk-2.0.8.tar` & `finbourne_insights_sdk-2.0.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    10647 2024-02-21 16:41:34.053582 finbourne_insights_sdk-2.0.8/README.md
--rw-r--r--   0        0        0     3697 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/__init__.py
--rw-r--r--   0        0        0      395 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/api/__init__.py
--rw-r--r--   0        0        0    24453 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/api/access_evaluations_api.py
--rw-r--r--   0        0        0     7547 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/api/application_metadata_api.py
--rw-r--r--   0        0        0    24163 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/api/auditing_api.py
--rw-r--r--   0        0        0    35942 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/api/requests_api.py
--rw-r--r--   0        0        0    36142 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/api/vendor_logs_api.py
--rw-r--r--   0        0        0    30813 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/api_client.py
--rw-r--r--   0        0        0      852 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/api_response.py
--rw-r--r--   0        0        0    14459 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/configuration.py
--rw-r--r--   0        0        0     5339 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/exceptions.py
--rw-r--r--   0        0        0      302 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/__init__.py
--rw-r--r--   0        0        0    30684 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/api_client.py
--rw-r--r--   0        0        0     9803 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8117 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/api_configuration.py
--rw-r--r--   0        0        0     6812 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/rest.py
--rw-r--r--   0        0        0    11577 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2024-02-21 16:41:34.051582 finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     2789 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/__init__.py
--rw-r--r--   0        0        0     3912 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/access_controlled_action.py
--rw-r--r--   0        0        0     4855 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/access_controlled_resource.py
--rw-r--r--   0        0        0    11912 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/access_evaluation_log.py
--rw-r--r--   0        0        0     2067 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/action_id.py
--rw-r--r--   0        0        0     3753 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_data.py
--rw-r--r--   0        0        0     2216 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_data_summary.py
--rw-r--r--   0        0        0     3448 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_entry.py
--rw-r--r--   0        0        0     2093 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_entry_note.py
--rw-r--r--   0        0        0     2776 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_process.py
--rw-r--r--   0        0        0     3036 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_process_summary.py
--rw-r--r--   0        0        0     2116 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/bucket.py
--rw-r--r--   0        0        0     2516 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/create_audit_entry.py
--rw-r--r--   0        0        0     2594 2024-02-21 16:41:34.047582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/histogram.py
--rw-r--r--   0        0        0     3181 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/id_selector_definition.py
--rw-r--r--   0        0        0     3106 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2259 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/link.py
--rw-r--r--   0        0        0     3854 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4690 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3209 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/problem_details.py
--rw-r--r--   0        0        0     5507 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/request.py
--rw-r--r--   0        0        0     8265 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/request_log.py
--rw-r--r--   0        0        0     2371 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource.py
--rw-r--r--   0        0        0     4260 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4200 2024-02-21 16:41:34.048582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_of_audit_process_summary.py
--rw-r--r--   0        0        0     4735 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
--rw-r--r--   0        0        0     4635 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
--rw-r--r--   0        0        0     4624 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
--rw-r--r--   0        0        0     5045 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/response.py
--rw-r--r--   0        0        0     2910 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/scrollable_collection_of_audit_entry.py
--rw-r--r--   0        0        0     4517 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/vendor_log.py
--rw-r--r--   0        0        0     2794 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/vendor_request.py
--rw-r--r--   0        0        0     2820 2024-02-21 16:41:34.049582 finbourne_insights_sdk-2.0.8/finbourne_insights/models/vendor_response.py
--rw-r--r--   0        0        0        0 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/py.typed
--rw-r--r--   0        0        0    10033 2024-02-21 16:41:34.050582 finbourne_insights_sdk-2.0.8/finbourne_insights/rest.py
--rw-r--r--   0        0        0      872 2024-02-21 16:41:34.053582 finbourne_insights_sdk-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    11701 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10647 2024-02-22 10:34:34.037325 finbourne_insights_sdk-2.0.9/README.md
+-rw-r--r--   0        0        0     3697 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/__init__.py
+-rw-r--r--   0        0        0      395 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/__init__.py
+-rw-r--r--   0        0        0    24453 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/access_evaluations_api.py
+-rw-r--r--   0        0        0     7547 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/application_metadata_api.py
+-rw-r--r--   0        0        0    24163 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/auditing_api.py
+-rw-r--r--   0        0        0    35942 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/requests_api.py
+-rw-r--r--   0        0        0    36142 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/api/vendor_logs_api.py
+-rw-r--r--   0        0        0    30813 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/api_client.py
+-rw-r--r--   0        0        0      852 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/api_response.py
+-rw-r--r--   0        0        0    14459 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/configuration.py
+-rw-r--r--   0        0        0     5339 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/exceptions.py
+-rw-r--r--   0        0        0      302 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/__init__.py
+-rw-r--r--   0        0        0    30684 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client.py
+-rw-r--r--   0        0        0     9803 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8117 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6812 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     2789 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/__init__.py
+-rw-r--r--   0        0        0     3912 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4855 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_resource.py
+-rw-r--r--   0        0        0    11912 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_evaluation_log.py
+-rw-r--r--   0        0        0     2067 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/action_id.py
+-rw-r--r--   0        0        0     3753 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data.py
+-rw-r--r--   0        0        0     2216 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data_summary.py
+-rw-r--r--   0        0        0     3448 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry.py
+-rw-r--r--   0        0        0     2093 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry_note.py
+-rw-r--r--   0        0        0     2776 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process.py
+-rw-r--r--   0        0        0     3036 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process_summary.py
+-rw-r--r--   0        0        0     2116 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/bucket.py
+-rw-r--r--   0        0        0     2516 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/create_audit_entry.py
+-rw-r--r--   0        0        0     2594 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/histogram.py
+-rw-r--r--   0        0        0     3181 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3106 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2259 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/link.py
+-rw-r--r--   0        0        0     3854 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4690 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3209 2024-02-22 10:34:34.033325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/problem_details.py
+-rw-r--r--   0        0        0     5507 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/request.py
+-rw-r--r--   0        0        0     8265 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/request_log.py
+-rw-r--r--   0        0        0     2371 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource.py
+-rw-r--r--   0        0        0     4260 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4200 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_audit_process_summary.py
+-rw-r--r--   0        0        0     4735 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py
+-rw-r--r--   0        0        0     4635 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_request_log.py
+-rw-r--r--   0        0        0     4624 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py
+-rw-r--r--   0        0        0     5045 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/response.py
+-rw-r--r--   0        0        0     2910 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/scrollable_collection_of_audit_entry.py
+-rw-r--r--   0        0        0     4517 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_log.py
+-rw-r--r--   0        0        0     2794 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_request.py
+-rw-r--r--   0        0        0     2820 2024-02-22 10:34:34.034325 finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_response.py
+-rw-r--r--   0        0        0        0 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/py.typed
+-rw-r--r--   0        0        0    10033 2024-02-22 10:34:34.035325 finbourne_insights_sdk-2.0.9/finbourne_insights/rest.py
+-rw-r--r--   0        0        0      872 2024-02-22 10:34:34.037325 finbourne_insights_sdk-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11701 1970-01-01 00:00:00.000000 finbourne_insights_sdk-2.0.9/PKG-INFO
```

### Comparing `finbourne_insights_sdk-2.0.8/README.md` & `finbourne_insights_sdk-2.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.758
-- Package version: 2.0.8
+- API version: 0.0.759
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/__init__.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/api/access_evaluations_api.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/api/access_evaluations_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/api/application_metadata_api.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/api/auditing_api.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/api/auditing_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/api/requests_api.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/api/requests_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/api/vendor_logs_api.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/api/vendor_logs_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/api_client.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/api_response.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/configuration.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_insights-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.758\n"\
+               "Version of the API: 0.0.759\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/exceptions.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/api_client.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/api_client_factory.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/api_configuration.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/configuration_loaders.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/proxy_config.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/refreshing_token.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/rest.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/retry.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/socket_keep_alive.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/extensions/tcp_keep_alive_connector.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/__init__.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/access_controlled_action.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/access_controlled_resource.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/access_evaluation_log.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/access_evaluation_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/action_id.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_data.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_data_summary.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_data_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_entry.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_entry_note.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_entry_note.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_process.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/audit_process_summary.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/audit_process_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/bucket.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/bucket.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/create_audit_entry.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/create_audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/histogram.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/histogram.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/id_selector_definition.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/identifier_part_schema.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/link.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/lusid_problem_details.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/lusid_validation_problem_details.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/problem_details.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/request.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/request.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/request_log.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/request_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_of_access_controlled_resource.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_of_audit_process_summary.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_of_audit_process_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_access_evaluation_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_with_histogram_of_request_log.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_request_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/resource_list_with_histogram_of_vendor_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/response.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/scrollable_collection_of_audit_entry.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/scrollable_collection_of_audit_entry.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/vendor_log.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_log.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/vendor_request.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/models/vendor_response.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/models/vendor_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/finbourne_insights/rest.py` & `finbourne_insights_sdk-2.0.9/finbourne_insights/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_insights_sdk-2.0.8/pyproject.toml` & `finbourne_insights_sdk-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-insights-sdk"
-version = "2.0.8"
+version = "2.0.9"
 description = "FINBOURNE Insights API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/insights-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Insights API", "finbourne-insights-sdk"]
 packages = [
```

### Comparing `finbourne_insights_sdk-2.0.8/PKG-INFO` & `finbourne_insights_sdk-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-insights-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: FINBOURNE Insights API
 Home-page: https://github.com/finbourne/insights-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Insights API,finbourne-insights-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-insights-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.758
-- Package version: 2.0.8
+- API version: 0.0.759
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

