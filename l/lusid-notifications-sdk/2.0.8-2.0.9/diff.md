# Comparing `tmp/lusid_notifications_sdk-2.0.8.tar.gz` & `tmp/lusid_notifications_sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_notifications_sdk-2.0.8.tar", max compression
+gzip compressed data, was "lusid_notifications_sdk-2.0.9.tar", max compression
```

## Comparing `lusid_notifications_sdk-2.0.8.tar` & `lusid_notifications_sdk-2.0.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     9297 2024-01-12 17:05:32.761026 lusid_notifications_sdk-2.0.8/README.md
--rw-r--r--   0        0        0     4665 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/__init__.py
--rw-r--r--   0        0        0      473 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api/__init__.py
--rw-r--r--   0        0        0     7556 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0        0        0    13216 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0        0        0    14128 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api/event_types_api.py
--rw-r--r--   0        0        0     8478 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api/manual_event_api.py
--rw-r--r--   0        0        0    45083 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api/notifications_api.py
--rw-r--r--   0        0        0    44721 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0        0        0    30825 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api_client.py
--rw-r--r--   0        0        0      852 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/api_response.py
--rw-r--r--   0        0        0    14474 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/configuration.py
--rw-r--r--   0        0        0     5344 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/exceptions.py
--rw-r--r--   0        0        0      304 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/__init__.py
--rw-r--r--   0        0        0    30697 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/api_client.py
--rw-r--r--   0        0        0     9813 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8032 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/api_configuration.py
--rw-r--r--   0        0        0     6888 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12712 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/rest.py
--rw-r--r--   0        0        0    11578 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3891 2024-01-12 17:05:32.758026 lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3671 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/__init__.py
--rw-r--r--   0        0        0     3920 2024-01-12 17:05:32.753026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0        0        0     4863 2024-01-12 17:05:32.753026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2072 2024-01-12 17:05:32.753026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/action_id.py
--rw-r--r--   0        0        0     3443 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/amazon_sqs_notification_type.py
--rw-r--r--   0        0        0     3922 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/amazon_sqs_notification_type_response.py
--rw-r--r--   0        0        0     2519 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/attempt.py
--rw-r--r--   0        0        0     2412 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/attempt_status.py
--rw-r--r--   0        0        0     4248 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/create_notification_request.py
--rw-r--r--   0        0        0     5201 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/create_subscription.py
--rw-r--r--   0        0        0     3813 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/delivery.py
--rw-r--r--   0        0        0     5205 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/email_notification_type.py
--rw-r--r--   0        0        0     4817 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/email_notification_type_response.py
--rw-r--r--   0        0        0     2459 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/event_field_definition.py
--rw-r--r--   0        0        0     5524 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0        0        0     3187 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0        0        0     3112 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2264 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/link.py
--rw-r--r--   0        0        0     3859 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4695 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2530 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event.py
--rw-r--r--   0        0        0     3129 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event_body.py
--rw-r--r--   0        0        0     3196 2024-01-12 17:05:32.754026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event_header.py
--rw-r--r--   0        0        0     2188 2024-01-12 17:05:32.755026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event_request.py
--rw-r--r--   0        0        0     3241 2024-01-12 17:05:32.755026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0        0        0     5023 2024-01-12 17:05:32.755026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification.py
--rw-r--r--   0        0        0     2404 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification_status.py
--rw-r--r--   0        0        0     7237 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification_type.py
--rw-r--r--   0        0        0     7796 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification_type_response.py
--rw-r--r--   0        0        0     2079 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_id.py
--rw-r--r--   0        0        0     4267 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4073 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0        0        0     4159 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0        0        0     4121 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0        0        0     4121 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0        0        0     2911 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/sms_notification_type.py
--rw-r--r--   0        0        0     3004 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/sms_notification_type_response.py
--rw-r--r--   0        0        0     4770 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/subscription.py
--rw-r--r--   0        0        0     3701 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/update_notification_request.py
--rw-r--r--   0        0        0     4862 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/update_subscription.py
--rw-r--r--   0        0        0     5542 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/webhook_notification_type.py
--rw-r--r--   0        0        0     5672 2024-01-12 17:05:32.756026 lusid_notifications_sdk-2.0.8/lusid_notifications/models/webhook_notification_type_response.py
--rw-r--r--   0        0        0        0 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/py.typed
--rw-r--r--   0        0        0    10039 2024-01-12 17:05:32.757026 lusid_notifications_sdk-2.0.8/lusid_notifications/rest.py
--rw-r--r--   0        0        0      891 2024-01-12 17:05:32.761026 lusid_notifications_sdk-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    10373 1970-01-01 00:00:00.000000 lusid_notifications_sdk-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     9297 2024-01-16 10:29:34.453622 lusid_notifications_sdk-2.0.9/README.md
+-rw-r--r--   0        0        0     4665 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/__init__.py
+-rw-r--r--   0        0        0      473 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/__init__.py
+-rw-r--r--   0        0        0     7556 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0        0        0    13216 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0        0        0    14128 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0        0        0     8478 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/manual_event_api.py
+-rw-r--r--   0        0        0    45083 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0        0        0    44721 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0        0        0    30825 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api_client.py
+-rw-r--r--   0        0        0      852 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/api_response.py
+-rw-r--r--   0        0        0    14474 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/configuration.py
+-rw-r--r--   0        0        0     5344 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/exceptions.py
+-rw-r--r--   0        0        0      304 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/__init__.py
+-rw-r--r--   0        0        0    30697 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client.py
+-rw-r--r--   0        0        0     9813 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8032 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6888 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2055 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12712 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/rest.py
+-rw-r--r--   0        0        0    11578 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3891 2024-01-16 10:29:34.450622 lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     3671 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/__init__.py
+-rw-r--r--   0        0        0     3920 2024-01-16 10:29:34.444623 lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4863 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2072 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/action_id.py
+-rw-r--r--   0        0        0     3443 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type.py
+-rw-r--r--   0        0        0     3922 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0        0        0     2519 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt.py
+-rw-r--r--   0        0        0     2412 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0        0        0     4248 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_notification_request.py
+-rw-r--r--   0        0        0     5201 2024-01-16 10:29:34.446622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0        0        0     3813 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/delivery.py
+-rw-r--r--   0        0        0     5205 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type.py
+-rw-r--r--   0        0        0     4817 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type_response.py
+-rw-r--r--   0        0        0     2459 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_field_definition.py
+-rw-r--r--   0        0        0     5524 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0        0        0     3187 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3112 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2264 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/link.py
+-rw-r--r--   0        0        0     3859 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4695 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2530 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event.py
+-rw-r--r--   0        0        0     3129 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_body.py
+-rw-r--r--   0        0        0     3196 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_header.py
+-rw-r--r--   0        0        0     2188 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_request.py
+-rw-r--r--   0        0        0     3241 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0        0        0     5023 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification.py
+-rw-r--r--   0        0        0     2404 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_status.py
+-rw-r--r--   0        0        0     7237 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type.py
+-rw-r--r--   0        0        0     7796 2024-01-16 10:29:34.447622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type_response.py
+-rw-r--r--   0        0        0     2079 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_id.py
+-rw-r--r--   0        0        0     4267 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4073 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0        0        0     4159 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0        0        0     4121 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0        0        0     4121 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0        0        0     2911 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type.py
+-rw-r--r--   0        0        0     3004 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type_response.py
+-rw-r--r--   0        0        0     4770 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/subscription.py
+-rw-r--r--   0        0        0     3701 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_notification_request.py
+-rw-r--r--   0        0        0     4862 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0        0        0     5542 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type.py
+-rw-r--r--   0        0        0     5672 2024-01-16 10:29:34.448622 lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type_response.py
+-rw-r--r--   0        0        0        0 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/py.typed
+-rw-r--r--   0        0        0    10039 2024-01-16 10:29:34.449622 lusid_notifications_sdk-2.0.9/lusid_notifications/rest.py
+-rw-r--r--   0        0        0      891 2024-01-16 10:29:34.453622 lusid_notifications_sdk-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10373 1970-01-01 00:00:00.000000 lusid_notifications_sdk-2.0.9/PKG-INFO
```

### Comparing `lusid_notifications_sdk-2.0.8/README.md` & `lusid_notifications_sdk-2.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.905
-- Package version: 2.0.8
+- API version: 0.1.906
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/__init__.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api/application_metadata_api.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api/deliveries_api.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api/deliveries_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api/event_types_api.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api/event_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api/manual_event_api.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api/manual_event_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api/notifications_api.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api/subscriptions_api.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api/subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api_client.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/api_response.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/configuration.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_notifications-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.905\n"\
+               "Version of the API: 0.1.906\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/exceptions.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/api_client.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/api_client_factory.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/api_configuration.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/configuration_loaders.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/proxy_config.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/refreshing_token.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/rest.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/retry.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/socket_keep_alive.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/extensions/tcp_keep_alive_connector.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/__init__.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/access_controlled_action.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/access_controlled_resource.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/action_id.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/amazon_sqs_notification_type.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/amazon_sqs_notification_type_response.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/amazon_sqs_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/attempt.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/attempt_status.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/attempt_status.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/create_notification_request.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_notification_request.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/create_subscription.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/create_subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/delivery.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/delivery.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/email_notification_type.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/email_notification_type_response.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/email_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/event_field_definition.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/event_type_schema.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/event_type_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/id_selector_definition.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/identifier_part_schema.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/link.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/lusid_problem_details.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event_body.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_body.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event_header.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_header.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/manual_event_request.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/manual_event_request.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/matching_pattern.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/matching_pattern.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification_status.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_status.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification_type.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/notification_type_response.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_id.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_delivery.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_delivery.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_event_type_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_notification.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_notification.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/resource_list_of_subscription.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/resource_list_of_subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/sms_notification_type.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/sms_notification_type_response.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/sms_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/subscription.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/update_notification_request.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_notification_request.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/update_subscription.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/update_subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/webhook_notification_type.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/models/webhook_notification_type_response.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/models/webhook_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/lusid_notifications/rest.py` & `lusid_notifications_sdk-2.0.9/lusid_notifications/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.0.8/pyproject.toml` & `lusid_notifications_sdk-2.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-notifications-sdk"
-version = "2.0.8"
+version = "2.0.9"
 description = "FINBOURNE Notifications API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/notifications-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Notifications API", "lusid-notifications-sdk"]
 packages = [
```

### Comparing `lusid_notifications_sdk-2.0.8/PKG-INFO` & `lusid_notifications_sdk-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-notifications-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: FINBOURNE Notifications API
 Home-page: https://github.com/finbourne/notifications-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Notifications API,lusid-notifications-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.905
-- Package version: 2.0.8
+- API version: 0.1.906
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

