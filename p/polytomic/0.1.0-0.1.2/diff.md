# Comparing `tmp/polytomic-0.1.0.tar.gz` & `tmp/polytomic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytomic-0.1.0.tar", max compression
+gzip compressed data, was "polytomic-0.1.2.tar", max compression
```

## Comparing `polytomic-0.1.0.tar` & `polytomic-0.1.2.tar`

### file list

```diff
@@ -1,156 +1,181 @@
--rw-r--r--   0        0        0     1066 2024-02-14 03:19:27.701362 polytomic-0.1.0/LICENSE
--rw-r--r--   0        0        0     1860 2024-02-14 03:19:27.701362 polytomic-0.1.0/README.md
--rw-r--r--   0        0        0      404 2024-02-14 03:19:27.701362 polytomic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6123 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/__init__.py
--rw-r--r--   0        0        0     4497 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/client.py
--rw-r--r--   0        0        0      519 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/core/__init__.py
--rw-r--r--   0        0        0      426 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/core/api_error.py
--rw-r--r--   0        0        0     2200 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      161 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/environment.py
--rw-r--r--   0        0        0      148 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/errors/__init__.py
--rw-r--r--   0        0        0      294 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/py.typed
--rw-r--r--   0        0        0      498 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/__init__.py
--rw-r--r--   0        0        0      145 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/bulk_sync/__init__.py
--rw-r--r--   0        0        0    43724 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/bulk_sync/client.py
--rw-r--r--   0        0        0      136 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/bulk_sync/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/bulk_sync/resources/executions/__init__.py
--rw-r--r--   0        0        0    10324 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/bulk_sync/resources/executions/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/bulk_sync/resources/schemas/__init__.py
--rw-r--r--   0        0        0    10374 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/bulk_sync/resources/schemas/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/connections/__init__.py
--rw-r--r--   0        0        0    40316 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/connections/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/events/__init__.py
--rw-r--r--   0        0        0     8259 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/events/client.py
--rw-r--r--   0        0        0      247 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/__init__.py
--rw-r--r--   0        0        0    36806 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/client.py
--rw-r--r--   0        0        0      116 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/resources/executions/__init__.py
--rw-r--r--   0        0        0     6300 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/resources/executions/client.py
--rw-r--r--   0        0        0      263 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/types/__init__.py
--rw-r--r--   0        0        0     1179 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/types/v_2_create_sync_request_mode.py
--rw-r--r--   0        0        0     1179 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/model_sync/types/v_2_update_sync_request_mode.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/models/__init__.py
--rw-r--r--   0        0        0    22128 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/models/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/organization/__init__.py
--rw-r--r--   0        0        0    19225 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/organization/client.py
--rw-r--r--   0        0        0      137 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/permissions/__init__.py
--rw-r--r--   0        0        0      857 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/permissions/client.py
--rw-r--r--   0        0        0      128 2024-02-14 03:19:27.701362 polytomic-0.1.0/src/polytomic/resources/permissions/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/permissions/resources/policies/__init__.py
--rw-r--r--   0        0        0    16844 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/permissions/resources/policies/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/permissions/resources/roles/__init__.py
--rw-r--r--   0        0        0    14536 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/permissions/resources/roles/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/schemas/__init__.py
--rw-r--r--   0        0        0     3722 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/schemas/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/users/__init__.py
--rw-r--r--   0        0        0    20810 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/users/client.py
--rw-r--r--   0        0        0       65 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/webhooks/__init__.py
--rw-r--r--   0        0        0    17310 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/resources/webhooks/client.py
--rw-r--r--   0        0        0     8801 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/__init__.py
--rw-r--r--   0        0        0     1047 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/bulk_schedule.py
--rw-r--r--   0        0        0      122 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/label_label.py
--rw-r--r--   0        0        0     1223 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/rest_err_response.py
--rw-r--r--   0        0        0     1015 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/schema_association.py
--rw-r--r--   0        0        0     1377 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/sync_destination_properties.py
--rw-r--r--   0        0        0      972 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_activate_sync_envelope.py
--rw-r--r--   0        0        0      879 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_activate_sync_input.py
--rw-r--r--   0        0        0      926 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_activate_sync_output.py
--rw-r--r--   0        0        0      891 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_api_key_response.py
--rw-r--r--   0        0        0      962 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_api_key_response_envelope.py
--rw-r--r--   0        0        0     1027 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_dest.py
--rw-r--r--   0        0        0      954 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_dest_envelope.py
--rw-r--r--   0        0        0      979 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_list_envelope.py
--rw-r--r--   0        0        0     1444 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_response.py
--rw-r--r--   0        0        0      970 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_response_envelope.py
--rw-r--r--   0        0        0      946 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_configuration_value.py
--rw-r--r--   0        0        0     1013 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_list_response_envelope.py
--rw-r--r--   0        0        0     1003 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_meta.py
--rw-r--r--   0        0        0     1185 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_meta_response.py
--rw-r--r--   0        0        0      996 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_response_envelope.py
--rw-r--r--   0        0        0     1269 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_response_schema.py
--rw-r--r--   0        0        0     1100 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_type.py
--rw-r--r--   0        0        0      982 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_type_response_envelope.py
--rw-r--r--   0        0        0      925 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_connection_type_schema.py
--rw-r--r--   0        0        0     1021 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_create_connection_response_envelope.py
--rw-r--r--   0        0        0     1538 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_create_connection_response_schema.py
--rw-r--r--   0        0        0     1036 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_event.py
--rw-r--r--   0        0        0      907 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_event_types_envelope.py
--rw-r--r--   0        0        0      938 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_events_envelope.py
--rw-r--r--   0        0        0      990 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_execution_counts.py
--rw-r--r--   0        0        0      978 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_filter.py
--rw-r--r--   0        0        0      989 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_get_connection_meta_envelope.py
--rw-r--r--   0        0        0     1005 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_get_execution_response_envelope.py
--rw-r--r--   0        0        0     1246 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_get_execution_response_schema.py
--rw-r--r--   0        0        0     1001 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_get_identity_response_envelope.py
--rw-r--r--   0        0        0     1201 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_get_identity_response_schema.py
--rw-r--r--   0        0        0     1025 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_identity.py
--rw-r--r--   0        0        0      922 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_identity_function.py
--rw-r--r--   0        0        0     1019 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_list_execution_response_envelope.py
--rw-r--r--   0        0        0      980 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_list_policies_response_envelope.py
--rw-r--r--   0        0        0      970 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_list_sync_response_envelope.py
--rw-r--r--   0        0        0      938 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_list_users_envelope.py
--rw-r--r--   0        0        0     1098 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_mode.py
--rw-r--r--   0        0        0     1138 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_model_field.py
--rw-r--r--   0        0        0      939 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_model_field_request.py
--rw-r--r--   0        0        0      958 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_model_field_response.py
--rw-r--r--   0        0        0      974 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_model_list_response_envelope.py
--rw-r--r--   0        0        0     1550 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_model_response.py
--rw-r--r--   0        0        0      957 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_model_response_envelope.py
--rw-r--r--   0        0        0     1024 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_organization.py
--rw-r--r--   0        0        0      952 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_organization_envelope.py
--rw-r--r--   0        0        0      966 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_organizations_envelope.py
--rw-r--r--   0        0        0     1004 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_override.py
--rw-r--r--   0        0        0      921 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_policy_action.py
--rw-r--r--   0        0        0     1106 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_policy_response.py
--rw-r--r--   0        0        0      961 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_policy_response_envelope.py
--rw-r--r--   0        0        0     1042 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_relation.py
--rw-r--r--   0        0        0      922 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_relation_to.py
--rw-r--r--   0        0        0      970 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_role_list_response_envelope.py
--rw-r--r--   0        0        0      993 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_role_response.py
--rw-r--r--   0        0        0      953 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_role_response_envelope.py
--rw-r--r--   0        0        0      954 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_run_after.py
--rw-r--r--   0        0        0     1143 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_schedule.py
--rw-r--r--   0        0        0      884 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_source.py
--rw-r--r--   0        0        0      993 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_start_sync_response_envelope.py
--rw-r--r--   0        0        0      975 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_start_sync_response_schema.py
--rw-r--r--   0        0        0     1138 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_supported_mode.py
--rw-r--r--   0        0        0     1032 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_sync_field.py
--rw-r--r--   0        0        0     1719 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_sync_response.py
--rw-r--r--   0        0        0      953 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_sync_response_envelope.py
--rw-r--r--   0        0        0      970 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_sync_status_envelope.py
--rw-r--r--   0        0        0     1128 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_sync_status_response.py
--rw-r--r--   0        0        0     1094 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_target.py
--rw-r--r--   0        0        0     1384 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_target_field.py
--rw-r--r--   0        0        0     1269 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_target_response.py
--rw-r--r--   0        0        0      961 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_target_response_envelope.py
--rw-r--r--   0        0        0      983 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_user.py
--rw-r--r--   0        0        0      920 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_user_envelope.py
--rw-r--r--   0        0        0     1036 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_webhook.py
--rw-r--r--   0        0        0      932 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_webhook_envelope.py
--rw-r--r--   0        0        0      949 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_2_webhook_list_envelope.py
--rw-r--r--   0        0        0      956 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_field.py
--rw-r--r--   0        0        0     1053 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_schema.py
--rw-r--r--   0        0        0      945 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_schema_envelope.py
--rw-r--r--   0        0        0     1303 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_execution.py
--rw-r--r--   0        0        0      974 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_execution_envelope.py
--rw-r--r--   0        0        0     1224 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_schema_execution.py
--rw-r--r--   0        0        0      991 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source.py
--rw-r--r--   0        0        0      962 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_envelope.py
--rw-r--r--   0        0        0      942 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_schema_envelope.py
--rw-r--r--   0        0        0     1015 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_status.py
--rw-r--r--   0        0        0      987 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_status_envelope.py
--rw-r--r--   0        0        0      987 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_status_envelope.py
--rw-r--r--   0        0        0     1095 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_status_response.py
--rw-r--r--   0        0        0      935 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_connect_card_response.py
--rw-r--r--   0        0        0      982 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_connect_card_response_envelope.py
--rw-r--r--   0        0        0      962 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_list_bulk_schema_envelope.py
--rw-r--r--   0        0        0      992 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_list_bulk_sync_executions_envelope.py
--rw-r--r--   0        0        0      918 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_pick_value.py
--rw-r--r--   0        0        0     1011 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_schema.py
--rw-r--r--   0        0        0     1181 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_schema_field.py
--rw-r--r--   0        0        0      943 2024-02-14 03:19:27.705363 polytomic-0.1.0/src/polytomic/types/v_3_schema_records_response_envelope.py
--rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 polytomic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-04 02:07:02.834260 polytomic-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1868 2024-04-04 02:07:02.834260 polytomic-0.1.2/README.md
+-rw-r--r--   0        0        0      596 2024-04-04 02:07:02.834260 polytomic-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6967 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/__init__.py
+-rw-r--r--   0        0        0     7571 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/client.py
+-rw-r--r--   0        0        0      790 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/api_error.py
+-rw-r--r--   0        0        0     2558 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/core/request_options.py
+-rw-r--r--   0        0        0      152 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/environment.py
+-rw-r--r--   0        0        0      148 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/errors/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/py.typed
+-rw-r--r--   0        0        0      430 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/__init__.py
+-rw-r--r--   0        0        0    70925 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/client.py
+-rw-r--r--   0        0        0      136 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/executions/__init__.py
+-rw-r--r--   0        0        0    17013 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/executions/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/schemas/__init__.py
+-rw-r--r--   0        0        0    18162 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/schemas/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/connections/__init__.py
+-rw-r--r--   0        0        0    65762 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/connections/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/events/__init__.py
+-rw-r--r--   0        0        0    12416 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/events/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     5572 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/jobs/client.py
+-rw-r--r--   0        0        0      125 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/__init__.py
+-rw-r--r--   0        0        0    58565 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/client.py
+-rw-r--r--   0        0        0      116 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/resources/executions/__init__.py
+-rw-r--r--   0        0        0    59453 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/model_sync/resources/executions/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/models/__init__.py
+-rw-r--r--   0        0        0    34659 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/models/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/organization/__init__.py
+-rw-r--r--   0        0        0    30862 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/organization/client.py
+-rw-r--r--   0        0        0      137 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/client.py
+-rw-r--r--   0        0        0      128 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/policies/__init__.py
+-rw-r--r--   0        0        0    27695 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/policies/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/roles/__init__.py
+-rw-r--r--   0        0        0    25551 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/permissions/resources/roles/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/schemas/__init__.py
+-rw-r--r--   0        0        0     5861 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/schemas/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/users/__init__.py
+-rw-r--r--   0        0        0    35157 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/users/client.py
+-rw-r--r--   0        0        0       65 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0    28121 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/resources/webhooks/client.py
+-rw-r--r--   0        0        0    10037 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/__init__.py
+-rw-r--r--   0        0        0      998 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/activate_sync_envelope.py
+-rw-r--r--   0        0        0      906 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/activate_sync_input.py
+-rw-r--r--   0        0        0      967 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/activate_sync_output.py
+-rw-r--r--   0        0        0      925 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/api_key_response.py
+-rw-r--r--   0        0        0      988 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/api_key_response_envelope.py
+-rw-r--r--   0        0        0      851 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_discover.py
+-rw-r--r--   0        0        0     1756 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_execution_status.py
+-rw-r--r--   0        0        0     1004 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_field.py
+-rw-r--r--   0        0        0     1134 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_itemized_schedule.py
+-rw-r--r--   0        0        0     1152 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_multi_schedule_configuration.py
+-rw-r--r--   0        0        0     1407 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schedule.py
+-rw-r--r--   0        0        0     1145 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schema.py
+-rw-r--r--   0        0        0      971 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schema_envelope.py
+-rw-r--r--   0        0        0     1337 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_schema_execution_status.py
+-rw-r--r--   0        0        0      763 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_selective_mode.py
+-rw-r--r--   0        0        0     1060 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_dest.py
+-rw-r--r--   0        0        0      980 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_dest_envelope.py
+-rw-r--r--   0        0        0     1456 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_execution.py
+-rw-r--r--   0        0        0     1000 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_execution_envelope.py
+-rw-r--r--   0        0        0     1005 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_list_envelope.py
+-rw-r--r--   0        0        0     1555 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_response.py
+-rw-r--r--   0        0        0      996 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_response_envelope.py
+-rw-r--r--   0        0        0     1429 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_schema_execution.py
+-rw-r--r--   0        0        0     1024 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source.py
+-rw-r--r--   0        0        0      988 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_envelope.py
+-rw-r--r--   0        0        0      968 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_schema_envelope.py
+-rw-r--r--   0        0        0     1063 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status.py
+-rw-r--r--   0        0        0     1013 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status_envelope.py
+-rw-r--r--   0        0        0     1013 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_status_envelope.py
+-rw-r--r--   0        0        0     1133 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/bulk_sync_status_response.py
+-rw-r--r--   0        0        0      987 2024-04-04 02:07:02.834260 polytomic-0.1.2/src/polytomic/types/configuration_value.py
+-rw-r--r--   0        0        0      976 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connect_card_response.py
+-rw-r--r--   0        0        0     1008 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connect_card_response_envelope.py
+-rw-r--r--   0        0        0     1039 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_list_response_envelope.py
+-rw-r--r--   0        0        0     1051 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_meta.py
+-rw-r--r--   0        0        0     1217 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_meta_response.py
+-rw-r--r--   0        0        0      981 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_parameter_value.py
+-rw-r--r--   0        0        0     1090 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_parameter_values_resp.py
+-rw-r--r--   0        0        0     1088 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_parameter_values_response_envelope.py
+-rw-r--r--   0        0        0     1022 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_response_envelope.py
+-rw-r--r--   0        0        0     1344 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_response_schema.py
+-rw-r--r--   0        0        0     1194 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_type.py
+-rw-r--r--   0        0        0     1008 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_type_response_envelope.py
+-rw-r--r--   0        0        0     1023 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/connection_type_schema.py
+-rw-r--r--   0        0        0     1047 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/create_connection_response_envelope.py
+-rw-r--r--   0        0        0     1639 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/create_connection_response_schema.py
+-rw-r--r--   0        0        0     1098 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/event.py
+-rw-r--r--   0        0        0      941 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/event_types_envelope.py
+-rw-r--r--   0        0        0      964 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/events_envelope.py
+-rw-r--r--   0        0        0     1045 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_counts.py
+-rw-r--r--   0        0        0      992 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_log_response.py
+-rw-r--r--   0        0        0     1013 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_logs_response_envelope.py
+-rw-r--r--   0        0        0     1867 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/execution_status.py
+-rw-r--r--   0        0        0     1019 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/filter.py
+-rw-r--r--   0        0        0     1015 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_connection_meta_envelope.py
+-rw-r--r--   0        0        0     1031 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_execution_response_envelope.py
+-rw-r--r--   0        0        0     1379 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_execution_response_schema.py
+-rw-r--r--   0        0        0     1027 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_identity_response_envelope.py
+-rw-r--r--   0        0        0     1291 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/get_identity_response_schema.py
+-rw-r--r--   0        0        0     1058 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/identity.py
+-rw-r--r--   0        0        0      963 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/identity_function.py
+-rw-r--r--   0        0        0     1143 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/job_response.py
+-rw-r--r--   0        0        0      975 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/job_response_envelope.py
+-rw-r--r--   0        0        0      118 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/jsonschema_form.py
+-rw-r--r--   0        0        0      114 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/label_label.py
+-rw-r--r--   0        0        0      980 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_bulk_schema.py
+-rw-r--r--   0        0        0     1018 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_bulk_sync_executions_envelope.py
+-rw-r--r--   0        0        0     1045 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_execution_response_envelope.py
+-rw-r--r--   0        0        0     1017 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1006 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_policies_response_envelope.py
+-rw-r--r--   0        0        0      964 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/list_users_envelope.py
+-rw-r--r--   0        0        0     1167 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/mode.py
+-rw-r--r--   0        0        0     1221 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_field.py
+-rw-r--r--   0        0        0      984 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_field_response.py
+-rw-r--r--   0        0        0     1000 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_list_response_envelope.py
+-rw-r--r--   0        0        0      978 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_model_field_request.py
+-rw-r--r--   0        0        0     1135 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_relation.py
+-rw-r--r--   0        0        0      968 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_relation_to.py
+-rw-r--r--   0        0        0     1652 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_response.py
+-rw-r--r--   0        0        0     1066 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_response_envelope.py
+-rw-r--r--   0        0        0     1077 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_sync_field.py
+-rw-r--r--   0        0        0     1827 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_sync_response.py
+-rw-r--r--   0        0        0     1000 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1086 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/organization.py
+-rw-r--r--   0        0        0      978 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/organization_envelope.py
+-rw-r--r--   0        0        0      992 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/organizations_envelope.py
+-rw-r--r--   0        0        0     1059 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/override.py
+-rw-r--r--   0        0        0      959 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/pick_value.py
+-rw-r--r--   0        0        0      955 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/policy_action.py
+-rw-r--r--   0        0        0     1160 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/policy_response.py
+-rw-r--r--   0        0        0      987 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/policy_response_envelope.py
+-rw-r--r--   0        0        0     1114 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/relation.py
+-rw-r--r--   0        0        0      963 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/relation_to.py
+-rw-r--r--   0        0        0     1331 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/rest_err_response.py
+-rw-r--r--   0        0        0      996 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/role_list_response_envelope.py
+-rw-r--r--   0        0        0     1048 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/role_response.py
+-rw-r--r--   0        0        0      979 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/role_response_envelope.py
+-rw-r--r--   0        0        0      995 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/run_after.py
+-rw-r--r--   0        0        0     1298 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule.py
+-rw-r--r--   0        0        0     1669 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_frequency.py
+-rw-r--r--   0        0        0     1037 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_option_response.py
+-rw-r--r--   0        0        0     1020 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_option_response_envelope.py
+-rw-r--r--   0        0        0     1187 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schedule_schedule_option.py
+-rw-r--r--   0        0        0     1051 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema.py
+-rw-r--r--   0        0        0     1072 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema_association.py
+-rw-r--r--   0        0        0     1242 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema_field.py
+-rw-r--r--   0        0        0      977 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/schema_records_response_envelope.py
+-rw-r--r--   0        0        0      911 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/source.py
+-rw-r--r--   0        0        0     1040 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/start_model_sync_response_envelope.py
+-rw-r--r--   0        0        0     1086 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/start_model_sync_response_schema.py
+-rw-r--r--   0        0        0     1220 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/supported_mode.py
+-rw-r--r--   0        0        0     1476 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/sync_destination_properties.py
+-rw-r--r--   0        0        0      996 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/sync_status_envelope.py
+-rw-r--r--   0        0        0     1166 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/sync_status_response.py
+-rw-r--r--   0        0        0     1149 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target.py
+-rw-r--r--   0        0        0     1487 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target_field.py
+-rw-r--r--   0        0        0     1322 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target_response.py
+-rw-r--r--   0        0        0      987 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/target_response_envelope.py
+-rw-r--r--   0        0        0     1038 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/user.py
+-rw-r--r--   0        0        0      946 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/user_envelope.py
+-rw-r--r--   0        0        0     1098 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/webhook.py
+-rw-r--r--   0        0        0      958 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/webhook_envelope.py
+-rw-r--r--   0        0        0      975 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/webhook_list_envelope.py
+-rw-r--r--   0        0        0      623 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/types/work_task_status.py
+-rw-r--r--   0        0        0       77 2024-04-04 02:07:02.838260 polytomic-0.1.2/src/polytomic/version.py
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 polytomic-0.1.2/PKG-INFO
```

### Comparing `polytomic-0.1.0/LICENSE` & `polytomic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.0/README.md` & `polytomic-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
 ```python
 from polytomic.client import Polytomic
 
 client = Polytomic(
-    polytomic_version="YOUR_POLYTOMIC_VERSION",
+    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 ```python
 from polytomic.client import AsyncPolytomic
 
 client = AsyncPolytomic(
-    polytomic_version="YOUR_POLYTOMIC_VERSION",
+    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Async Usage  -->
 
 <!-- Begin Status, generated by Fern  -->
 # Beta Status
```

### Comparing `polytomic-0.1.0/src/polytomic/core/datetime_utils.py` & `polytomic-0.1.2/src/polytomic/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `polytomic-0.1.0/src/polytomic/core/jsonable_encoder.py` & `polytomic-0.1.2/src/polytomic/core/jsonable_encoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -61,18 +61,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
```

### Comparing `polytomic-0.1.0/src/polytomic/resources/bulk_sync/client.py` & `polytomic-0.1.2/src/polytomic/resources/models/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,382 +1,285 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
 from ...errors.unauthorized_error import UnauthorizedError
-from ...types.bulk_schedule import BulkSchedule
+from ...types.model_list_response_envelope import ModelListResponseEnvelope
+from ...types.model_model_field_request import ModelModelFieldRequest
+from ...types.model_relation import ModelRelation
+from ...types.model_response_envelope import ModelResponseEnvelope
 from ...types.rest_err_response import RestErrResponse
-from ...types.v_2_activate_sync_envelope import V2ActivateSyncEnvelope
-from ...types.v_2_activate_sync_input import V2ActivateSyncInput
-from ...types.v_2_bulk_sync_dest_envelope import V2BulkSyncDestEnvelope
-from ...types.v_2_bulk_sync_list_envelope import V2BulkSyncListEnvelope
-from ...types.v_2_bulk_sync_response_envelope import V2BulkSyncResponseEnvelope
-from ...types.v_3_bulk_sync_source_envelope import V3BulkSyncSourceEnvelope
-from ...types.v_3_bulk_sync_source_schema_envelope import V3BulkSyncSourceSchemaEnvelope
-from ...types.v_3_bulk_sync_source_status_envelope import V3BulkSyncSourceStatusEnvelope
-from ...types.v_3_bulk_sync_status_envelope import V3BulkSyncStatusEnvelope
-from .resources.executions.client import AsyncExecutionsClient, ExecutionsClient
-from .resources.schemas.client import AsyncSchemasClient, SchemasClient
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class BulkSyncClient:
+class ModelsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
-        self.executions = ExecutionsClient(client_wrapper=self._client_wrapper)
-        self.schemas = SchemasClient(client_wrapper=self._client_wrapper)
 
-    def get_destination(self, id: str) -> V2BulkSyncDestEnvelope:
+    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ModelListResponseEnvelope:
         """
         Parameters:
-            - id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.get_destination(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+        client.models.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/dest/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncDestEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_source(
-        self,
-        connection_id: str,
-        *,
-        refresh_schemas: typing.Optional[bool] = None,
-        include_fields: typing.Optional[bool] = None,
-    ) -> V3BulkSyncSourceEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-
-            - refresh_schemas: typing.Optional[bool].
-
-            - include_fields: typing.Optional[bool].
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.get_source(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{connection_id}"),
-            params=remove_none_from_dict({"refresh_schemas": refresh_schemas, "include_fields": include_fields}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncSourceEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_source_schema(self, connection_id: str, schema_id: str) -> V3BulkSyncSourceSchemaEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-
-            - schema_id: str.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.get_source_schema(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="schema_id",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{connection_id}/schema/{schema_id}"
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/models"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncSourceSchemaEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def api_v_3_get_bulk_source_status(self, connection_id: str) -> V3BulkSyncSourceStatusEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.api_v_3_get_bulk_source_status(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{connection_id}/status"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncSourceStatusEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def list(self) -> V2BulkSyncListEnvelope:
-        """
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.list()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/bulk/syncs"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncListEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelListResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
-        active: typing.Optional[bool] = OMIT,
-        automatically_add_new_fields: typing.Optional[bool] = OMIT,
-        automatically_add_new_objects: typing.Optional[bool] = OMIT,
-        destination_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        destination_connection_id: str,
-        disable_record_timestamps: typing.Optional[bool] = OMIT,
-        discover: typing.Optional[bool] = OMIT,
-        mode: str,
+        async_: typing.Optional[bool] = None,
+        additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
+        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        connection_id: str,
+        fields: typing.Optional[typing.Sequence[str]] = OMIT,
+        identifier: typing.Optional[str] = OMIT,
+        labels: typing.Optional[typing.Sequence[str]] = OMIT,
         name: str,
         organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        schedule: BulkSchedule,
-        schemas: typing.Optional[typing.List[str]] = OMIT,
-        source_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        source_connection_id: str,
-    ) -> V2BulkSyncResponseEnvelope:
+        policies: typing.Optional[typing.Sequence[str]] = OMIT,
+        relations: typing.Optional[typing.Sequence[ModelRelation]] = OMIT,
+        tracking_columns: typing.Optional[typing.Sequence[str]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ModelResponseEnvelope:
         """
         Parameters:
-            - active: typing.Optional[bool].
+            - async_: typing.Optional[bool].
 
-            - automatically_add_new_fields: typing.Optional[bool].
+            - additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]].
 
-            - automatically_add_new_objects: typing.Optional[bool].
+            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
 
-            - destination_configuration: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - destination_connection_id: str.
+            - connection_id: str.
 
-            - disable_record_timestamps: typing.Optional[bool].
+            - fields: typing.Optional[typing.Sequence[str]].
 
-            - discover: typing.Optional[bool]. DEPRECATED: Use automatically_add_new_objects/automatically_add_new_fields instead
+            - identifier: typing.Optional[str].
 
-            - mode: str.
+            - labels: typing.Optional[typing.Sequence[str]].
 
             - name: str.
 
             - organization_id: typing.Optional[str].
 
-            - policies: typing.Optional[typing.List[str]].
-
-            - schedule: BulkSchedule.
+            - policies: typing.Optional[typing.Sequence[str]].
 
-            - schemas: typing.Optional[typing.List[str]].
+            - relations: typing.Optional[typing.Sequence[ModelRelation]].
 
-            - source_configuration: typing.Optional[typing.Dict[str, typing.Any]].
+            - tracking_columns: typing.Optional[typing.Sequence[str]].
 
-            - source_connection_id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import BulkSchedule
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.create(
-            destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="mode",
-            name="name",
-            schedule=BulkSchedule(
-                frequency="frequency",
-            ),
-            source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.models.create(
+            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            identifier="id",
+            name="Users",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "destination_connection_id": destination_connection_id,
-            "mode": mode,
-            "name": name,
-            "schedule": schedule,
-            "source_connection_id": source_connection_id,
-        }
-        if active is not OMIT:
-            _request["active"] = active
-        if automatically_add_new_fields is not OMIT:
-            _request["automatically_add_new_fields"] = automatically_add_new_fields
-        if automatically_add_new_objects is not OMIT:
-            _request["automatically_add_new_objects"] = automatically_add_new_objects
-        if destination_configuration is not OMIT:
-            _request["destination_configuration"] = destination_configuration
-        if disable_record_timestamps is not OMIT:
-            _request["disable_record_timestamps"] = disable_record_timestamps
-        if discover is not OMIT:
-            _request["discover"] = discover
+        _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
+        if additional_fields is not OMIT:
+            _request["additional_fields"] = additional_fields
+        if configuration is not OMIT:
+            _request["configuration"] = configuration
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if identifier is not OMIT:
+            _request["identifier"] = identifier
+        if labels is not OMIT:
+            _request["labels"] = labels
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policies is not OMIT:
             _request["policies"] = policies
-        if schemas is not OMIT:
-            _request["schemas"] = schemas
-        if source_configuration is not OMIT:
-            _request["source_configuration"] = source_configuration
+        if relations is not OMIT:
+            _request["relations"] = relations
+        if tracking_columns is not OMIT:
+            _request["tracking_columns"] = tracking_columns
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/bulk/syncs"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/models"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "async": async_,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str, *, refresh_schemas: typing.Optional[bool] = None) -> V2BulkSyncResponseEnvelope:
+    def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ModelResponseEnvelope:
         """
         Parameters:
             - id: str.
 
-            - refresh_schemas: typing.Optional[bool].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.get(
+        client.models.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}"),
-            params=remove_none_from_dict({"refresh_schemas": refresh_schemas}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def remove(self, id: str, *, refresh_schemas: typing.Optional[bool] = None) -> None:
+    def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Parameters:
             - id: str.
 
-            - refresh_schemas: typing.Optional[bool].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.remove(
+        client.models.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}"),
-            params=remove_none_from_dict({"refresh_schemas": refresh_schemas}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
@@ -384,521 +287,388 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
         *,
-        active: typing.Optional[bool] = OMIT,
-        destination_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        destination_connection_id: str,
-        discover: typing.Optional[bool] = OMIT,
-        mode: str,
+        async_: typing.Optional[bool] = None,
+        additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
+        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        connection_id: str,
+        fields: typing.Optional[typing.Sequence[str]] = OMIT,
+        identifier: typing.Optional[str] = OMIT,
+        labels: typing.Optional[typing.Sequence[str]] = OMIT,
         name: str,
         organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        schedule: BulkSchedule,
-        source_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        source_connection_id: str,
-    ) -> V2BulkSyncResponseEnvelope:
+        policies: typing.Optional[typing.Sequence[str]] = OMIT,
+        relations: typing.Optional[typing.Sequence[ModelRelation]] = OMIT,
+        tracking_columns: typing.Optional[typing.Sequence[str]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ModelResponseEnvelope:
         """
-        > 📘 Updating schemas
-        >
-        > Schema updates can be performed using the [Update Bulk Sync Schemas](https://docs.polytomic.com/reference/apiv3updatebulksyncschemas) endpoint.
-
         Parameters:
             - id: str.
 
-            - active: typing.Optional[bool].
+            - async_: typing.Optional[bool].
+
+            - additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]].
 
-            - destination_configuration: typing.Optional[typing.Dict[str, typing.Any]].
+            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
+
+            - connection_id: str.
 
-            - destination_connection_id: str.
+            - fields: typing.Optional[typing.Sequence[str]].
 
-            - discover: typing.Optional[bool].
+            - identifier: typing.Optional[str].
 
-            - mode: str.
+            - labels: typing.Optional[typing.Sequence[str]].
 
             - name: str.
 
             - organization_id: typing.Optional[str].
 
-            - policies: typing.Optional[typing.List[str]].
+            - policies: typing.Optional[typing.Sequence[str]].
 
-            - schedule: BulkSchedule.
+            - relations: typing.Optional[typing.Sequence[ModelRelation]].
 
-            - source_configuration: typing.Optional[typing.Dict[str, typing.Any]].
+            - tracking_columns: typing.Optional[typing.Sequence[str]].
 
-            - source_connection_id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import BulkSchedule
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.bulk_sync.update(
+        client.models.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="mode",
-            name="name",
-            schedule=BulkSchedule(
-                frequency="frequency",
-            ),
-            source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            async_=False,
+            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            identifier="id",
+            name="Users",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "destination_connection_id": destination_connection_id,
-            "mode": mode,
-            "name": name,
-            "schedule": schedule,
-            "source_connection_id": source_connection_id,
-        }
-        if active is not OMIT:
-            _request["active"] = active
-        if destination_configuration is not OMIT:
-            _request["destination_configuration"] = destination_configuration
-        if discover is not OMIT:
-            _request["discover"] = discover
+        _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
+        if additional_fields is not OMIT:
+            _request["additional_fields"] = additional_fields
+        if configuration is not OMIT:
+            _request["configuration"] = configuration
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if identifier is not OMIT:
+            _request["identifier"] = identifier
+        if labels is not OMIT:
+            _request["labels"] = labels
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policies is not OMIT:
             _request["policies"] = policies
-        if source_configuration is not OMIT:
-            _request["source_configuration"] = source_configuration
+        if relations is not OMIT:
+            _request["relations"] = relations
+        if tracking_columns is not OMIT:
+            _request["tracking_columns"] = tracking_columns
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def activate(self, id: str, *, request: V2ActivateSyncInput) -> V2ActivateSyncEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - request: V2ActivateSyncInput.
-        ---
-        from polytomic import V2ActivateSyncInput
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.activate(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            request=V2ActivateSyncInput(
-                active=True,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "async": async_,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}/activate"),
-            json=jsonable_encoder(request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ActivateSyncEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_status(self, id: str) -> V3BulkSyncStatusEnvelope:
-        """
-        Parameters:
-            - id: str.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.bulk_sync.get_status(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}/status"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncStatusEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncBulkSyncClient:
+class AsyncModelsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
-        self.executions = AsyncExecutionsClient(client_wrapper=self._client_wrapper)
-        self.schemas = AsyncSchemasClient(client_wrapper=self._client_wrapper)
 
-    async def get_destination(self, id: str) -> V2BulkSyncDestEnvelope:
+    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ModelListResponseEnvelope:
         """
         Parameters:
-            - id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.get_destination(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+        await client.models.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/dest/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncDestEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_source(
-        self,
-        connection_id: str,
-        *,
-        refresh_schemas: typing.Optional[bool] = None,
-        include_fields: typing.Optional[bool] = None,
-    ) -> V3BulkSyncSourceEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-
-            - refresh_schemas: typing.Optional[bool].
-
-            - include_fields: typing.Optional[bool].
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.get_source(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{connection_id}"),
-            params=remove_none_from_dict({"refresh_schemas": refresh_schemas, "include_fields": include_fields}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncSourceEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_source_schema(self, connection_id: str, schema_id: str) -> V3BulkSyncSourceSchemaEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-
-            - schema_id: str.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.get_source_schema(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            schema_id="schema_id",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{connection_id}/schema/{schema_id}"
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/models"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncSourceSchemaEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def api_v_3_get_bulk_source_status(self, connection_id: str) -> V3BulkSyncSourceStatusEnvelope:
-        """
-        Parameters:
-            - connection_id: str.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.api_v_3_get_bulk_source_status(
-            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/source/{connection_id}/status"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncSourceStatusEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def list(self) -> V2BulkSyncListEnvelope:
-        """
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.list()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/bulk/syncs"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncListEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelListResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
-        active: typing.Optional[bool] = OMIT,
-        automatically_add_new_fields: typing.Optional[bool] = OMIT,
-        automatically_add_new_objects: typing.Optional[bool] = OMIT,
-        destination_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        destination_connection_id: str,
-        disable_record_timestamps: typing.Optional[bool] = OMIT,
-        discover: typing.Optional[bool] = OMIT,
-        mode: str,
+        async_: typing.Optional[bool] = None,
+        additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
+        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        connection_id: str,
+        fields: typing.Optional[typing.Sequence[str]] = OMIT,
+        identifier: typing.Optional[str] = OMIT,
+        labels: typing.Optional[typing.Sequence[str]] = OMIT,
         name: str,
         organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        schedule: BulkSchedule,
-        schemas: typing.Optional[typing.List[str]] = OMIT,
-        source_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        source_connection_id: str,
-    ) -> V2BulkSyncResponseEnvelope:
+        policies: typing.Optional[typing.Sequence[str]] = OMIT,
+        relations: typing.Optional[typing.Sequence[ModelRelation]] = OMIT,
+        tracking_columns: typing.Optional[typing.Sequence[str]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ModelResponseEnvelope:
         """
         Parameters:
-            - active: typing.Optional[bool].
+            - async_: typing.Optional[bool].
 
-            - automatically_add_new_fields: typing.Optional[bool].
+            - additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]].
 
-            - automatically_add_new_objects: typing.Optional[bool].
+            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
 
-            - destination_configuration: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - destination_connection_id: str.
+            - connection_id: str.
 
-            - disable_record_timestamps: typing.Optional[bool].
+            - fields: typing.Optional[typing.Sequence[str]].
 
-            - discover: typing.Optional[bool]. DEPRECATED: Use automatically_add_new_objects/automatically_add_new_fields instead
+            - identifier: typing.Optional[str].
 
-            - mode: str.
+            - labels: typing.Optional[typing.Sequence[str]].
 
             - name: str.
 
             - organization_id: typing.Optional[str].
 
-            - policies: typing.Optional[typing.List[str]].
-
-            - schedule: BulkSchedule.
+            - policies: typing.Optional[typing.Sequence[str]].
 
-            - schemas: typing.Optional[typing.List[str]].
+            - relations: typing.Optional[typing.Sequence[ModelRelation]].
 
-            - source_configuration: typing.Optional[typing.Dict[str, typing.Any]].
+            - tracking_columns: typing.Optional[typing.Sequence[str]].
 
-            - source_connection_id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import BulkSchedule
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.create(
-            destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="mode",
-            name="name",
-            schedule=BulkSchedule(
-                frequency="frequency",
-            ),
-            source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.models.create(
+            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            identifier="id",
+            name="Users",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "destination_connection_id": destination_connection_id,
-            "mode": mode,
-            "name": name,
-            "schedule": schedule,
-            "source_connection_id": source_connection_id,
-        }
-        if active is not OMIT:
-            _request["active"] = active
-        if automatically_add_new_fields is not OMIT:
-            _request["automatically_add_new_fields"] = automatically_add_new_fields
-        if automatically_add_new_objects is not OMIT:
-            _request["automatically_add_new_objects"] = automatically_add_new_objects
-        if destination_configuration is not OMIT:
-            _request["destination_configuration"] = destination_configuration
-        if disable_record_timestamps is not OMIT:
-            _request["disable_record_timestamps"] = disable_record_timestamps
-        if discover is not OMIT:
-            _request["discover"] = discover
+        _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
+        if additional_fields is not OMIT:
+            _request["additional_fields"] = additional_fields
+        if configuration is not OMIT:
+            _request["configuration"] = configuration
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if identifier is not OMIT:
+            _request["identifier"] = identifier
+        if labels is not OMIT:
+            _request["labels"] = labels
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policies is not OMIT:
             _request["policies"] = policies
-        if schemas is not OMIT:
-            _request["schemas"] = schemas
-        if source_configuration is not OMIT:
-            _request["source_configuration"] = source_configuration
+        if relations is not OMIT:
+            _request["relations"] = relations
+        if tracking_columns is not OMIT:
+            _request["tracking_columns"] = tracking_columns
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/bulk/syncs"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/models"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "async": async_,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, id: str, *, refresh_schemas: typing.Optional[bool] = None) -> V2BulkSyncResponseEnvelope:
+    async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ModelResponseEnvelope:
         """
         Parameters:
             - id: str.
 
-            - refresh_schemas: typing.Optional[bool].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.get(
+        await client.models.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}"),
-            params=remove_none_from_dict({"refresh_schemas": refresh_schemas}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def remove(self, id: str, *, refresh_schemas: typing.Optional[bool] = None) -> None:
+    async def remove(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         Parameters:
             - id: str.
 
-            - refresh_schemas: typing.Optional[bool].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.remove(
+        await client.models.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}"),
-            params=remove_none_from_dict({"refresh_schemas": refresh_schemas}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
@@ -906,171 +676,128 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
         *,
-        active: typing.Optional[bool] = OMIT,
-        destination_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        destination_connection_id: str,
-        discover: typing.Optional[bool] = OMIT,
-        mode: str,
+        async_: typing.Optional[bool] = None,
+        additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]] = OMIT,
+        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        connection_id: str,
+        fields: typing.Optional[typing.Sequence[str]] = OMIT,
+        identifier: typing.Optional[str] = OMIT,
+        labels: typing.Optional[typing.Sequence[str]] = OMIT,
         name: str,
         organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        schedule: BulkSchedule,
-        source_configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        source_connection_id: str,
-    ) -> V2BulkSyncResponseEnvelope:
+        policies: typing.Optional[typing.Sequence[str]] = OMIT,
+        relations: typing.Optional[typing.Sequence[ModelRelation]] = OMIT,
+        tracking_columns: typing.Optional[typing.Sequence[str]] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ModelResponseEnvelope:
         """
-        > 📘 Updating schemas
-        >
-        > Schema updates can be performed using the [Update Bulk Sync Schemas](https://docs.polytomic.com/reference/apiv3updatebulksyncschemas) endpoint.
-
         Parameters:
             - id: str.
 
-            - active: typing.Optional[bool].
+            - async_: typing.Optional[bool].
+
+            - additional_fields: typing.Optional[typing.Sequence[ModelModelFieldRequest]].
 
-            - destination_configuration: typing.Optional[typing.Dict[str, typing.Any]].
+            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
+
+            - connection_id: str.
 
-            - destination_connection_id: str.
+            - fields: typing.Optional[typing.Sequence[str]].
 
-            - discover: typing.Optional[bool].
+            - identifier: typing.Optional[str].
 
-            - mode: str.
+            - labels: typing.Optional[typing.Sequence[str]].
 
             - name: str.
 
             - organization_id: typing.Optional[str].
 
-            - policies: typing.Optional[typing.List[str]].
+            - policies: typing.Optional[typing.Sequence[str]].
 
-            - schedule: BulkSchedule.
+            - relations: typing.Optional[typing.Sequence[ModelRelation]].
 
-            - source_configuration: typing.Optional[typing.Dict[str, typing.Any]].
+            - tracking_columns: typing.Optional[typing.Sequence[str]].
 
-            - source_connection_id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import BulkSchedule
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.bulk_sync.update(
+        await client.models.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            destination_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            mode="mode",
-            name="name",
-            schedule=BulkSchedule(
-                frequency="frequency",
-            ),
-            source_connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            async_=False,
+            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            identifier="id",
+            name="Users",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "destination_connection_id": destination_connection_id,
-            "mode": mode,
-            "name": name,
-            "schedule": schedule,
-            "source_connection_id": source_connection_id,
-        }
-        if active is not OMIT:
-            _request["active"] = active
-        if destination_configuration is not OMIT:
-            _request["destination_configuration"] = destination_configuration
-        if discover is not OMIT:
-            _request["discover"] = discover
+        _request: typing.Dict[str, typing.Any] = {"connection_id": connection_id, "name": name}
+        if additional_fields is not OMIT:
+            _request["additional_fields"] = additional_fields
+        if configuration is not OMIT:
+            _request["configuration"] = configuration
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if identifier is not OMIT:
+            _request["identifier"] = identifier
+        if labels is not OMIT:
+            _request["labels"] = labels
         if organization_id is not OMIT:
             _request["organization_id"] = organization_id
         if policies is not OMIT:
             _request["policies"] = policies
-        if source_configuration is not OMIT:
-            _request["source_configuration"] = source_configuration
+        if relations is not OMIT:
+            _request["relations"] = relations
+        if tracking_columns is not OMIT:
+            _request["tracking_columns"] = tracking_columns
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2BulkSyncResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def activate(self, id: str, *, request: V2ActivateSyncInput) -> V2ActivateSyncEnvelope:
-        """
-        Parameters:
-            - id: str.
-
-            - request: V2ActivateSyncInput.
-        ---
-        from polytomic import V2ActivateSyncInput
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.activate(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            request=V2ActivateSyncInput(
-                active=True,
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/models/{jsonable_encoder(id)}"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "async": async_,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}/activate"),
-            json=jsonable_encoder(request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ActivateSyncEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_status(self, id: str) -> V3BulkSyncStatusEnvelope:
-        """
-        Parameters:
-            - id: str.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.bulk_sync.get_status(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{id}/status"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3BulkSyncStatusEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ModelResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `polytomic-0.1.0/src/polytomic/resources/connections/client.py` & `polytomic-0.1.2/src/polytomic/resources/users/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1018 +1,840 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
 from ...errors.unauthorized_error import UnauthorizedError
+from ...types.api_key_response_envelope import ApiKeyResponseEnvelope
+from ...types.list_users_envelope import ListUsersEnvelope
 from ...types.rest_err_response import RestErrResponse
-from ...types.v_2_connection_list_response_envelope import V2ConnectionListResponseEnvelope
-from ...types.v_2_connection_response_envelope import V2ConnectionResponseEnvelope
-from ...types.v_2_connection_type_response_envelope import V2ConnectionTypeResponseEnvelope
-from ...types.v_2_create_connection_response_envelope import V2CreateConnectionResponseEnvelope
-from ...types.v_2_get_connection_meta_envelope import V2GetConnectionMetaEnvelope
-from ...types.v_2_model_field_response import V2ModelFieldResponse
-from ...types.v_2_target_response_envelope import V2TargetResponseEnvelope
-from ...types.v_3_connect_card_response_envelope import V3ConnectCardResponseEnvelope
+from ...types.user_envelope import UserEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class ConnectionsClient:
+class UsersClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get_types(self) -> V2ConnectionTypeResponseEnvelope:
+    def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
         """
-        from polytomic.client import Polytomic
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.get_types()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connection_types"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ConnectionTypeResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        Parameters:
+            - org_id: str.
 
-    def list(self) -> V2ConnectionListResponseEnvelope:
-        """
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.list()
+        client.users.list(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ConnectionListResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListUsersEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
+        org_id: str,
         *,
-        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        redirect_url: typing.Optional[str] = OMIT,
-        type: str,
-        validate: typing.Optional[bool] = OMIT,
-    ) -> V2CreateConnectionResponseEnvelope:
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
-        Parameters:
-            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - name: str.
-
-            - organization_id: typing.Optional[str].
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-            - policies: typing.Optional[typing.List[str]].
+        Parameters:
+            - org_id: str.
 
-            - redirect_url: typing.Optional[str]. URL to redirect to after completing OAuth flow.
+            - email: str.
 
-            - type: str.
+            - role: typing.Optional[str].
 
-            - validate: typing.Optional[bool]. Validate connection configuration.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.create(
-            name="name",
-            type="type",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
-        if configuration is not OMIT:
-            _request["configuration"] = configuration
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policies is not OMIT:
-            _request["policies"] = policies
-        if redirect_url is not OMIT:
-            _request["redirect_url"] = redirect_url
-        if validate is not OMIT:
-            _request["validate"] = validate
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client.users.create(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2CreateConnectionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def api_v_3_connect(
-        self,
-        *,
-        connection: typing.Optional[str] = OMIT,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        redirect_url: str,
-        type: typing.Optional[str] = OMIT,
-        whitelist: typing.Optional[typing.List[str]] = OMIT,
-    ) -> V3ConnectCardResponseEnvelope:
         """
-        Parameters:
-            - connection: typing.Optional[str].
-
-            - name: str.
-
-            - organization_id: typing.Optional[str].
-
-            - redirect_url: str.
-
-            - type: typing.Optional[str].
-
-            - whitelist: typing.Optional[typing.List[str]].
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.api_v_3_connect(
-            connection="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
-            redirect_url="redirect_url",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "redirect_url": redirect_url}
-        if connection is not OMIT:
-            _request["connection"] = connection
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if type is not OMIT:
-            _request["type"] = type
-        if whitelist is not OMIT:
-            _request["whitelist"] = whitelist
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3ConnectCardResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, id: str) -> V2ConnectionResponseEnvelope:
+    def get(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
             - id: str.
+
+            - org_id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.get(
+        client.users.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ConnectionResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def remove(self, id: str, *, force: typing.Optional[bool] = None) -> None:
+    def remove(self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> UserEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
             - id: str.
 
-            - force: typing.Optional[bool].
+            - org_id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.remove(
+        client.users.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}"),
-            params=remove_none_from_dict({"force": force}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
         self,
         id: str,
+        org_id: str,
         *,
-        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        reconnect: typing.Optional[bool] = OMIT,
-        type: typing.Optional[str] = OMIT,
-        validate: typing.Optional[bool] = OMIT,
-    ) -> V2CreateConnectionResponseEnvelope:
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
             - id: str.
 
-            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - name: str.
-
-            - organization_id: typing.Optional[str].
+            - org_id: str.
 
-            - policies: typing.Optional[typing.List[str]].
+            - email: str.
 
-            - reconnect: typing.Optional[bool].
+            - role: typing.Optional[str].
 
-            - type: typing.Optional[str].
-
-            - validate: typing.Optional[bool]. Validate connection configuration.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.update(
+        client.users.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if configuration is not OMIT:
-            _request["configuration"] = configuration
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policies is not OMIT:
-            _request["policies"] = policies
-        if reconnect is not OMIT:
-            _request["reconnect"] = reconnect
-        if type is not OMIT:
-            _request["type"] = type
-        if validate is not OMIT:
-            _request["validate"] = validate
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2CreateConnectionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_source(self, id: str) -> V2GetConnectionMetaEnvelope:
-        """
-        Parameters:
-            - id: str.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.get_source(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/source"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2GetConnectionMetaEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_source_fields(
-        self, id: str, *, query: typing.Optional[typing.Dict[str, typing.Any]] = OMIT
-    ) -> V2ModelFieldResponse:
-        """
-        Parameters:
-            - id: str.
-
-            - query: typing.Optional[typing.Dict[str, typing.Any]].
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.get_source_fields(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+    def create_api_key(
+        self,
+        org_id: str,
+        id: str,
+        *,
+        force: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ApiKeyResponseEnvelope:
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if query is not OMIT:
-            _request["query"] = query
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/source/fields"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ModelFieldResponse, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-    def get_target(
-        self, id: str, *, type: typing.Optional[str] = None, search: typing.Optional[str] = None
-    ) -> V2GetConnectionMetaEnvelope:
-        """
         Parameters:
-            - id: str.
-
-            - type: typing.Optional[str].
+            - org_id: str.
 
-            - search: typing.Optional[str].
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.get_target(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/target"),
-            params=remove_none_from_dict({"type": type, "search": search}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2GetConnectionMetaEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_target_fields(
-        self, id: str, *, refresh: typing.Optional[bool] = OMIT, target: str
-    ) -> V2TargetResponseEnvelope:
-        """
-        Parameters:
             - id: str.
 
-            - refresh: typing.Optional[bool].
+            - force: typing.Optional[bool].
 
-            - target: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.connections.get_target_fields(
+        client.users.create_api_key(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            target="database.table",
+            force=True,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"target": target}
-        if refresh is not OMIT:
-            _request["refresh"] = refresh
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/target/fields"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2TargetResponseEnvelope, _response.json())  # type: ignore
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}/keys",
+            ),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "force": force,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ApiKeyResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def connect(self) -> None:
-        """
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.connections.connect()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
 
-class AsyncConnectionsClient:
+class AsyncUsersClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get_types(self) -> V2ConnectionTypeResponseEnvelope:
+    async def list(self, org_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> ListUsersEnvelope:
         """
-        from polytomic.client import AsyncPolytomic
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.get_types()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connection_types"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ConnectionTypeResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        Parameters:
+            - org_id: str.
 
-    async def list(self) -> V2ConnectionListResponseEnvelope:
-        """
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.list()
+        await client.users.list(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ConnectionListResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListUsersEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
+        org_id: str,
         *,
-        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        redirect_url: typing.Optional[str] = OMIT,
-        type: str,
-        validate: typing.Optional[bool] = OMIT,
-    ) -> V2CreateConnectionResponseEnvelope:
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
-        Parameters:
-            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - name: str.
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-            - organization_id: typing.Optional[str].
-
-            - policies: typing.Optional[typing.List[str]].
+        Parameters:
+            - org_id: str.
 
-            - redirect_url: typing.Optional[str]. URL to redirect to after completing OAuth flow.
+            - email: str.
 
-            - type: str.
+            - role: typing.Optional[str].
 
-            - validate: typing.Optional[bool]. Validate connection configuration.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.create(
-            name="name",
-            type="type",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
-        if configuration is not OMIT:
-            _request["configuration"] = configuration
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policies is not OMIT:
-            _request["policies"] = policies
-        if redirect_url is not OMIT:
-            _request["redirect_url"] = redirect_url
-        if validate is not OMIT:
-            _request["validate"] = validate
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        await client.users.create(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2CreateConnectionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def api_v_3_connect(
-        self,
-        *,
-        connection: typing.Optional[str] = OMIT,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        redirect_url: str,
-        type: typing.Optional[str] = OMIT,
-        whitelist: typing.Optional[typing.List[str]] = OMIT,
-    ) -> V3ConnectCardResponseEnvelope:
         """
-        Parameters:
-            - connection: typing.Optional[str].
-
-            - name: str.
-
-            - organization_id: typing.Optional[str].
-
-            - redirect_url: str.
-
-            - type: typing.Optional[str].
-
-            - whitelist: typing.Optional[typing.List[str]].
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.api_v_3_connect(
-            connection="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
-            redirect_url="redirect_url",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name, "redirect_url": redirect_url}
-        if connection is not OMIT:
-            _request["connection"] = connection
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if type is not OMIT:
-            _request["type"] = type
-        if whitelist is not OMIT:
-            _request["whitelist"] = whitelist
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{jsonable_encoder(org_id)}/users"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V3ConnectCardResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, id: str) -> V2ConnectionResponseEnvelope:
+    async def get(
+        self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
             - id: str.
+
+            - org_id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.get(
+        await client.users.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ConnectionResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def remove(self, id: str, *, force: typing.Optional[bool] = None) -> None:
+    async def remove(
+        self, id: str, org_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
             - id: str.
 
-            - force: typing.Optional[bool].
+            - org_id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.remove(
+        await client.users.remove(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}"),
-            params=remove_none_from_dict({"force": force}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
         self,
         id: str,
+        org_id: str,
         *,
-        configuration: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policies: typing.Optional[typing.List[str]] = OMIT,
-        reconnect: typing.Optional[bool] = OMIT,
-        type: typing.Optional[str] = OMIT,
-        validate: typing.Optional[bool] = OMIT,
-    ) -> V2CreateConnectionResponseEnvelope:
+        email: str,
+        role: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserEnvelope:
         """
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+
         Parameters:
             - id: str.
 
-            - configuration: typing.Optional[typing.Dict[str, typing.Any]].
-
-            - name: str.
+            - org_id: str.
 
-            - organization_id: typing.Optional[str].
+            - email: str.
 
-            - policies: typing.Optional[typing.List[str]].
+            - role: typing.Optional[str].
 
-            - reconnect: typing.Optional[bool].
-
-            - type: typing.Optional[str].
-
-            - validate: typing.Optional[bool]. Validate connection configuration.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.update(
+        await client.users.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="name",
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            email="mail@example.com",
+            role="admin",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if configuration is not OMIT:
-            _request["configuration"] = configuration
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policies is not OMIT:
-            _request["policies"] = policies
-        if reconnect is not OMIT:
-            _request["reconnect"] = reconnect
-        if type is not OMIT:
-            _request["type"] = type
-        if validate is not OMIT:
-            _request["validate"] = validate
+        _request: typing.Dict[str, typing.Any] = {"email": email}
+        if role is not OMIT:
+            _request["role"] = role
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2CreateConnectionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_source(self, id: str) -> V2GetConnectionMetaEnvelope:
-        """
-        Parameters:
-            - id: str.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.get_source(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/source"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2GetConnectionMetaEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UserEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_source_fields(
-        self, id: str, *, query: typing.Optional[typing.Dict[str, typing.Any]] = OMIT
-    ) -> V2ModelFieldResponse:
-        """
-        Parameters:
-            - id: str.
-
-            - query: typing.Optional[typing.Dict[str, typing.Any]].
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.get_source_fields(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
+    async def create_api_key(
+        self,
+        org_id: str,
+        id: str,
+        *,
+        force: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ApiKeyResponseEnvelope:
         """
-        _request: typing.Dict[str, typing.Any] = {}
-        if query is not OMIT:
-            _request["query"] = query
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/source/fields"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ModelFieldResponse, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        > 🚧 Requires partner key
+        >
+        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
 
-    async def get_target(
-        self, id: str, *, type: typing.Optional[str] = None, search: typing.Optional[str] = None
-    ) -> V2GetConnectionMetaEnvelope:
-        """
         Parameters:
-            - id: str.
-
-            - type: typing.Optional[str].
-
-            - search: typing.Optional[str].
-        ---
-        from polytomic.client import AsyncPolytomic
+            - org_id: str.
 
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.get_target(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/target"),
-            params=remove_none_from_dict({"type": type, "search": search}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2GetConnectionMetaEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_target_fields(
-        self, id: str, *, refresh: typing.Optional[bool] = OMIT, target: str
-    ) -> V2TargetResponseEnvelope:
-        """
-        Parameters:
             - id: str.
 
-            - refresh: typing.Optional[bool].
+            - force: typing.Optional[bool].
 
-            - target: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.connections.get_target_fields(
+        await client.users.create_api_key(
+            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            target="database.table",
+            force=True,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"target": target}
-        if refresh is not OMIT:
-            _request["refresh"] = refresh
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/connections/{id}/target/fields"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/organizations/{jsonable_encoder(org_id)}/users/{jsonable_encoder(id)}/keys",
+            ),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "force": force,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
+            if request_options is not None
+            else None,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2TargetResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ApiKeyResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def connect(self) -> None:
-        """
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.connections.connect()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/connections/connect"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polytomic-0.1.0/src/polytomic/resources/model_sync/resources/executions/client.py` & `polytomic-0.1.2/src/polytomic/resources/schemas/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,139 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
+import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .....core.api_error import ApiError
-from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from .....errors.unauthorized_error import UnauthorizedError
-from .....types.rest_err_response import RestErrResponse
-from .....types.v_2_get_execution_response_envelope import V2GetExecutionResponseEnvelope
-from .....types.v_2_list_execution_response_envelope import V2ListExecutionResponseEnvelope
+from ...core.api_error import ApiError
+from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ...core.jsonable_encoder import jsonable_encoder
+from ...core.remove_none_from_dict import remove_none_from_dict
+from ...core.request_options import RequestOptions
+from ...errors.unauthorized_error import UnauthorizedError
+from ...types.rest_err_response import RestErrResponse
+from ...types.schema_records_response_envelope import SchemaRecordsResponseEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ExecutionsClient:
+class SchemasClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self, sync_id: str) -> V2ListExecutionResponseEnvelope:
+    def get_records(
+        self, connection_id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> SchemaRecordsResponseEnvelope:
         """
         Parameters:
-            - sync_id: str.
-        ---
-        from polytomic.client import Polytomic
+            - connection_id: str.
 
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.model_sync.executions.list(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{sync_id}/executions"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ListExecutionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get(self, sync_id: str, id: str) -> V2GetExecutionResponseEnvelope:
-        """
-        Parameters:
-            - sync_id: str.
+            - schema_id: str.
 
-            - id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.model_sync.executions.get(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.schemas.get_records(
+            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="contact",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{sync_id}/executions/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/connections/{jsonable_encoder(connection_id)}/{jsonable_encoder(schema_id)}/records",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2GetExecutionResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SchemaRecordsResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncExecutionsClient:
+class AsyncSchemasClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(self, sync_id: str) -> V2ListExecutionResponseEnvelope:
+    async def get_records(
+        self, connection_id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> SchemaRecordsResponseEnvelope:
         """
         Parameters:
-            - sync_id: str.
-        ---
-        from polytomic.client import AsyncPolytomic
+            - connection_id: str.
 
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.model_sync.executions.list(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{sync_id}/executions"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ListExecutionResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(self, sync_id: str, id: str) -> V2GetExecutionResponseEnvelope:
-        """
-        Parameters:
-            - sync_id: str.
+            - schema_id: str.
 
-            - id: str.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.model_sync.executions.get(
-            sync_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.schemas.get_records(
+            connection_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="contact",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/syncs/{sync_id}/executions/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/connections/{jsonable_encoder(connection_id)}/{jsonable_encoder(schema_id)}/records",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2GetExecutionResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SchemaRecordsResponseEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.0/src/polytomic/resources/model_sync/types/v_2_create_sync_request_mode.py` & `polytomic-0.1.2/src/polytomic/types/bulk_schema_execution_status.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class V2CreateSyncRequestMode(str, enum.Enum):
-    UPDATE = "update"
-    UPDATE_OR_CREATE = "updateOrCreate"
-    CREATE = "create"
-    REPLACE = "replace"
-    APPEND = "append"
-    SNAPSHOT = "snapshot"
+class BulkSchemaExecutionStatus(str, enum.Enum):
+    CREATED = "created"
+    SCHEDULED = "scheduled"
+    RUNNING = "running"
+    EXPORTING = "exporting"
+    CANCELED = "canceled"
+    COMPLETED = "completed"
+    FAILED = "failed"
 
     def visit(
         self,
-        update: typing.Callable[[], T_Result],
-        update_or_create: typing.Callable[[], T_Result],
-        create: typing.Callable[[], T_Result],
-        replace: typing.Callable[[], T_Result],
-        append: typing.Callable[[], T_Result],
-        snapshot: typing.Callable[[], T_Result],
+        created: typing.Callable[[], T_Result],
+        scheduled: typing.Callable[[], T_Result],
+        running: typing.Callable[[], T_Result],
+        exporting: typing.Callable[[], T_Result],
+        canceled: typing.Callable[[], T_Result],
+        completed: typing.Callable[[], T_Result],
+        failed: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is V2CreateSyncRequestMode.UPDATE:
-            return update()
-        if self is V2CreateSyncRequestMode.UPDATE_OR_CREATE:
-            return update_or_create()
-        if self is V2CreateSyncRequestMode.CREATE:
-            return create()
-        if self is V2CreateSyncRequestMode.REPLACE:
-            return replace()
-        if self is V2CreateSyncRequestMode.APPEND:
-            return append()
-        if self is V2CreateSyncRequestMode.SNAPSHOT:
-            return snapshot()
+        if self is BulkSchemaExecutionStatus.CREATED:
+            return created()
+        if self is BulkSchemaExecutionStatus.SCHEDULED:
+            return scheduled()
+        if self is BulkSchemaExecutionStatus.RUNNING:
+            return running()
+        if self is BulkSchemaExecutionStatus.EXPORTING:
+            return exporting()
+        if self is BulkSchemaExecutionStatus.CANCELED:
+            return canceled()
+        if self is BulkSchemaExecutionStatus.COMPLETED:
+            return completed()
+        if self is BulkSchemaExecutionStatus.FAILED:
+            return failed()
```

### Comparing `polytomic-0.1.0/src/polytomic/resources/permissions/client.py` & `polytomic-0.1.2/src/polytomic/resources/permissions/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .resources.policies.client import AsyncPoliciesClient, PoliciesClient
 from .resources.roles.client import AsyncRolesClient, RolesClient
 
 
 class PermissionsClient:
```

### Comparing `polytomic-0.1.0/src/polytomic/resources/permissions/resources/policies/client.py` & `polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/executions/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,432 +1,401 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from .....core.api_error import ApiError
 from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
+from .....core.request_options import RequestOptions
 from .....errors.unauthorized_error import UnauthorizedError
+from .....types.bulk_sync_execution_envelope import BulkSyncExecutionEnvelope
+from .....types.list_bulk_sync_executions_envelope import ListBulkSyncExecutionsEnvelope
 from .....types.rest_err_response import RestErrResponse
-from .....types.v_2_list_policies_response_envelope import V2ListPoliciesResponseEnvelope
-from .....types.v_2_policy_action import V2PolicyAction
-from .....types.v_2_policy_response_envelope import V2PolicyResponseEnvelope
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class PoliciesClient:
+class ExecutionsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self) -> V2ListPoliciesResponseEnvelope:
-        """
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.permissions.policies.list()
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ListPoliciesResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def create(
-        self,
-        *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.List[V2PolicyAction]] = OMIT,
-    ) -> V2PolicyResponseEnvelope:
-        """
-        Parameters:
-            - name: str.
-
-            - organization_id: typing.Optional[str].
-
-            - policy_actions: typing.Optional[typing.List[V2PolicyAction]].
-        ---
-        from polytomic import V2PolicyAction
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.permissions.policies.create(
-            name="Custom",
-            policy_actions=[
-                V2PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2PolicyResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get(self, id: str) -> V2PolicyResponseEnvelope:
+    def list(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ListBulkSyncExecutionsEnvelope:
         """
         Parameters:
             - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.get(
+        client.bulk_sync.executions.list(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSyncExecutionsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete(self, id: str) -> None:
+    def start(
+        self,
+        id: str,
+        *,
+        resync: typing.Optional[bool] = OMIT,
+        schemas: typing.Optional[typing.Sequence[str]] = OMIT,
+        test: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> BulkSyncExecutionEnvelope:
         """
         Parameters:
             - id: str.
+
+            - resync: typing.Optional[bool].
+
+            - schemas: typing.Optional[typing.Sequence[str]].
+
+            - test: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.delete(
+        client.bulk_sync.executions.start(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            resync=False,
+            test=False,
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if resync is not OMIT:
+            _request["resync"] = resync
+        if schemas is not OMIT:
+            _request["schemas"] = schemas
+        if test is not OMIT:
+            _request["test"] = test
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "POST",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(
-        self,
-        id: str,
-        *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.List[V2PolicyAction]] = OMIT,
-    ) -> V2PolicyResponseEnvelope:
+    def get(
+        self, id: str, exec_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncExecutionEnvelope:
         """
         Parameters:
             - id: str.
 
-            - name: str.
+            - exec_id: str.
 
-            - organization_id: typing.Optional[str].
-
-            - policy_actions: typing.Optional[typing.List[V2PolicyAction]].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import V2PolicyAction
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.permissions.policies.update(
+        client.bulk_sync.executions.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="Custom",
-            policy_actions=[
-                V2PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
+            exec_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/executions/{jsonable_encoder(exec_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncPoliciesClient:
+class AsyncExecutionsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(self) -> V2ListPoliciesResponseEnvelope:
-        """
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.permissions.policies.list()
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ListPoliciesResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def create(
-        self,
-        *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.List[V2PolicyAction]] = OMIT,
-    ) -> V2PolicyResponseEnvelope:
-        """
-        Parameters:
-            - name: str.
-
-            - organization_id: typing.Optional[str].
-
-            - policy_actions: typing.Optional[typing.List[V2PolicyAction]].
-        ---
-        from polytomic import V2PolicyAction
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.permissions.policies.create(
-            name="Custom",
-            policy_actions=[
-                V2PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "api/permissions/policies"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2PolicyResponseEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(self, id: str) -> V2PolicyResponseEnvelope:
+    async def list(
+        self, id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> ListBulkSyncExecutionsEnvelope:
         """
         Parameters:
             - id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.get(
+        await client.bulk_sync.executions.list(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSyncExecutionsEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete(self, id: str) -> None:
+    async def start(
+        self,
+        id: str,
+        *,
+        resync: typing.Optional[bool] = OMIT,
+        schemas: typing.Optional[typing.Sequence[str]] = OMIT,
+        test: typing.Optional[bool] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> BulkSyncExecutionEnvelope:
         """
         Parameters:
             - id: str.
+
+            - resync: typing.Optional[bool].
+
+            - schemas: typing.Optional[typing.Sequence[str]].
+
+            - test: typing.Optional[bool].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.delete(
+        await client.bulk_sync.executions.start(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            resync=False,
+            test=False,
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if resync is not OMIT:
+            _request["resync"] = resync
+        if schemas is not OMIT:
+            _request["schemas"] = schemas
+        if test is not OMIT:
+            _request["test"] = test
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "POST",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/executions"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(
-        self,
-        id: str,
-        *,
-        name: str,
-        organization_id: typing.Optional[str] = OMIT,
-        policy_actions: typing.Optional[typing.List[V2PolicyAction]] = OMIT,
-    ) -> V2PolicyResponseEnvelope:
+    async def get(
+        self, id: str, exec_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSyncExecutionEnvelope:
         """
         Parameters:
             - id: str.
 
-            - name: str.
+            - exec_id: str.
 
-            - organization_id: typing.Optional[str].
-
-            - policy_actions: typing.Optional[typing.List[V2PolicyAction]].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from polytomic import V2PolicyAction
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.permissions.policies.update(
+        await client.bulk_sync.executions.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            name="Custom",
-            policy_actions=[
-                V2PolicyAction(
-                    action="read",
-                    role_ids=["248df4b7-aa70-47b8-a036-33ac447e668d"],
-                )
-            ],
+            exec_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"name": name}
-        if organization_id is not OMIT:
-            _request["organization_id"] = organization_id
-        if policy_actions is not OMIT:
-            _request["policy_actions"] = policy_actions
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/permissions/policies/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/executions/{jsonable_encoder(exec_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2PolicyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSyncExecutionEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `polytomic-0.1.0/src/polytomic/resources/users/client.py` & `polytomic-0.1.2/src/polytomic/resources/bulk_sync/resources/schemas/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,525 +1,442 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
-from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ...core.jsonable_encoder import jsonable_encoder
-from ...core.remove_none_from_dict import remove_none_from_dict
-from ...errors.unauthorized_error import UnauthorizedError
-from ...types.rest_err_response import RestErrResponse
-from ...types.v_2_api_key_response_envelope import V2ApiKeyResponseEnvelope
-from ...types.v_2_list_users_envelope import V2ListUsersEnvelope
-from ...types.v_2_user_envelope import V2UserEnvelope
+from .....core.api_error import ApiError
+from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .....core.jsonable_encoder import jsonable_encoder
+from .....core.remove_none_from_dict import remove_none_from_dict
+from .....core.request_options import RequestOptions
+from .....errors.unauthorized_error import UnauthorizedError
+from .....types.bulk_field import BulkField
+from .....types.bulk_schema_envelope import BulkSchemaEnvelope
+from .....types.list_bulk_schema import ListBulkSchema
+from .....types.rest_err_response import RestErrResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class UsersClient:
+class SchemasClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self, org_id: str) -> V2ListUsersEnvelope:
+    def list(
+        self,
+        id: str,
+        *,
+        filters: typing.Optional[typing.Dict[str, typing.Optional[str]]] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListBulkSchema:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
-        Parameters:
-            - org_id: str.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.users.list(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ListUsersEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def create(self, org_id: str, *, email: str, role: typing.Optional[str] = OMIT) -> V2UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
-        Parameters:
-            - org_id: str.
-
-            - email: str.
-
-            - role: typing.Optional[str].
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.users.create(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="email",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get(self, id: str, org_id: str) -> V2UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
+            - filters: typing.Optional[typing.Dict[str, typing.Optional[str]]].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.get(
+        client.bulk_sync.schemas.list(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+            ),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "filters": jsonable_encoder(filters),
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def remove(self, id: str, org_id: str) -> V2UserEnvelope:
+    def update(
+        self,
+        id: str,
+        schema_id: str,
+        *,
+        enabled: typing.Optional[bool] = OMIT,
+        fields: typing.Optional[typing.Sequence[BulkField]] = OMIT,
+        partition_key: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> BulkSchemaEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
-        ---
-        from polytomic.client import Polytomic
-
-        client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        client.users.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def update(self, id: str, org_id: str, *, email: str, role: typing.Optional[str] = OMIT) -> V2UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+            - schema_id: str.
 
-        Parameters:
-            - id: str.
+            - enabled: typing.Optional[bool].
 
-            - org_id: str.
+            - fields: typing.Optional[typing.Sequence[BulkField]].
 
-            - email: str.
+            - partition_key: typing.Optional[str].
 
-            - role: typing.Optional[str].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.update(
+        client.bulk_sync.schemas.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="email",
+            schema_id="contact",
+            enabled=True,
+            partition_key="email",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
+        _request: typing.Dict[str, typing.Any] = {}
+        if enabled is not OMIT:
+            _request["enabled"] = enabled
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if partition_key is not OMIT:
+            _request["partition_key"] = partition_key
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_api_key(self, org_id: str, id: str, *, force: typing.Optional[bool] = None) -> V2ApiKeyResponseEnvelope:
+    def get(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSchemaEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
-            - org_id: str.
-
             - id: str.
 
-            - force: typing.Optional[bool].
+            - schema_id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import Polytomic
 
         client = Polytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        client.users.create_api_key(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        client.bulk_sync.schemas.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="Contact",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
+            "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}/keys"
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            params=remove_none_from_dict({"force": force}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ApiKeyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncUsersClient:
+class AsyncSchemasClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(self, org_id: str) -> V2ListUsersEnvelope:
+    async def list(
+        self,
+        id: str,
+        *,
+        filters: typing.Optional[typing.Dict[str, typing.Optional[str]]] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListBulkSchema:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
-        Parameters:
-            - org_id: str.
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.users.list(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ListUsersEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def create(self, org_id: str, *, email: str, role: typing.Optional[str] = OMIT) -> V2UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
-        Parameters:
-            - org_id: str.
-
-            - email: str.
-
-            - role: typing.Optional[str].
-        ---
-        from polytomic.client import AsyncPolytomic
-
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.users.create(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="email",
-        )
-        """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get(self, id: str, org_id: str) -> V2UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
+            - filters: typing.Optional[typing.Dict[str, typing.Optional[str]]].
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.get(
+        await client.bulk_sync.schemas.list(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"api/bulk/syncs/{jsonable_encoder(id)}/schemas"
+            ),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "filters": jsonable_encoder(filters),
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ListBulkSchema, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def remove(self, id: str, org_id: str) -> V2UserEnvelope:
+    async def update(
+        self,
+        id: str,
+        schema_id: str,
+        *,
+        enabled: typing.Optional[bool] = OMIT,
+        fields: typing.Optional[typing.Sequence[BulkField]] = OMIT,
+        partition_key: typing.Optional[str] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> BulkSchemaEnvelope:
         """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
         Parameters:
             - id: str.
 
-            - org_id: str.
-        ---
-        from polytomic.client import AsyncPolytomic
+            - schema_id: str.
 
-        client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
-            token="YOUR_TOKEN",
-        )
-        await client.users.remove(
-            id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-        )
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            - enabled: typing.Optional[bool].
 
-    async def update(self, id: str, org_id: str, *, email: str, role: typing.Optional[str] = OMIT) -> V2UserEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
+            - fields: typing.Optional[typing.Sequence[BulkField]].
 
-        Parameters:
-            - id: str.
-
-            - org_id: str.
+            - partition_key: typing.Optional[str].
 
-            - email: str.
-
-            - role: typing.Optional[str].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.update(
+        await client.bulk_sync.schemas.update(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
-            email="email",
+            schema_id="contact",
+            enabled=True,
+            partition_key="email",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"email": email}
-        if role is not OMIT:
-            _request["role"] = role
+        _request: typing.Dict[str, typing.Any] = {}
+        if enabled is not OMIT:
+            _request["enabled"] = enabled
+        if fields is not OMIT:
+            _request["fields"] = fields
+        if partition_key is not OMIT:
+            _request["partition_key"] = partition_key
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2UserEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_api_key(
-        self, org_id: str, id: str, *, force: typing.Optional[bool] = None
-    ) -> V2ApiKeyResponseEnvelope:
-        """
-        > 🚧 Requires partner key
-        >
-        > User endpoints are only accessible using [partner keys](https://docs.polytomic.com/reference/authentication#partner-keys)
-
+    async def get(
+        self, id: str, schema_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> BulkSchemaEnvelope:
+        """
         Parameters:
-            - org_id: str.
-
             - id: str.
 
-            - force: typing.Optional[bool].
+            - schema_id: str.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from polytomic.client import AsyncPolytomic
 
         client = AsyncPolytomic(
-            polytomic_version="YOUR_POLYTOMIC_VERSION",
+            x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
             token="YOUR_TOKEN",
         )
-        await client.users.create_api_key(
-            org_id="248df4b7-aa70-47b8-a036-33ac447e668d",
+        await client.bulk_sync.schemas.get(
             id="248df4b7-aa70-47b8-a036-33ac447e668d",
+            schema_id="Contact",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
+            "GET",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"api/organizations/{org_id}/users/{id}/keys"
+                f"{self._client_wrapper.get_base_url()}/",
+                f"api/bulk/syncs/{jsonable_encoder(id)}/schemas/{jsonable_encoder(schema_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
             ),
-            params=remove_none_from_dict({"force": force}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(V2ApiKeyResponseEnvelope, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BulkSchemaEnvelope, _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(RestErrResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `polytomic-0.1.0/src/polytomic/types/__init__.py` & `polytomic-0.1.2/src/polytomic/types/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,209 +1,253 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .activate_sync_envelope import ActivateSyncEnvelope
+from .activate_sync_input import ActivateSyncInput
+from .activate_sync_output import ActivateSyncOutput
+from .api_key_response import ApiKeyResponse
+from .api_key_response_envelope import ApiKeyResponseEnvelope
+from .bulk_discover import BulkDiscover
+from .bulk_execution_status import BulkExecutionStatus
+from .bulk_field import BulkField
+from .bulk_itemized_schedule import BulkItemizedSchedule
+from .bulk_multi_schedule_configuration import BulkMultiScheduleConfiguration
 from .bulk_schedule import BulkSchedule
+from .bulk_schema import BulkSchema
+from .bulk_schema_envelope import BulkSchemaEnvelope
+from .bulk_schema_execution_status import BulkSchemaExecutionStatus
+from .bulk_selective_mode import BulkSelectiveMode
+from .bulk_sync_dest import BulkSyncDest
+from .bulk_sync_dest_envelope import BulkSyncDestEnvelope
+from .bulk_sync_execution import BulkSyncExecution
+from .bulk_sync_execution_envelope import BulkSyncExecutionEnvelope
+from .bulk_sync_list_envelope import BulkSyncListEnvelope
+from .bulk_sync_response import BulkSyncResponse
+from .bulk_sync_response_envelope import BulkSyncResponseEnvelope
+from .bulk_sync_schema_execution import BulkSyncSchemaExecution
+from .bulk_sync_source import BulkSyncSource
+from .bulk_sync_source_envelope import BulkSyncSourceEnvelope
+from .bulk_sync_source_schema_envelope import BulkSyncSourceSchemaEnvelope
+from .bulk_sync_source_status import BulkSyncSourceStatus
+from .bulk_sync_source_status_envelope import BulkSyncSourceStatusEnvelope
+from .bulk_sync_status_envelope import BulkSyncStatusEnvelope
+from .bulk_sync_status_response import BulkSyncStatusResponse
+from .configuration_value import ConfigurationValue
+from .connect_card_response import ConnectCardResponse
+from .connect_card_response_envelope import ConnectCardResponseEnvelope
+from .connection_list_response_envelope import ConnectionListResponseEnvelope
+from .connection_meta import ConnectionMeta
+from .connection_meta_response import ConnectionMetaResponse
+from .connection_parameter_value import ConnectionParameterValue
+from .connection_parameter_values_resp import ConnectionParameterValuesResp
+from .connection_parameter_values_response_envelope import ConnectionParameterValuesResponseEnvelope
+from .connection_response_envelope import ConnectionResponseEnvelope
+from .connection_response_schema import ConnectionResponseSchema
+from .connection_type import ConnectionType
+from .connection_type_response_envelope import ConnectionTypeResponseEnvelope
+from .connection_type_schema import ConnectionTypeSchema
+from .create_connection_response_envelope import CreateConnectionResponseEnvelope
+from .create_connection_response_schema import CreateConnectionResponseSchema
+from .event import Event
+from .event_types_envelope import EventTypesEnvelope
+from .events_envelope import EventsEnvelope
+from .execution_counts import ExecutionCounts
+from .execution_log_response import ExecutionLogResponse
+from .execution_logs_response_envelope import ExecutionLogsResponseEnvelope
+from .execution_status import ExecutionStatus
+from .filter import Filter
+from .get_connection_meta_envelope import GetConnectionMetaEnvelope
+from .get_execution_response_envelope import GetExecutionResponseEnvelope
+from .get_execution_response_schema import GetExecutionResponseSchema
+from .get_identity_response_envelope import GetIdentityResponseEnvelope
+from .get_identity_response_schema import GetIdentityResponseSchema
+from .identity import Identity
+from .identity_function import IdentityFunction
+from .job_response import JobResponse
+from .job_response_envelope import JobResponseEnvelope
+from .jsonschema_form import JsonschemaForm
 from .label_label import LabelLabel
+from .list_bulk_schema import ListBulkSchema
+from .list_bulk_sync_executions_envelope import ListBulkSyncExecutionsEnvelope
+from .list_execution_response_envelope import ListExecutionResponseEnvelope
+from .list_model_sync_response_envelope import ListModelSyncResponseEnvelope
+from .list_policies_response_envelope import ListPoliciesResponseEnvelope
+from .list_users_envelope import ListUsersEnvelope
+from .mode import Mode
+from .model_field import ModelField
+from .model_field_response import ModelFieldResponse
+from .model_list_response_envelope import ModelListResponseEnvelope
+from .model_model_field_request import ModelModelFieldRequest
+from .model_relation import ModelRelation
+from .model_relation_to import ModelRelationTo
+from .model_response import ModelResponse
+from .model_response_envelope import ModelResponseEnvelope
+from .model_sync_field import ModelSyncField
+from .model_sync_response import ModelSyncResponse
+from .model_sync_response_envelope import ModelSyncResponseEnvelope
+from .organization import Organization
+from .organization_envelope import OrganizationEnvelope
+from .organizations_envelope import OrganizationsEnvelope
+from .override import Override
+from .pick_value import PickValue
+from .policy_action import PolicyAction
+from .policy_response import PolicyResponse
+from .policy_response_envelope import PolicyResponseEnvelope
+from .relation import Relation
+from .relation_to import RelationTo
 from .rest_err_response import RestErrResponse
+from .role_list_response_envelope import RoleListResponseEnvelope
+from .role_response import RoleResponse
+from .role_response_envelope import RoleResponseEnvelope
+from .run_after import RunAfter
+from .schedule import Schedule
+from .schedule_frequency import ScheduleFrequency
+from .schedule_option_response import ScheduleOptionResponse
+from .schedule_option_response_envelope import ScheduleOptionResponseEnvelope
+from .schedule_schedule_option import ScheduleScheduleOption
+from .schema import Schema
 from .schema_association import SchemaAssociation
+from .schema_field import SchemaField
+from .schema_records_response_envelope import SchemaRecordsResponseEnvelope
+from .source import Source
+from .start_model_sync_response_envelope import StartModelSyncResponseEnvelope
+from .start_model_sync_response_schema import StartModelSyncResponseSchema
+from .supported_mode import SupportedMode
 from .sync_destination_properties import SyncDestinationProperties
-from .v_2_activate_sync_envelope import V2ActivateSyncEnvelope
-from .v_2_activate_sync_input import V2ActivateSyncInput
-from .v_2_activate_sync_output import V2ActivateSyncOutput
-from .v_2_api_key_response import V2ApiKeyResponse
-from .v_2_api_key_response_envelope import V2ApiKeyResponseEnvelope
-from .v_2_bulk_sync_dest import V2BulkSyncDest
-from .v_2_bulk_sync_dest_envelope import V2BulkSyncDestEnvelope
-from .v_2_bulk_sync_list_envelope import V2BulkSyncListEnvelope
-from .v_2_bulk_sync_response import V2BulkSyncResponse
-from .v_2_bulk_sync_response_envelope import V2BulkSyncResponseEnvelope
-from .v_2_configuration_value import V2ConfigurationValue
-from .v_2_connection_list_response_envelope import V2ConnectionListResponseEnvelope
-from .v_2_connection_meta import V2ConnectionMeta
-from .v_2_connection_meta_response import V2ConnectionMetaResponse
-from .v_2_connection_response_envelope import V2ConnectionResponseEnvelope
-from .v_2_connection_response_schema import V2ConnectionResponseSchema
-from .v_2_connection_type import V2ConnectionType
-from .v_2_connection_type_response_envelope import V2ConnectionTypeResponseEnvelope
-from .v_2_connection_type_schema import V2ConnectionTypeSchema
-from .v_2_create_connection_response_envelope import V2CreateConnectionResponseEnvelope
-from .v_2_create_connection_response_schema import V2CreateConnectionResponseSchema
-from .v_2_event import V2Event
-from .v_2_event_types_envelope import V2EventTypesEnvelope
-from .v_2_events_envelope import V2EventsEnvelope
-from .v_2_execution_counts import V2ExecutionCounts
-from .v_2_filter import V2Filter
-from .v_2_get_connection_meta_envelope import V2GetConnectionMetaEnvelope
-from .v_2_get_execution_response_envelope import V2GetExecutionResponseEnvelope
-from .v_2_get_execution_response_schema import V2GetExecutionResponseSchema
-from .v_2_get_identity_response_envelope import V2GetIdentityResponseEnvelope
-from .v_2_get_identity_response_schema import V2GetIdentityResponseSchema
-from .v_2_identity import V2Identity
-from .v_2_identity_function import V2IdentityFunction
-from .v_2_list_execution_response_envelope import V2ListExecutionResponseEnvelope
-from .v_2_list_policies_response_envelope import V2ListPoliciesResponseEnvelope
-from .v_2_list_sync_response_envelope import V2ListSyncResponseEnvelope
-from .v_2_list_users_envelope import V2ListUsersEnvelope
-from .v_2_mode import V2Mode
-from .v_2_model_field import V2ModelField
-from .v_2_model_field_request import V2ModelFieldRequest
-from .v_2_model_field_response import V2ModelFieldResponse
-from .v_2_model_list_response_envelope import V2ModelListResponseEnvelope
-from .v_2_model_response import V2ModelResponse
-from .v_2_model_response_envelope import V2ModelResponseEnvelope
-from .v_2_organization import V2Organization
-from .v_2_organization_envelope import V2OrganizationEnvelope
-from .v_2_organizations_envelope import V2OrganizationsEnvelope
-from .v_2_override import V2Override
-from .v_2_policy_action import V2PolicyAction
-from .v_2_policy_response import V2PolicyResponse
-from .v_2_policy_response_envelope import V2PolicyResponseEnvelope
-from .v_2_relation import V2Relation
-from .v_2_relation_to import V2RelationTo
-from .v_2_role_list_response_envelope import V2RoleListResponseEnvelope
-from .v_2_role_response import V2RoleResponse
-from .v_2_role_response_envelope import V2RoleResponseEnvelope
-from .v_2_run_after import V2RunAfter
-from .v_2_schedule import V2Schedule
-from .v_2_source import V2Source
-from .v_2_start_sync_response_envelope import V2StartSyncResponseEnvelope
-from .v_2_start_sync_response_schema import V2StartSyncResponseSchema
-from .v_2_supported_mode import V2SupportedMode
-from .v_2_sync_field import V2SyncField
-from .v_2_sync_response import V2SyncResponse
-from .v_2_sync_response_envelope import V2SyncResponseEnvelope
-from .v_2_sync_status_envelope import V2SyncStatusEnvelope
-from .v_2_sync_status_response import V2SyncStatusResponse
-from .v_2_target import V2Target
-from .v_2_target_field import V2TargetField
-from .v_2_target_response import V2TargetResponse
-from .v_2_target_response_envelope import V2TargetResponseEnvelope
-from .v_2_user import V2User
-from .v_2_user_envelope import V2UserEnvelope
-from .v_2_webhook import V2Webhook
-from .v_2_webhook_envelope import V2WebhookEnvelope
-from .v_2_webhook_list_envelope import V2WebhookListEnvelope
-from .v_3_bulk_field import V3BulkField
-from .v_3_bulk_schema import V3BulkSchema
-from .v_3_bulk_schema_envelope import V3BulkSchemaEnvelope
-from .v_3_bulk_sync_execution import V3BulkSyncExecution
-from .v_3_bulk_sync_execution_envelope import V3BulkSyncExecutionEnvelope
-from .v_3_bulk_sync_schema_execution import V3BulkSyncSchemaExecution
-from .v_3_bulk_sync_source import V3BulkSyncSource
-from .v_3_bulk_sync_source_envelope import V3BulkSyncSourceEnvelope
-from .v_3_bulk_sync_source_schema_envelope import V3BulkSyncSourceSchemaEnvelope
-from .v_3_bulk_sync_source_status import V3BulkSyncSourceStatus
-from .v_3_bulk_sync_source_status_envelope import V3BulkSyncSourceStatusEnvelope
-from .v_3_bulk_sync_status_envelope import V3BulkSyncStatusEnvelope
-from .v_3_bulk_sync_status_response import V3BulkSyncStatusResponse
-from .v_3_connect_card_response import V3ConnectCardResponse
-from .v_3_connect_card_response_envelope import V3ConnectCardResponseEnvelope
-from .v_3_list_bulk_schema_envelope import V3ListBulkSchemaEnvelope
-from .v_3_list_bulk_sync_executions_envelope import V3ListBulkSyncExecutionsEnvelope
-from .v_3_pick_value import V3PickValue
-from .v_3_schema import V3Schema
-from .v_3_schema_field import V3SchemaField
-from .v_3_schema_records_response_envelope import V3SchemaRecordsResponseEnvelope
+from .sync_status_envelope import SyncStatusEnvelope
+from .sync_status_response import SyncStatusResponse
+from .target import Target
+from .target_field import TargetField
+from .target_response import TargetResponse
+from .target_response_envelope import TargetResponseEnvelope
+from .user import User
+from .user_envelope import UserEnvelope
+from .webhook import Webhook
+from .webhook_envelope import WebhookEnvelope
+from .webhook_list_envelope import WebhookListEnvelope
+from .work_task_status import WorkTaskStatus
 
 __all__ = [
+    "ActivateSyncEnvelope",
+    "ActivateSyncInput",
+    "ActivateSyncOutput",
+    "ApiKeyResponse",
+    "ApiKeyResponseEnvelope",
+    "BulkDiscover",
+    "BulkExecutionStatus",
+    "BulkField",
+    "BulkItemizedSchedule",
+    "BulkMultiScheduleConfiguration",
     "BulkSchedule",
+    "BulkSchema",
+    "BulkSchemaEnvelope",
+    "BulkSchemaExecutionStatus",
+    "BulkSelectiveMode",
+    "BulkSyncDest",
+    "BulkSyncDestEnvelope",
+    "BulkSyncExecution",
+    "BulkSyncExecutionEnvelope",
+    "BulkSyncListEnvelope",
+    "BulkSyncResponse",
+    "BulkSyncResponseEnvelope",
+    "BulkSyncSchemaExecution",
+    "BulkSyncSource",
+    "BulkSyncSourceEnvelope",
+    "BulkSyncSourceSchemaEnvelope",
+    "BulkSyncSourceStatus",
+    "BulkSyncSourceStatusEnvelope",
+    "BulkSyncStatusEnvelope",
+    "BulkSyncStatusResponse",
+    "ConfigurationValue",
+    "ConnectCardResponse",
+    "ConnectCardResponseEnvelope",
+    "ConnectionListResponseEnvelope",
+    "ConnectionMeta",
+    "ConnectionMetaResponse",
+    "ConnectionParameterValue",
+    "ConnectionParameterValuesResp",
+    "ConnectionParameterValuesResponseEnvelope",
+    "ConnectionResponseEnvelope",
+    "ConnectionResponseSchema",
+    "ConnectionType",
+    "ConnectionTypeResponseEnvelope",
+    "ConnectionTypeSchema",
+    "CreateConnectionResponseEnvelope",
+    "CreateConnectionResponseSchema",
+    "Event",
+    "EventTypesEnvelope",
+    "EventsEnvelope",
+    "ExecutionCounts",
+    "ExecutionLogResponse",
+    "ExecutionLogsResponseEnvelope",
+    "ExecutionStatus",
+    "Filter",
+    "GetConnectionMetaEnvelope",
+    "GetExecutionResponseEnvelope",
+    "GetExecutionResponseSchema",
+    "GetIdentityResponseEnvelope",
+    "GetIdentityResponseSchema",
+    "Identity",
+    "IdentityFunction",
+    "JobResponse",
+    "JobResponseEnvelope",
+    "JsonschemaForm",
     "LabelLabel",
+    "ListBulkSchema",
+    "ListBulkSyncExecutionsEnvelope",
+    "ListExecutionResponseEnvelope",
+    "ListModelSyncResponseEnvelope",
+    "ListPoliciesResponseEnvelope",
+    "ListUsersEnvelope",
+    "Mode",
+    "ModelField",
+    "ModelFieldResponse",
+    "ModelListResponseEnvelope",
+    "ModelModelFieldRequest",
+    "ModelRelation",
+    "ModelRelationTo",
+    "ModelResponse",
+    "ModelResponseEnvelope",
+    "ModelSyncField",
+    "ModelSyncResponse",
+    "ModelSyncResponseEnvelope",
+    "Organization",
+    "OrganizationEnvelope",
+    "OrganizationsEnvelope",
+    "Override",
+    "PickValue",
+    "PolicyAction",
+    "PolicyResponse",
+    "PolicyResponseEnvelope",
+    "Relation",
+    "RelationTo",
     "RestErrResponse",
+    "RoleListResponseEnvelope",
+    "RoleResponse",
+    "RoleResponseEnvelope",
+    "RunAfter",
+    "Schedule",
+    "ScheduleFrequency",
+    "ScheduleOptionResponse",
+    "ScheduleOptionResponseEnvelope",
+    "ScheduleScheduleOption",
+    "Schema",
     "SchemaAssociation",
+    "SchemaField",
+    "SchemaRecordsResponseEnvelope",
+    "Source",
+    "StartModelSyncResponseEnvelope",
+    "StartModelSyncResponseSchema",
+    "SupportedMode",
     "SyncDestinationProperties",
-    "V2ActivateSyncEnvelope",
-    "V2ActivateSyncInput",
-    "V2ActivateSyncOutput",
-    "V2ApiKeyResponse",
-    "V2ApiKeyResponseEnvelope",
-    "V2BulkSyncDest",
-    "V2BulkSyncDestEnvelope",
-    "V2BulkSyncListEnvelope",
-    "V2BulkSyncResponse",
-    "V2BulkSyncResponseEnvelope",
-    "V2ConfigurationValue",
-    "V2ConnectionListResponseEnvelope",
-    "V2ConnectionMeta",
-    "V2ConnectionMetaResponse",
-    "V2ConnectionResponseEnvelope",
-    "V2ConnectionResponseSchema",
-    "V2ConnectionType",
-    "V2ConnectionTypeResponseEnvelope",
-    "V2ConnectionTypeSchema",
-    "V2CreateConnectionResponseEnvelope",
-    "V2CreateConnectionResponseSchema",
-    "V2Event",
-    "V2EventTypesEnvelope",
-    "V2EventsEnvelope",
-    "V2ExecutionCounts",
-    "V2Filter",
-    "V2GetConnectionMetaEnvelope",
-    "V2GetExecutionResponseEnvelope",
-    "V2GetExecutionResponseSchema",
-    "V2GetIdentityResponseEnvelope",
-    "V2GetIdentityResponseSchema",
-    "V2Identity",
-    "V2IdentityFunction",
-    "V2ListExecutionResponseEnvelope",
-    "V2ListPoliciesResponseEnvelope",
-    "V2ListSyncResponseEnvelope",
-    "V2ListUsersEnvelope",
-    "V2Mode",
-    "V2ModelField",
-    "V2ModelFieldRequest",
-    "V2ModelFieldResponse",
-    "V2ModelListResponseEnvelope",
-    "V2ModelResponse",
-    "V2ModelResponseEnvelope",
-    "V2Organization",
-    "V2OrganizationEnvelope",
-    "V2OrganizationsEnvelope",
-    "V2Override",
-    "V2PolicyAction",
-    "V2PolicyResponse",
-    "V2PolicyResponseEnvelope",
-    "V2Relation",
-    "V2RelationTo",
-    "V2RoleListResponseEnvelope",
-    "V2RoleResponse",
-    "V2RoleResponseEnvelope",
-    "V2RunAfter",
-    "V2Schedule",
-    "V2Source",
-    "V2StartSyncResponseEnvelope",
-    "V2StartSyncResponseSchema",
-    "V2SupportedMode",
-    "V2SyncField",
-    "V2SyncResponse",
-    "V2SyncResponseEnvelope",
-    "V2SyncStatusEnvelope",
-    "V2SyncStatusResponse",
-    "V2Target",
-    "V2TargetField",
-    "V2TargetResponse",
-    "V2TargetResponseEnvelope",
-    "V2User",
-    "V2UserEnvelope",
-    "V2Webhook",
-    "V2WebhookEnvelope",
-    "V2WebhookListEnvelope",
-    "V3BulkField",
-    "V3BulkSchema",
-    "V3BulkSchemaEnvelope",
-    "V3BulkSyncExecution",
-    "V3BulkSyncExecutionEnvelope",
-    "V3BulkSyncSchemaExecution",
-    "V3BulkSyncSource",
-    "V3BulkSyncSourceEnvelope",
-    "V3BulkSyncSourceSchemaEnvelope",
-    "V3BulkSyncSourceStatus",
-    "V3BulkSyncSourceStatusEnvelope",
-    "V3BulkSyncStatusEnvelope",
-    "V3BulkSyncStatusResponse",
-    "V3ConnectCardResponse",
-    "V3ConnectCardResponseEnvelope",
-    "V3ListBulkSchemaEnvelope",
-    "V3ListBulkSyncExecutionsEnvelope",
-    "V3PickValue",
-    "V3Schema",
-    "V3SchemaField",
-    "V3SchemaRecordsResponseEnvelope",
+    "SyncStatusEnvelope",
+    "SyncStatusResponse",
+    "Target",
+    "TargetField",
+    "TargetResponse",
+    "TargetResponseEnvelope",
+    "User",
+    "UserEnvelope",
+    "Webhook",
+    "WebhookEnvelope",
+    "WebhookListEnvelope",
+    "WorkTaskStatus",
 ]
```

### Comparing `polytomic-0.1.0/src/polytomic/types/bulk_schedule.py` & `polytomic-0.1.2/src/polytomic/types/connection_type_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class BulkSchedule(pydantic.BaseModel):
-    day_of_month: typing.Optional[str]
-    day_of_week: typing.Optional[str]
-    frequency: str
-    hour: typing.Optional[str]
-    minute: typing.Optional[str]
-    month: typing.Optional[str]
+class ConnectionTypeSchema(pydantic.BaseModel):
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    operations: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/rest_err_response.py` & `polytomic-0.1.2/src/polytomic/types/model_sync_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .source import Source
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class RestErrResponse(pydantic.BaseModel):
-    code: typing.Optional[int] = pydantic.Field(description="Application-specific error code.")
-    context: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(description="Application context.")
-    error: typing.Optional[str] = pydantic.Field(description="Error message.")
-    status: typing.Optional[str] = pydantic.Field(description="Status text.")
+class ModelSyncField(pydantic.BaseModel):
+    new: typing.Optional[bool] = None
+    override_value: typing.Optional[str] = None
+    source: Source
+    sync_mode: typing.Optional[str] = None
+    target: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/schema_association.py` & `polytomic-0.1.2/src/polytomic/types/api_key_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SchemaAssociation(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: typing.Optional[str]
-    reference_to: typing.Optional[typing.List[str]]
-    referenced_field: typing.Optional[str]
+class ApiKeyResponse(pydantic.BaseModel):
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/sync_destination_properties.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .schema import Schema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class SyncDestinationProperties(pydantic.BaseModel):
-    does_not_report_operation_counts: typing.Optional[bool]
-    new_target_label: typing.Optional[str]
-    optional_target_mappings: typing.Optional[bool]
-    primary_metadata_object: typing.Optional[str]
-    requires_configuration: typing.Optional[bool]
-    supports_field_creation: typing.Optional[bool]
-    supports_field_type_selection: typing.Optional[bool]
-    supports_target_filters: typing.Optional[bool]
-    target_creator: typing.Optional[bool]
-    use_field_names_as_labels: typing.Optional[bool]
+class BulkSyncSource(pydantic.BaseModel):
+    configuration: typing.Optional[typing.Any] = None
+    schemas: typing.Optional[typing.List[Schema]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_activate_sync_envelope.py` & `polytomic-0.1.2/src/polytomic/types/connect_card_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_activate_sync_output import V2ActivateSyncOutput
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ActivateSyncEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2ActivateSyncOutput]
+class ConnectCardResponse(pydantic.BaseModel):
+    redirect_url: typing.Optional[str] = None
+    token: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_activate_sync_input.py` & `polytomic-0.1.2/src/polytomic/types/connection_parameter_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ActivateSyncInput(pydantic.BaseModel):
-    active: bool
+class ConnectionParameterValue(pydantic.BaseModel):
+    label: typing.Optional[str] = None
+    value: typing.Optional[typing.Any] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_activate_sync_output.py` & `polytomic-0.1.2/src/polytomic/types/model_relation_to.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ActivateSyncOutput(pydantic.BaseModel):
-    active: typing.Optional[bool]
-    id: typing.Optional[str]
+class ModelRelationTo(pydantic.BaseModel):
+    field: typing.Optional[str] = None
+    model_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_api_key_response.py` & `polytomic-0.1.2/src/polytomic/types/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .schema_field import SchemaField
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ApiKeyResponse(pydantic.BaseModel):
-    value: typing.Optional[str]
+class Schema(pydantic.BaseModel):
+    fields: typing.Optional[typing.List[SchemaField]] = None
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_api_key_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/event_types_envelope.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_api_key_response import V2ApiKeyResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ApiKeyResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2ApiKeyResponse]
+class EventTypesEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_dest.py` & `polytomic-0.1.2/src/polytomic/types/api_key_response_envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_supported_mode import V2SupportedMode
+from .api_key_response import ApiKeyResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2BulkSyncDest(pydantic.BaseModel):
-    configuration: typing.Optional[typing.Dict[str, typing.Any]]
-    modes: typing.Optional[typing.List[V2SupportedMode]]
+class ApiKeyResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ApiKeyResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_dest_envelope.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_dest_envelope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_bulk_sync_dest import V2BulkSyncDest
+from .bulk_sync_dest import BulkSyncDest
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2BulkSyncDestEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2BulkSyncDest]
+class BulkSyncDestEnvelope(pydantic.BaseModel):
+    data: typing.Optional[BulkSyncDest] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_list_envelope.py` & `polytomic-0.1.2/src/polytomic/types/model_sync_response_envelope.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_bulk_sync_response import V2BulkSyncResponse
+from .model_sync_response import ModelSyncResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2BulkSyncListEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2BulkSyncResponse]]
+class ModelSyncResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ModelSyncResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_response.py` & `polytomic-0.1.2/src/polytomic/types/schedule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .bulk_schedule import BulkSchedule
+from .run_after import RunAfter
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2BulkSyncResponse(pydantic.BaseModel):
-    active: typing.Optional[bool]
-    destination_configuration: typing.Optional[typing.Dict[str, typing.Any]]
-    destination_connection_id: typing.Optional[str]
-    discover: typing.Optional[bool]
-    id: typing.Optional[str]
-    mode: typing.Optional[str]
-    name: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    policies: typing.Optional[typing.List[str]]
-    schedule: typing.Optional[BulkSchedule]
-    source_configuration: typing.Optional[typing.Dict[str, typing.Any]]
-    source_connection_id: typing.Optional[str]
+class Schedule(pydantic.BaseModel):
+    connection_id: typing.Optional[str] = None
+    day_of_month: typing.Optional[str] = None
+    day_of_week: typing.Optional[str] = None
+    frequency: typing.Optional[str] = None
+    hour: typing.Optional[str] = None
+    job_id: typing.Optional[int] = None
+    minute: typing.Optional[str] = None
+    month: typing.Optional[str] = None
+    run_after: typing.Optional[RunAfter] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_bulk_sync_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_schema_envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_bulk_sync_response import V2BulkSyncResponse
+from .schema import Schema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2BulkSyncResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2BulkSyncResponse]
+class BulkSyncSourceSchemaEnvelope(pydantic.BaseModel):
+    data: typing.Optional[Schema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_configuration_value.py` & `polytomic-0.1.2/src/polytomic/types/execution_counts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConfigurationValue(pydantic.BaseModel):
-    items: typing.Optional[typing.List[typing.Any]]
-    type: typing.Optional[str]
+class ExecutionCounts(pydantic.BaseModel):
+    error: typing.Optional[int] = None
+    insert: typing.Optional[int] = None
+    total: typing.Optional[int] = None
+    update: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_list_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/connection_parameter_values_resp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_connection_response_schema import V2ConnectionResponseSchema
+from .connection_parameter_value import ConnectionParameterValue
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionListResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2ConnectionResponseSchema]]
+class ConnectionParameterValuesResp(pydantic.BaseModel):
+    allows_creation: typing.Optional[bool] = None
+    values: typing.Optional[typing.List[ConnectionParameterValue]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_meta.py` & `polytomic-0.1.2/src/polytomic/types/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionMeta(pydantic.BaseModel):
-    has_items: typing.Optional[bool]
-    items: typing.Optional[typing.List[typing.Any]]
-    requires_one_of: typing.Optional[typing.List[str]]
+class Source(pydantic.BaseModel):
+    field: str
+    model_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_meta_response.py` & `polytomic-0.1.2/src/polytomic/types/webhook_envelope.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_configuration_value import V2ConfigurationValue
-from .v_2_connection_meta import V2ConnectionMeta
+from .webhook import Webhook
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionMetaResponse(pydantic.BaseModel):
-    configuration: typing.Optional[typing.Dict[str, V2ConfigurationValue]]
-    items: typing.Optional[typing.Dict[str, typing.Optional[V2ConnectionMeta]]]
-    requires_one_of: typing.Optional[typing.List[str]]
+class WebhookEnvelope(pydantic.BaseModel):
+    data: typing.Optional[Webhook] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/connection_list_response_envelope.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_connection_response_schema import V2ConnectionResponseSchema
+from .connection_response_schema import ConnectionResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2ConnectionResponseSchema]
+class ConnectionListResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ConnectionResponseSchema]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_response_schema.py` & `polytomic-0.1.2/src/polytomic/types/create_connection_response_schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,47 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_connection_type_schema import V2ConnectionTypeSchema
+from .connection_type_schema import ConnectionTypeSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionResponseSchema(pydantic.BaseModel):
-    configuration: typing.Optional[typing.Dict[str, typing.Any]]
-    id: typing.Optional[str]
-    name: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    policies: typing.Optional[typing.List[str]]
-    status: typing.Optional[str]
-    status_error: typing.Optional[str]
-    type: typing.Optional[V2ConnectionTypeSchema]
+class CreateConnectionResponseSchema(pydantic.BaseModel):
+    auth_code: typing.Optional[str] = pydantic.Field(default=None)
+    """
+    Code to enter in order to complete connection authentication.
+    """
+
+    auth_url: typing.Optional[str] = pydantic.Field(default=None)
+    """
+    URL to visit to complete connection authentication.
+    """
+
+    configuration: typing.Optional[typing.Dict[str, typing.Any]] = None
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    policies: typing.Optional[typing.List[str]] = None
+    status: typing.Optional[str] = None
+    status_error: typing.Optional[str] = None
+    type: typing.Optional[ConnectionTypeSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_type.py` & `polytomic-0.1.2/src/polytomic/types/connection_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionType(pydantic.BaseModel):
-    env_config: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(alias="envConfig")
-    id: typing.Optional[str]
-    name: typing.Optional[str]
-    use_oauth: typing.Optional[bool]
+class ConnectionType(pydantic.BaseModel):
+    env_config: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(alias="envConfig", default=None)
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    use_oauth: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_type_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/connection_type_response_envelope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_connection_type import V2ConnectionType
+from .connection_type import ConnectionType
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionTypeResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2ConnectionType]]
+class ConnectionTypeResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ConnectionType]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_connection_type_schema.py` & `polytomic-0.1.2/src/polytomic/types/role_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ConnectionTypeSchema(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: typing.Optional[str]
+class RoleResponse(pydantic.BaseModel):
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    system: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_create_connection_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/model_field_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_create_connection_response_schema import V2CreateConnectionResponseSchema
+from .model_field import ModelField
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2CreateConnectionResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2CreateConnectionResponseSchema]
+class ModelFieldResponse(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ModelField]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_create_connection_response_schema.py` & `polytomic-0.1.2/src/polytomic/types/supported_mode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_connection_type_schema import V2ConnectionTypeSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2CreateConnectionResponseSchema(pydantic.BaseModel):
-    auth_code: typing.Optional[str] = pydantic.Field(
-        description="Code to enter in order to complete connection authentication."
-    )
-    auth_url: typing.Optional[str] = pydantic.Field(description="URL to visit to complete connection authentication.")
-    configuration: typing.Optional[typing.Dict[str, typing.Any]]
-    id: typing.Optional[str]
-    name: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    policies: typing.Optional[typing.List[str]]
-    status: typing.Optional[str]
-    status_error: typing.Optional[str]
-    type: typing.Optional[V2ConnectionTypeSchema]
+class SupportedMode(pydantic.BaseModel):
+    description: typing.Optional[str] = None
+    id: typing.Optional[str] = pydantic.Field(default=None)
+    """
+    
+    """
+
+    label: typing.Optional[str] = None
+    requires_identity: typing.Optional[bool] = None
+    supports_field_sync_mode: typing.Optional[bool] = None
+    supports_target_filters: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_event.py` & `polytomic-0.1.2/src/polytomic/types/override.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Event(pydantic.BaseModel):
-    created_at: typing.Optional[dt.datetime]
-    event: typing.Optional[typing.Any]
-    id: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    type: typing.Optional[str]
+class Override(pydantic.BaseModel):
+    field_id: typing.Optional[str] = None
+    function: typing.Optional[str] = None
+    override: typing.Optional[typing.Any] = None
+    value: typing.Optional[typing.Any] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_event_types_envelope.py` & `polytomic-0.1.2/src/polytomic/types/policy_action.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2EventTypesEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[str]]
+class PolicyAction(pydantic.BaseModel):
+    action: str
+    role_ids: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_events_envelope.py` & `polytomic-0.1.2/src/polytomic/types/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_event import V2Event
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2EventsEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2Event]]
+class User(pydantic.BaseModel):
+    email: typing.Optional[str] = None
+    id: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    role: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_execution_counts.py` & `polytomic-0.1.2/src/polytomic/types/pick_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ExecutionCounts(pydantic.BaseModel):
-    error: typing.Optional[int]
-    insert: typing.Optional[int]
-    total: typing.Optional[int]
-    update: typing.Optional[int]
+class PickValue(pydantic.BaseModel):
+    label: typing.Optional[str] = None
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_filter.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_response_envelope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .bulk_sync_response import BulkSyncResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Filter(pydantic.BaseModel):
-    field_id: str
-    field_type: str
-    function: str
-    label: typing.Optional[str]
-    value: typing.Optional[typing.Any]
+class BulkSyncResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[BulkSyncResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_get_connection_meta_envelope.py` & `polytomic-0.1.2/src/polytomic/types/get_connection_meta_envelope.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_connection_meta_response import V2ConnectionMetaResponse
+from .connection_meta_response import ConnectionMetaResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2GetConnectionMetaEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2ConnectionMetaResponse]
+class GetConnectionMetaEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ConnectionMetaResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_get_execution_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/get_execution_response_envelope.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_get_execution_response_schema import V2GetExecutionResponseSchema
+from .get_execution_response_schema import GetExecutionResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2GetExecutionResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2GetExecutionResponseSchema]
+class GetExecutionResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[GetExecutionResponseSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_get_execution_response_schema.py` & `polytomic-0.1.2/src/polytomic/types/get_execution_response_schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_execution_counts import V2ExecutionCounts
+from .execution_counts import ExecutionCounts
+from .execution_status import ExecutionStatus
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2GetExecutionResponseSchema(pydantic.BaseModel):
-    completed_at: typing.Optional[dt.datetime]
-    counts: typing.Optional[V2ExecutionCounts]
-    created_at: typing.Optional[dt.datetime]
-    errors: typing.Optional[typing.List[str]]
-    id: typing.Optional[str]
-    started_at: typing.Optional[dt.datetime]
-    status: typing.Optional[str]
-    type: typing.Optional[str]
+class GetExecutionResponseSchema(pydantic.BaseModel):
+    completed_at: typing.Optional[dt.datetime] = None
+    counts: typing.Optional[ExecutionCounts] = None
+    created_at: typing.Optional[dt.datetime] = None
+    errors: typing.Optional[typing.List[str]] = None
+    id: typing.Optional[str] = None
+    started_at: typing.Optional[dt.datetime] = None
+    status: typing.Optional[ExecutionStatus] = None
+    type: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_get_identity_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/get_identity_response_envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_get_identity_response_schema import V2GetIdentityResponseSchema
+from .get_identity_response_schema import GetIdentityResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2GetIdentityResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2GetIdentityResponseSchema]
+class GetIdentityResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[GetIdentityResponseSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_get_identity_response_schema.py` & `polytomic-0.1.2/src/polytomic/types/webhook.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2GetIdentityResponseSchema(pydantic.BaseModel):
-    email: typing.Optional[str]
-    id: typing.Optional[str]
-    is_organization: typing.Optional[bool]
-    is_partner: typing.Optional[bool]
-    is_system: typing.Optional[bool]
-    is_user: typing.Optional[bool]
-    organization_id: typing.Optional[str]
-    organization_name: typing.Optional[str]
-    role: typing.Optional[str]
+class Webhook(pydantic.BaseModel):
+    created_at: typing.Optional[dt.datetime] = None
+    endpoint: typing.Optional[str] = None
+    id: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    secret: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_identity.py` & `polytomic-0.1.2/src/polytomic/types/list_execution_response_envelope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_source import V2Source
+from .get_execution_response_schema import GetExecutionResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Identity(pydantic.BaseModel):
-    function: str
-    new_field: typing.Optional[bool]
-    remote_field_type_id: typing.Optional[str]
-    source: V2Source
-    target: str
+class ListExecutionResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[GetExecutionResponseSchema]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_identity_function.py` & `polytomic-0.1.2/src/polytomic/types/relation_to.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2IdentityFunction(pydantic.BaseModel):
-    id: typing.Optional[str]
-    label: typing.Optional[str]
+class RelationTo(pydantic.BaseModel):
+    field: typing.Optional[str] = None
+    model_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_list_execution_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/list_bulk_sync_executions_envelope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_get_execution_response_schema import V2GetExecutionResponseSchema
+from .bulk_sync_execution import BulkSyncExecution
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ListExecutionResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2GetExecutionResponseSchema]]
+class ListBulkSyncExecutionsEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[BulkSyncExecution]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_list_policies_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/execution_log_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_policy_response import V2PolicyResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ListPoliciesResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2PolicyResponse]]
+class ExecutionLogResponse(pydantic.BaseModel):
+    expires: typing.Optional[dt.datetime] = None
+    urls: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_list_sync_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/activate_sync_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_sync_response import V2SyncResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ListSyncResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2SyncResponse]]
+class ActivateSyncInput(pydantic.BaseModel):
+    active: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_list_users_envelope.py` & `polytomic-0.1.2/src/polytomic/types/schema_records_response_envelope.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_user import V2User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ListUsersEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2User]]
+class SchemaRecordsResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_mode.py` & `polytomic-0.1.2/src/polytomic/types/bulk_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .bulk_field import BulkField
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Mode(pydantic.BaseModel):
-    description: typing.Optional[str]
-    label: typing.Optional[str]
-    mode: typing.Optional[str]
-    requires_identity: typing.Optional[bool]
-    supports_field_sync_mode: typing.Optional[bool]
-    supports_target_filters: typing.Optional[bool]
+class BulkSchema(pydantic.BaseModel):
+    enabled: typing.Optional[bool] = None
+    fields: typing.Optional[typing.List[BulkField]] = None
+    id: typing.Optional[str] = None
+    output_name: typing.Optional[str] = None
+    partition_key: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_model_field.py` & `polytomic-0.1.2/src/polytomic/types/schema_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .pick_value import PickValue
+from .schema_association import SchemaAssociation
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ModelField(pydantic.BaseModel):
-    description: typing.Optional[str]
-    example: typing.Optional[typing.Any]
-    label: typing.Optional[str]
-    name: typing.Optional[str]
-    remote_type: typing.Optional[str]
-    type: typing.Optional[str]
-    unique: typing.Optional[bool]
-    user_added: typing.Optional[bool]
+class SchemaField(pydantic.BaseModel):
+    association: typing.Optional[SchemaAssociation] = None
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    remote_type: typing.Optional[str] = None
+    type: typing.Optional[str] = None
+    values: typing.Optional[typing.List[PickValue]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_model_field_request.py` & `polytomic-0.1.2/src/polytomic/types/job_response_envelope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .job_response import JobResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ModelFieldRequest(pydantic.BaseModel):
-    example: typing.Optional[str]
-    label: str
-    name: str
-    type: str
+class JobResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[JobResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_model_field_response.py` & `polytomic-0.1.2/src/polytomic/types/list_users_envelope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_model_field import V2ModelField
+from .user import User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ModelFieldResponse(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2ModelField]]
+class ListUsersEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[User]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_model_list_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/execution_logs_response_envelope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_model_response import V2ModelResponse
+from .execution_log_response import ExecutionLogResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ModelListResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2ModelResponse]]
+class ExecutionLogsResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ExecutionLogResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_model_response.py` & `polytomic-0.1.2/src/polytomic/types/model_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .label_label import LabelLabel
-from .v_2_model_field import V2ModelField
-from .v_2_relation import V2Relation
+from .model_field import ModelField
+from .relation import Relation
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ModelResponse(pydantic.BaseModel):
-    configuration: typing.Optional[typing.Dict[str, typing.Any]]
-    connection_id: typing.Optional[str]
-    fields: typing.Optional[typing.List[V2ModelField]]
-    id: typing.Optional[str]
-    identifier: typing.Optional[str]
-    labels: typing.Optional[typing.List[LabelLabel]]
-    name: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    policies: typing.Optional[typing.List[str]]
-    relations: typing.Optional[typing.List[V2Relation]]
-    tracking_columns: typing.Optional[typing.List[str]]
-    type: typing.Optional[str]
-    version: typing.Optional[int]
+class ModelResponse(pydantic.BaseModel):
+    configuration: typing.Optional[typing.Dict[str, typing.Any]] = None
+    connection_id: typing.Optional[str] = None
+    fields: typing.Optional[typing.List[ModelField]] = None
+    id: typing.Optional[str] = None
+    identifier: typing.Optional[str] = None
+    labels: typing.Optional[typing.List[LabelLabel]] = None
+    name: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    policies: typing.Optional[typing.List[str]] = None
+    relations: typing.Optional[typing.List[Relation]] = None
+    tracking_columns: typing.Optional[typing.List[str]] = None
+    type: typing.Optional[str] = None
+    version: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_model_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/model_list_response_envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_model_response import V2ModelResponse
+from .model_response import ModelResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2ModelResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2ModelResponse]
+class ModelListResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ModelResponse]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_organization.py` & `polytomic-0.1.2/src/polytomic/types/bulk_field.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Organization(pydantic.BaseModel):
-    id: typing.Optional[str]
-    issuer: typing.Optional[str]
-    name: typing.Optional[str]
-    sso_domain: typing.Optional[str]
-    sso_org_id: typing.Optional[str]
+class BulkField(pydantic.BaseModel):
+    enabled: typing.Optional[bool] = None
+    id: typing.Optional[str] = None
+    obfuscated: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_organization_envelope.py` & `polytomic-0.1.2/src/polytomic/types/organization_envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_organization import V2Organization
+from .organization import Organization
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2OrganizationEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2Organization]
+class OrganizationEnvelope(pydantic.BaseModel):
+    data: typing.Optional[Organization] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_organizations_envelope.py` & `polytomic-0.1.2/src/polytomic/types/run_after.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_organization import V2Organization
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2OrganizationsEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2Organization]]
+class RunAfter(pydantic.BaseModel):
+    bulk_sync_ids: typing.Optional[typing.List[str]] = None
+    sync_ids: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_override.py` & `polytomic-0.1.2/src/polytomic/types/model_model_field_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Override(pydantic.BaseModel):
-    field_id: typing.Optional[str]
-    function: typing.Optional[str]
-    override: typing.Optional[typing.Any]
-    value: typing.Optional[typing.Any]
+class ModelModelFieldRequest(pydantic.BaseModel):
+    example: typing.Optional[str] = None
+    label: str
+    name: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_policy_action.py` & `polytomic-0.1.2/src/polytomic/types/identity_function.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2PolicyAction(pydantic.BaseModel):
-    action: str
-    role_ids: typing.Optional[typing.List[str]]
+class IdentityFunction(pydantic.BaseModel):
+    id: typing.Optional[str] = None
+    label: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_policy_response.py` & `polytomic-0.1.2/src/polytomic/types/connection_response_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_policy_action import V2PolicyAction
+from .connection_type_schema import ConnectionTypeSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2PolicyResponse(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    policy_actions: typing.Optional[typing.List[V2PolicyAction]]
-    system: typing.Optional[bool]
+class ConnectionResponseSchema(pydantic.BaseModel):
+    configuration: typing.Optional[typing.Dict[str, typing.Any]] = None
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    policies: typing.Optional[typing.List[str]] = None
+    status: typing.Optional[str] = None
+    status_error: typing.Optional[str] = None
+    type: typing.Optional[ConnectionTypeSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_policy_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_policy_response import V2PolicyResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2PolicyResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2PolicyResponse]
+class BulkSyncSourceStatus(pydantic.BaseModel):
+    cache_status: typing.Optional[str] = None
+    last_refresh_finished: typing.Optional[dt.datetime] = None
+    last_refresh_started: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_relation.py` & `polytomic-0.1.2/src/polytomic/types/relation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_relation_to import V2RelationTo
+from .relation_to import RelationTo
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Relation(pydantic.BaseModel):
-    from_: typing.Optional[str] = pydantic.Field(alias="from")
-    to: typing.Optional[V2RelationTo]
+class Relation(pydantic.BaseModel):
+    from_: typing.Optional[str] = pydantic.Field(alias="from", default=None)
+    to: typing.Optional[RelationTo] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_relation_to.py` & `polytomic-0.1.2/src/polytomic/types/list_bulk_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .bulk_schema import BulkSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2RelationTo(pydantic.BaseModel):
-    field: typing.Optional[str]
-    model_id: typing.Optional[str]
+class ListBulkSchema(pydantic.BaseModel):
+    data: typing.Optional[typing.List[BulkSchema]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_role_list_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/schedule_option_response_envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_role_response import V2RoleResponse
+from .schedule_option_response import ScheduleOptionResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2RoleListResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2RoleResponse]]
+class ScheduleOptionResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ScheduleOptionResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_role_response.py` & `polytomic-0.1.2/src/polytomic/types/webhook_list_envelope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .webhook import Webhook
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2RoleResponse(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    system: typing.Optional[bool]
+class WebhookListEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[Webhook]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_role_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_status_envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_role_response import V2RoleResponse
+from .bulk_sync_status_response import BulkSyncStatusResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2RoleResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2RoleResponse]
+class BulkSyncStatusEnvelope(pydantic.BaseModel):
+    data: typing.Optional[BulkSyncStatusResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_run_after.py` & `polytomic-0.1.2/src/polytomic/types/events_envelope.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .event import Event
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2RunAfter(pydantic.BaseModel):
-    bulk_sync_ids: typing.Optional[typing.List[str]]
-    sync_ids: typing.Optional[typing.List[str]]
+class EventsEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[Event]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_schedule.py` & `polytomic-0.1.2/src/polytomic/types/job_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_run_after import V2RunAfter
+from .work_task_status import WorkTaskStatus
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Schedule(pydantic.BaseModel):
-    day_of_month: typing.Optional[str]
-    day_of_week: typing.Optional[str]
-    frequency: typing.Optional[str]
-    hour: typing.Optional[str]
-    minute: typing.Optional[str]
-    month: typing.Optional[str]
-    run_after: typing.Optional[V2RunAfter]
+class JobResponse(pydantic.BaseModel):
+    error: typing.Optional[str] = None
+    job_id: typing.Optional[str] = None
+    result: typing.Optional[typing.Any] = None
+    status: typing.Optional[WorkTaskStatus] = None
+    type: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_source.py` & `polytomic-0.1.2/src/polytomic/types/connection_parameter_values_response_envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .connection_parameter_values_resp import ConnectionParameterValuesResp
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Source(pydantic.BaseModel):
-    field: str
-    model_id: str
+class ConnectionParameterValuesResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.Dict[str, typing.Optional[ConnectionParameterValuesResp]]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_start_sync_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/list_model_sync_response_envelope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_start_sync_response_schema import V2StartSyncResponseSchema
+from .model_sync_response import ModelSyncResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2StartSyncResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2StartSyncResponseSchema]
+class ListModelSyncResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[ModelSyncResponse]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_start_sync_response_schema.py` & `polytomic-0.1.2/src/polytomic/types/configuration_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2StartSyncResponseSchema(pydantic.BaseModel):
-    created_at: typing.Optional[dt.datetime]
-    id: typing.Optional[str]
-    status: typing.Optional[str]
+class ConfigurationValue(pydantic.BaseModel):
+    items: typing.Optional[typing.List[typing.Any]] = None
+    type: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_supported_mode.py` & `polytomic-0.1.2/src/polytomic/types/mode.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2SupportedMode(pydantic.BaseModel):
-    description: typing.Optional[str]
-    id: typing.Optional[str] = pydantic.Field(description="")
-    label: typing.Optional[str]
-    requires_identity: typing.Optional[bool]
-    supports_field_sync_mode: typing.Optional[bool]
-    supports_target_filters: typing.Optional[bool]
+class Mode(pydantic.BaseModel):
+    description: typing.Optional[str] = None
+    label: typing.Optional[str] = None
+    mode: typing.Optional[str] = None
+    requires_identity: typing.Optional[bool] = None
+    supports_field_sync_mode: typing.Optional[bool] = None
+    supports_target_filters: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_sync_field.py` & `polytomic-0.1.2/src/polytomic/types/start_model_sync_response_envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_source import V2Source
+from .start_model_sync_response_schema import StartModelSyncResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2SyncField(pydantic.BaseModel):
-    new: typing.Optional[bool]
-    override_value: typing.Optional[str]
-    source: V2Source
-    sync_mode: typing.Optional[str]
-    target: str
+class StartModelSyncResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[StartModelSyncResponseSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_sync_response.py` & `polytomic-0.1.2/src/polytomic/types/target_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,37 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_filter import V2Filter
-from .v_2_identity import V2Identity
-from .v_2_override import V2Override
-from .v_2_schedule import V2Schedule
-from .v_2_sync_field import V2SyncField
-from .v_2_target import V2Target
+from .mode import Mode
+from .sync_destination_properties import SyncDestinationProperties
+from .target_field import TargetField
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2SyncResponse(pydantic.BaseModel):
-    active: typing.Optional[bool]
-    fields: typing.Optional[typing.List[V2SyncField]]
-    filter_logic: typing.Optional[str]
-    filters: typing.Optional[typing.List[V2Filter]]
-    id: typing.Optional[str]
-    identity: typing.Optional[V2Identity]
-    mode: typing.Optional[str]
-    name: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    override_fields: typing.Optional[typing.List[V2SyncField]]
-    overrides: typing.Optional[typing.List[V2Override]]
-    policies: typing.Optional[typing.List[str]]
-    schedule: typing.Optional[V2Schedule]
-    sync_all_records: typing.Optional[bool]
-    target: typing.Optional[V2Target]
+class TargetResponse(pydantic.BaseModel):
+    fields: typing.Optional[typing.List[TargetField]] = None
+    id: typing.Optional[str] = None
+    modes: typing.Optional[typing.List[Mode]] = None
+    name: typing.Optional[str] = None
+    properties: typing.Optional[SyncDestinationProperties] = None
+    refreshed_at: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_sync_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_list_envelope.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_sync_response import V2SyncResponse
+from .bulk_sync_response import BulkSyncResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2SyncResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2SyncResponse]
+class BulkSyncListEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[BulkSyncResponse]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_sync_status_envelope.py` & `polytomic-0.1.2/src/polytomic/types/sync_status_envelope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_sync_status_response import V2SyncStatusResponse
+from .sync_status_response import SyncStatusResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2SyncStatusEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2SyncStatusResponse]
+class SyncStatusEnvelope(pydantic.BaseModel):
+    data: typing.Optional[SyncStatusResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_sync_status_response.py` & `polytomic-0.1.2/src/polytomic/types/sync_status_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_get_execution_response_schema import V2GetExecutionResponseSchema
+from .get_execution_response_schema import GetExecutionResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2SyncStatusResponse(pydantic.BaseModel):
-    current_execution: typing.Optional[V2GetExecutionResponseSchema]
-    last_execution: typing.Optional[V2GetExecutionResponseSchema]
-    next_execution_time: typing.Optional[dt.datetime]
+class SyncStatusResponse(pydantic.BaseModel):
+    current_execution: typing.Optional[GetExecutionResponseSchema] = None
+    last_execution: typing.Optional[GetExecutionResponseSchema] = None
+    next_execution_time: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_target.py` & `polytomic-0.1.2/src/polytomic/types/user_envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .user import User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Target(pydantic.BaseModel):
-    configuration: typing.Optional[typing.Dict[str, typing.Any]]
-    connection_id: str
-    filter_logic: typing.Optional[str]
-    new_name: typing.Optional[str]
-    object: str
-    search_values: typing.Optional[typing.Dict[str, typing.Any]]
+class UserEnvelope(pydantic.BaseModel):
+    data: typing.Optional[User] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_target_field.py` & `polytomic-0.1.2/src/polytomic/types/organization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_identity_function import V2IdentityFunction
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2TargetField(pydantic.BaseModel):
-    association: typing.Optional[bool]
-    createable: typing.Optional[bool]
-    description: typing.Optional[str]
-    filterable: typing.Optional[bool]
-    id: typing.Optional[str]
-    identity_functions: typing.Optional[typing.List[V2IdentityFunction]]
-    name: typing.Optional[str]
-    required: typing.Optional[bool]
-    source_type: typing.Optional[str]
-    supports_identity: typing.Optional[bool]
-    type: typing.Optional[str]
-    updateable: typing.Optional[bool]
+class Organization(pydantic.BaseModel):
+    id: typing.Optional[str] = None
+    issuer: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    sso_domain: typing.Optional[str] = None
+    sso_org_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_target_response.py` & `polytomic-0.1.2/src/polytomic/types/start_model_sync_response_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .sync_destination_properties import SyncDestinationProperties
-from .v_2_mode import V2Mode
-from .v_2_target_field import V2TargetField
+from .execution_status import ExecutionStatus
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2TargetResponse(pydantic.BaseModel):
-    fields: typing.Optional[typing.List[V2TargetField]]
-    id: typing.Optional[str]
-    modes: typing.Optional[typing.List[V2Mode]]
-    name: typing.Optional[str]
-    properties: typing.Optional[SyncDestinationProperties]
-    refreshed_at: typing.Optional[dt.datetime]
+class StartModelSyncResponseSchema(pydantic.BaseModel):
+    created_at: typing.Optional[dt.datetime] = None
+    id: typing.Optional[str] = None
+    status: typing.Optional[ExecutionStatus] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_target_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/target_response_envelope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_target_response import V2TargetResponse
+from .target_response import TargetResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2TargetResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2TargetResponse]
+class TargetResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[TargetResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_user.py` & `polytomic-0.1.2/src/polytomic/types/bulk_schema_envelope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .bulk_schema import BulkSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2User(pydantic.BaseModel):
-    email: typing.Optional[str]
-    id: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    role: typing.Optional[str]
+class BulkSchemaEnvelope(pydantic.BaseModel):
+    data: typing.Optional[BulkSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_user_envelope.py` & `polytomic-0.1.2/src/polytomic/types/filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_user import V2User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2UserEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2User]
+class Filter(pydantic.BaseModel):
+    field_id: str
+    field_type: str
+    function: str
+    label: typing.Optional[str] = None
+    value: typing.Optional[typing.Any] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_webhook.py` & `polytomic-0.1.2/src/polytomic/types/model_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2Webhook(pydantic.BaseModel):
-    created_at: typing.Optional[dt.datetime]
-    endpoint: typing.Optional[str]
-    id: typing.Optional[str]
-    organization_id: typing.Optional[str]
-    secret: typing.Optional[str]
+class ModelField(pydantic.BaseModel):
+    description: typing.Optional[str] = None
+    example: typing.Optional[typing.Any] = None
+    label: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    remote_type: typing.Optional[str] = None
+    type: typing.Optional[str] = None
+    unique: typing.Optional[bool] = None
+    user_added: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_webhook_envelope.py` & `polytomic-0.1.2/src/polytomic/types/schema_association.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_webhook import V2Webhook
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2WebhookEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V2Webhook]
+class SchemaAssociation(pydantic.BaseModel):
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    reference_to: typing.Optional[typing.List[str]] = None
+    referenced_field: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_2_webhook_list_envelope.py` & `polytomic-0.1.2/src/polytomic/types/activate_sync_envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_2_webhook import V2Webhook
+from .activate_sync_output import ActivateSyncOutput
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V2WebhookListEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V2Webhook]]
+class ActivateSyncEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ActivateSyncOutput] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_field.py` & `polytomic-0.1.2/src/polytomic/types/connect_card_response_envelope.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .connect_card_response import ConnectCardResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkField(pydantic.BaseModel):
-    enabled: typing.Optional[bool]
-    id: typing.Optional[str]
-    obfuscated: typing.Optional[bool]
+class ConnectCardResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ConnectCardResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_schema.py` & `polytomic-0.1.2/src/polytomic/types/activate_sync_output.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_field import V3BulkField
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSchema(pydantic.BaseModel):
-    enabled: typing.Optional[bool]
-    fields: typing.Optional[typing.List[V3BulkField]]
-    id: typing.Optional[str]
-    partition_key: typing.Optional[str]
+class ActivateSyncOutput(pydantic.BaseModel):
+    active: typing.Optional[bool] = None
+    id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_schema_envelope.py` & `polytomic-0.1.2/src/polytomic/types/role_list_response_envelope.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_schema import V3BulkSchema
+from .role_response import RoleResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSchemaEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V3BulkSchema]
+class RoleListResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[RoleResponse]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_execution.py` & `polytomic-0.1.2/src/polytomic/types/connection_meta_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_sync_schema_execution import V3BulkSyncSchemaExecution
+from .configuration_value import ConfigurationValue
+from .connection_meta import ConnectionMeta
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncExecution(pydantic.BaseModel):
-    completed_at: typing.Optional[dt.datetime]
-    created_at: typing.Optional[dt.datetime]
-    id: typing.Optional[str]
-    is_resync: typing.Optional[bool]
-    is_test: typing.Optional[bool]
-    schemas: typing.Optional[typing.List[V3BulkSyncSchemaExecution]]
-    started_at: typing.Optional[dt.datetime]
-    status: typing.Optional[str]
-    type: typing.Optional[str]
+class ConnectionMetaResponse(pydantic.BaseModel):
+    configuration: typing.Optional[typing.Dict[str, ConfigurationValue]] = None
+    items: typing.Optional[typing.Dict[str, typing.Optional[ConnectionMeta]]] = None
+    requires_one_of: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_execution_envelope.py` & `polytomic-0.1.2/src/polytomic/types/connection_response_envelope.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_sync_execution import V3BulkSyncExecution
+from .connection_response_schema import ConnectionResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncExecutionEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V3BulkSyncExecution]
+class ConnectionResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ConnectionResponseSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_schema_execution.py` & `polytomic-0.1.2/src/polytomic/types/model_response_envelope.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .job_response import JobResponse
+from .model_response import ModelResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncSchemaExecution(pydantic.BaseModel):
-    completed_at: typing.Optional[dt.datetime]
-    error_count: typing.Optional[int]
-    record_count: typing.Optional[int]
-    schema_: typing.Optional[str] = pydantic.Field(alias="schema")
-    started_at: typing.Optional[dt.datetime]
-    status: typing.Optional[str]
-    status_message: typing.Optional[str]
+class ModelResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[ModelResponse] = None
+    job: typing.Optional[JobResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source.py` & `polytomic-0.1.2/src/polytomic/types/list_policies_response_envelope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_schema import V3Schema
+from .policy_response import PolicyResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncSource(pydantic.BaseModel):
-    configuration: typing.Optional[typing.Any]
-    schemas: typing.Optional[typing.List[V3Schema]]
+class ListPoliciesResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[typing.List[PolicyResponse]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_envelope.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_envelope.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_sync_source import V3BulkSyncSource
+from .bulk_sync_source import BulkSyncSource
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncSourceEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V3BulkSyncSource]
+class BulkSyncSourceEnvelope(pydantic.BaseModel):
+    data: typing.Optional[BulkSyncSource] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_schema_envelope.py` & `polytomic-0.1.2/src/polytomic/types/role_response_envelope.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_schema import V3Schema
+from .role_response import RoleResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncSourceSchemaEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V3Schema]
+class RoleResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[RoleResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_status.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_dest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .supported_mode import SupportedMode
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncSourceStatus(pydantic.BaseModel):
-    cache_status: typing.Optional[str]
-    last_refresh_finished: typing.Optional[dt.datetime]
-    last_refresh_started: typing.Optional[dt.datetime]
+class BulkSyncDest(pydantic.BaseModel):
+    configuration: typing.Optional[typing.Dict[str, typing.Any]] = None
+    modes: typing.Optional[typing.List[SupportedMode]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_source_status_envelope.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_source_status_envelope.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_sync_source_status import V3BulkSyncSourceStatus
+from .bulk_sync_source_status import BulkSyncSourceStatus
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncSourceStatusEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V3BulkSyncSourceStatus]
+class BulkSyncSourceStatusEnvelope(pydantic.BaseModel):
+    data: typing.Optional[BulkSyncSourceStatus] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_status_envelope.py` & `polytomic-0.1.2/src/polytomic/types/create_connection_response_envelope.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_sync_status_response import V3BulkSyncStatusResponse
+from .create_connection_response_schema import CreateConnectionResponseSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncStatusEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V3BulkSyncStatusResponse]
+class CreateConnectionResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[CreateConnectionResponseSchema] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_bulk_sync_status_response.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_status_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_sync_execution import V3BulkSyncExecution
+from .bulk_sync_execution import BulkSyncExecution
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3BulkSyncStatusResponse(pydantic.BaseModel):
-    current_execution: typing.Optional[V3BulkSyncExecution]
-    last_execution: typing.Optional[V3BulkSyncExecution]
-    next_execution_time: typing.Optional[dt.datetime]
+class BulkSyncStatusResponse(pydantic.BaseModel):
+    current_execution: typing.Optional[BulkSyncExecution] = None
+    last_execution: typing.Optional[BulkSyncExecution] = None
+    next_execution_time: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_connect_card_response.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_execution_envelope.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .bulk_sync_execution import BulkSyncExecution
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3ConnectCardResponse(pydantic.BaseModel):
-    redirect_url: typing.Optional[str]
-    token: typing.Optional[str]
+class BulkSyncExecutionEnvelope(pydantic.BaseModel):
+    data: typing.Optional[BulkSyncExecution] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_connect_card_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/schedule_option_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_connect_card_response import V3ConnectCardResponse
+from .schedule_schedule_option import ScheduleScheduleOption
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3ConnectCardResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[V3ConnectCardResponse]
+class ScheduleOptionResponse(pydantic.BaseModel):
+    schedule_options: typing.Optional[typing.List[ScheduleScheduleOption]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_list_bulk_schema_envelope.py` & `polytomic-0.1.2/src/polytomic/types/event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_schema import V3BulkSchema
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3ListBulkSchemaEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V3BulkSchema]]
+class Event(pydantic.BaseModel):
+    created_at: typing.Optional[dt.datetime] = None
+    event: typing.Optional[typing.Any] = None
+    id: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    type: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_list_bulk_sync_executions_envelope.py` & `polytomic-0.1.2/src/polytomic/types/policy_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_bulk_sync_execution import V3BulkSyncExecution
+from .policy_action import PolicyAction
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3ListBulkSyncExecutionsEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[V3BulkSyncExecution]]
+class PolicyResponse(pydantic.BaseModel):
+    id: typing.Optional[str] = None
+    name: typing.Optional[str] = None
+    organization_id: typing.Optional[str] = None
+    policy_actions: typing.Optional[typing.List[PolicyAction]] = None
+    system: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_pick_value.py` & `polytomic-0.1.2/src/polytomic/types/target.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3PickValue(pydantic.BaseModel):
-    label: typing.Optional[str]
-    value: typing.Optional[str]
+class Target(pydantic.BaseModel):
+    configuration: typing.Optional[typing.Dict[str, typing.Any]] = None
+    connection_id: str
+    filter_logic: typing.Optional[str] = None
+    new_name: typing.Optional[str] = None
+    object: str
+    search_values: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_schema.py` & `polytomic-0.1.2/src/polytomic/types/schedule_schedule_option.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .v_3_schema_field import V3SchemaField
+from .jsonschema_form import JsonschemaForm
+from .schedule_frequency import ScheduleFrequency
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3Schema(pydantic.BaseModel):
-    fields: typing.Optional[typing.List[V3SchemaField]]
-    id: typing.Optional[str]
-    name: typing.Optional[str]
+class ScheduleScheduleOption(pydantic.BaseModel):
+    configuration: typing.Optional[JsonschemaForm] = None
+    description: typing.Optional[str] = None
+    frequency: typing.Optional[ScheduleFrequency] = None
+    label: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_schema_field.py` & `polytomic-0.1.2/src/polytomic/types/bulk_sync_execution.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .schema_association import SchemaAssociation
-from .v_3_pick_value import V3PickValue
+from .bulk_execution_status import BulkExecutionStatus
+from .bulk_sync_schema_execution import BulkSyncSchemaExecution
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3SchemaField(pydantic.BaseModel):
-    association: typing.Optional[SchemaAssociation]
-    id: typing.Optional[str]
-    name: typing.Optional[str]
-    remote_type: typing.Optional[str]
-    type: typing.Optional[str]
-    values: typing.Optional[typing.List[V3PickValue]]
+class BulkSyncExecution(pydantic.BaseModel):
+    completed_at: typing.Optional[dt.datetime] = None
+    created_at: typing.Optional[dt.datetime] = None
+    id: typing.Optional[str] = None
+    is_resync: typing.Optional[bool] = None
+    is_test: typing.Optional[bool] = None
+    schemas: typing.Optional[typing.List[BulkSyncSchemaExecution]] = None
+    started_at: typing.Optional[dt.datetime] = None
+    status: typing.Optional[BulkExecutionStatus] = None
+    type: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/src/polytomic/types/v_3_schema_records_response_envelope.py` & `polytomic-0.1.2/src/polytomic/types/policy_response_envelope.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-# This file was auto-generated by Fern from our API Definition.
+# This file was auto-generated from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .policy_response import PolicyResponse
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class V3SchemaRecordsResponseEnvelope(pydantic.BaseModel):
-    data: typing.Optional[typing.List[typing.Dict[str, typing.Any]]]
+class PolicyResponseEnvelope(pydantic.BaseModel):
+    data: typing.Optional[PolicyResponse] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `polytomic-0.1.0/PKG-INFO` & `polytomic-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: polytomic
-Version: 0.1.0
+Version: 0.1.2
 Summary: 
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.21.2)
-Requires-Dist: pydantic (>=1.9.2,<2.5.0)
+Requires-Dist: pydantic (>=1.9.2)
+Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 <!-- Begin Title, generated by Fern  -->
 # Polytomic Python Library
 
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
 
@@ -32,28 +32,28 @@
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
 ```python
 from polytomic.client import Polytomic
 
 client = Polytomic(
-    polytomic_version="YOUR_POLYTOMIC_VERSION",
+    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 ```python
 from polytomic.client import AsyncPolytomic
 
 client = AsyncPolytomic(
-    polytomic_version="YOUR_POLYTOMIC_VERSION",
+    x_polytomic_version="YOUR_X_POLYTOMIC_VERSION",
     token="YOUR_TOKEN",
 )
 ```
 <!-- End Async Usage  -->
 
 <!-- Begin Status, generated by Fern  -->
 # Beta Status
```

