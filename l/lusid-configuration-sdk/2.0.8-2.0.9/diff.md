# Comparing `tmp/lusid_configuration_sdk-2.0.8.tar.gz` & `tmp/lusid_configuration_sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_configuration_sdk-2.0.8.tar", max compression
+gzip compressed data, was "lusid_configuration_sdk-2.0.9.tar", max compression
```

## Comparing `lusid_configuration_sdk-2.0.8.tar` & `lusid_configuration_sdk-2.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     9255 2024-01-30 17:12:16.045914 lusid_configuration_sdk-2.0.8/README.md
--rw-r--r--   0        0        0     2940 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/__init__.py
--rw-r--r--   0        0        0      212 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/api/__init__.py
--rw-r--r--   0        0        0     7563 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/api/application_metadata_api.py
--rw-r--r--   0        0        0   138071 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/api/configuration_sets_api.py
--rw-r--r--   0        0        0    30832 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/api_client.py
--rw-r--r--   0        0        0      852 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/api_response.py
--rw-r--r--   0        0        0    14483 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/configuration.py
--rw-r--r--   0        0        0     5351 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/exceptions.py
--rw-r--r--   0        0        0      304 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/__init__.py
--rw-r--r--   0        0        0    30704 2024-01-30 17:12:16.065914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/api_client.py
--rw-r--r--   0        0        0     9813 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8032 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/api_configuration.py
--rw-r--r--   0        0        0     6888 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12712 2024-01-30 17:12:16.065914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/rest.py
--rw-r--r--   0        0        0    11578 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-01-30 17:12:16.065914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3891 2024-01-30 17:12:16.065914 lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     2207 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/__init__.py
--rw-r--r--   0        0        0     3927 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/access_controlled_action.py
--rw-r--r--   0        0        0     4870 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2079 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/action_id.py
--rw-r--r--   0        0        0     4736 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_item.py
--rw-r--r--   0        0        0     3480 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_item_summary.py
--rw-r--r--   0        0        0     5223 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_set.py
--rw-r--r--   0        0        0     3090 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_set_summary.py
--rw-r--r--   0        0        0     4233 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/create_configuration_item.py
--rw-r--r--   0        0        0     2826 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/create_configuration_set.py
--rw-r--r--   0        0        0     3194 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/id_selector_definition.py
--rw-r--r--   0        0        0     3119 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2271 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/link.py
--rw-r--r--   0        0        0     3866 2024-01-30 17:12:16.062914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4702 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3408 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/personal_access_token.py
--rw-r--r--   0        0        0     2086 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_id.py
--rw-r--r--   0        0        0     4274 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4189 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_configuration_item.py
--rw-r--r--   0        0        0     4177 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_configuration_set.py
--rw-r--r--   0        0        0     4262 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_configuration_set_summary.py
--rw-r--r--   0        0        0     2778 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/update_configuration_item.py
--rw-r--r--   0        0        0     2307 2024-01-30 17:12:16.063914 lusid_configuration_sdk-2.0.8/lusid_configuration/models/update_configuration_set.py
--rw-r--r--   0        0        0        0 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/py.typed
--rw-r--r--   0        0        0    10046 2024-01-30 17:12:16.064914 lusid_configuration_sdk-2.0.8/lusid_configuration/rest.py
--rw-r--r--   0        0        0      905 2024-01-30 17:12:16.053914 lusid_configuration_sdk-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    10345 1970-01-01 00:00:00.000000 lusid_configuration_sdk-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     9255 2024-02-01 16:09:12.248072 lusid_configuration_sdk-2.0.9/README.md
+-rw-r--r--   0        0        0     2940 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/__init__.py
+-rw-r--r--   0        0        0      212 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/api/__init__.py
+-rw-r--r--   0        0        0     7563 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/api/application_metadata_api.py
+-rw-r--r--   0        0        0   138071 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/api/configuration_sets_api.py
+-rw-r--r--   0        0        0    30832 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/api_client.py
+-rw-r--r--   0        0        0      852 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/api_response.py
+-rw-r--r--   0        0        0    14483 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/configuration.py
+-rw-r--r--   0        0        0     5351 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/exceptions.py
+-rw-r--r--   0        0        0      304 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/__init__.py
+-rw-r--r--   0        0        0    30704 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client.py
+-rw-r--r--   0        0        0     9813 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8032 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6888 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2055 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12712 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/rest.py
+-rw-r--r--   0        0        0    11578 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3891 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     2207 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/__init__.py
+-rw-r--r--   0        0        0     3927 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4870 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2079 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/action_id.py
+-rw-r--r--   0        0        0     4736 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item.py
+-rw-r--r--   0        0        0     3480 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item_summary.py
+-rw-r--r--   0        0        0     5223 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set.py
+-rw-r--r--   0        0        0     3090 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set_summary.py
+-rw-r--r--   0        0        0     4233 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_item.py
+-rw-r--r--   0        0        0     2826 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_set.py
+-rw-r--r--   0        0        0     3194 2024-02-01 16:09:12.244072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3119 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2271 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/link.py
+-rw-r--r--   0        0        0     3866 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4702 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3408 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/personal_access_token.py
+-rw-r--r--   0        0        0     2086 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_id.py
+-rw-r--r--   0        0        0     4274 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4189 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_item.py
+-rw-r--r--   0        0        0     4177 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set.py
+-rw-r--r--   0        0        0     4262 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set_summary.py
+-rw-r--r--   0        0        0     2778 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_item.py
+-rw-r--r--   0        0        0     2307 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_set.py
+-rw-r--r--   0        0        0        0 2024-02-01 16:09:12.245072 lusid_configuration_sdk-2.0.9/lusid_configuration/py.typed
+-rw-r--r--   0        0        0    10046 2024-02-01 16:09:12.246072 lusid_configuration_sdk-2.0.9/lusid_configuration/rest.py
+-rw-r--r--   0        0        0      905 2024-02-01 16:09:12.248072 lusid_configuration_sdk-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10345 1970-01-01 00:00:00.000000 lusid_configuration_sdk-2.0.9/PKG-INFO
```

### Comparing `lusid_configuration_sdk-2.0.8/README.md` & `lusid_configuration_sdk-2.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-configuration-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.491
-- Package version: 2.0.8
+- API version: 0.1.492
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/__init__.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/api/application_metadata_api.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/api/configuration_sets_api.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/api/configuration_sets_api.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/api_client.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/api_response.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/configuration.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_configuration-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.491\n"\
+               "Version of the API: 0.1.492\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/exceptions.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/api_client.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/api_client_factory.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/api_configuration.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/configuration_loaders.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/proxy_config.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/refreshing_token.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/rest.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/retry.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/socket_keep_alive.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/extensions/tcp_keep_alive_connector.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/__init__.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/access_controlled_action.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/access_controlled_resource.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/action_id.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_item.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_item_summary.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_item_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_set.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/configuration_set_summary.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/configuration_set_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/create_configuration_item.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/create_configuration_set.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/create_configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/id_selector_definition.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/identifier_part_schema.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/link.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/lusid_problem_details.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/lusid_validation_problem_details.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/personal_access_token.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_id.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_access_controlled_resource.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_configuration_item.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_configuration_set.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/resource_list_of_configuration_set_summary.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/resource_list_of_configuration_set_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/update_configuration_item.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_item.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/models/update_configuration_set.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/models/update_configuration_set.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/lusid_configuration/rest.py` & `lusid_configuration_sdk-2.0.9/lusid_configuration/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_configuration_sdk-2.0.8/pyproject.toml` & `lusid_configuration_sdk-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-configuration-sdk"
-version = "2.0.8"
+version = "2.0.9"
 description = "FINBOURNE ConfigurationService API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/configuration-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE ConfigurationService API", "lusid-configuration-sdk"]
 packages = [
```

### Comparing `lusid_configuration_sdk-2.0.8/PKG-INFO` & `lusid_configuration_sdk-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-configuration-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: FINBOURNE ConfigurationService API
 Home-page: https://github.com/finbourne/configuration-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE ConfigurationService API,lusid-configuration-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-configuration-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.491
-- Package version: 2.0.8
+- API version: 0.1.492
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

