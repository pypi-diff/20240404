# Comparing `tmp/dropbox-sign-1.3.0.tar.gz` & `tmp/dropbox-sign-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dropbox-sign-1.3.0.tar", last modified: Mon Jan 29 21:59:57 2024, max compression
+gzip compressed data, was "dropbox-sign-1.4.0.tar", last modified: Wed Apr  3 22:48:47 2024, max compression
```

## Comparing `dropbox-sign-1.3.0.tar` & `dropbox-sign-1.4.0.tar`

### file list

```diff
@@ -1,230 +1,234 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.660913 dropbox-sign-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-01-29 21:59:46.000000 dropbox-sign-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25349 2024-01-29 21:59:57.660913 dropbox-sign-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-01-29 21:59:46.000000 dropbox-sign-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.620913 dropbox-sign-1.3.0/dropbox_sign/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.624913 dropbox-sign-1.3.0/dropbox_sign/api/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24601 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29481 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/api_app_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/bulk_send_job_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/embedded_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/o_auth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/report_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   104099 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/signature_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    58636 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/team_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    69908 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/template_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27983 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api/unclaimed_draft_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39926 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.624913 dropbox-sign-1.3.0/dropbox_sign/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17158 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/event_callback_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.656913 dropbox-sign-1.3.0/dropbox_sign/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17077 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_response_quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_verify_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_verify_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/account_verify_response_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15768 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_owner_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_white_labeling_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    15674 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/api_app_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    30888 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_get_response_signature_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    13772 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_send_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/embedded_edit_url_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/embedded_edit_url_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/embedded_edit_url_response_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/embedded_sign_url_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/embedded_sign_url_response_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12913 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/error_response_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/event_callback_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/event_callback_request_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/event_callback_request_event_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/file_response_data_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/list_info_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14284 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/o_auth_token_generate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/o_auth_token_refresh_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13630 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/o_auth_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/report_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/report_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/report_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24637 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_bulk_create_embedded_with_template_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    24607 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_bulk_send_with_template_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    35921 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_create_embedded_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    23851 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_create_embedded_with_template_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13850 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_remind_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14441 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    16333 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    16730 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_checkbox_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_date_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    16639 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_initials.py
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    16593 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    16692 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_text_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    22495 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    37768 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_send_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_send_with_template_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/signature_request_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13686 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_bulk_signer_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_bulk_signer_list_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_editor_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_field_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_rule_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_rule_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    19870 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_checkbox_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_date_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)    22681 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_font_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    22389 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_hyperlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_initials.py
--rw-r--r--   0 runner    (1001) docker     (127)    20711 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    19738 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    27854 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    21759 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_text_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_merge_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_signature_request_grouped_signers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15435 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_signature_request_signer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15476 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_signature_request_template_signer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_signing_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_team_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_template_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_unclaimed_draft_signer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_unclaimed_draft_template_signer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21130 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/sub_white_labeling_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_add_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12814 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_get_info_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_info_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_invite_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_invites_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_member_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_members_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_parent_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_remove_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_sub_teams_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/team_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_add_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    34476 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_create_embedded_draft_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_create_embedded_draft_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_create_embedded_draft_response_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    28864 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_create_response_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_edit_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_remove_user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    24253 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_account_quota.py
--rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_cc_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    12435 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    16900 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    20643 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    16468 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    21458 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_field_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_field_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    19217 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_date_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    22170 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_hyperlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_initials.py
--rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_date_signed.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_dropdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_hyperlink.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_initials.py
--rw-r--r--   0 runner    (1001) docker     (127)    19791 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_field_avg_text_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_named_form_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    12356 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_response_signer_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_update_files_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_update_files_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/template_update_files_response_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    47111 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_embedded_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    37337 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_embedded_with_template_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    36686 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17571 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_edit_and_resend_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12457 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model/warning_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    81874 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.656913 dropbox-sign-1.3.0/dropbox_sign/models/
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/dropbox_sign/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.660913 dropbox-sign-1.3.0/dropbox_sign.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25349 2024-01-29 21:59:57.000000 dropbox-sign-1.3.0/dropbox_sign.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-01-29 21:59:57.000000 dropbox-sign-1.3.0/dropbox_sign.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 21:59:57.000000 dropbox-sign-1.3.0/dropbox_sign.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-29 21:59:57.000000 dropbox-sign-1.3.0/dropbox_sign.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-29 21:59:57.000000 dropbox-sign-1.3.0/dropbox_sign.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-29 21:59:57.660913 dropbox-sign-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:59:57.660913 dropbox-sign-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_api_app_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_bulk_send_job_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_embedded_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_event_callback_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_model_signature_request_send_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_oauth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_report_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_signature_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_sub_form_fields_per_document_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_team_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_template_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_unclaimed_draft_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-29 21:59:47.000000 dropbox-sign-1.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.567309 dropbox-sign-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26677 2024-04-03 22:48:47.567309 dropbox-sign-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26252 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.523309 dropbox-sign-1.4.0/dropbox_sign/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.527309 dropbox-sign-1.4.0/dropbox_sign/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24601 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29481 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/api_app_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/bulk_send_job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/embedded_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/o_auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/report_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132125 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/signature_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58636 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/team_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69908 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/template_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27983 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api/unclaimed_draft_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39926 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.527309 dropbox-sign-1.4.0/dropbox_sign/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17158 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/event_callback_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.563309 dropbox-sign-1.4.0/dropbox_sign/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14240 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17077 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_response_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_verify_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/account_verify_response_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15768 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12812 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_owner_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_white_labeling_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15674 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/api_app_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31494 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_get_response_signature_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13772 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_send_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19704 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/embedded_edit_url_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/embedded_edit_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/embedded_edit_url_response_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/embedded_sign_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/embedded_sign_url_response_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12913 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/error_response_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/event_callback_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15656 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/event_callback_request_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/event_callback_request_event_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/file_response_data_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/list_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14284 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/o_auth_token_generate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12858 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/o_auth_token_refresh_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13630 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/o_auth_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/report_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/report_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25417 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_bulk_create_embedded_with_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25387 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_bulk_send_with_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35921 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_create_embedded_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23851 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_create_embedded_with_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35911 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_edit_embedded_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23841 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_edit_embedded_with_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37768 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_edit_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_edit_with_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13850 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_remind_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29401 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14441 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16333 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16730 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_checkbox_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_date_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16639 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_initials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16593 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16692 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_text_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22495 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37768 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_send_with_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/signature_request_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13686 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_bulk_signer_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_bulk_signer_list_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12872 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_editor_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_field_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15028 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_rule_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_rule_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20694 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19870 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_checkbox_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21772 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_date_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22791 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_font_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22499 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_hyperlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_initials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20711 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19738 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21869 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_text_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_merge_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_signature_request_grouped_signers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_signature_request_signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16248 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_signature_request_template_signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_signing_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_team_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_template_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_unclaimed_draft_signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_unclaimed_draft_template_signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21130 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/sub_white_labeling_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_add_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12814 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_get_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13963 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_invite_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_invites_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_member_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_members_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_parent_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_remove_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13549 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_sub_teams_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/team_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_add_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34476 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_create_embedded_draft_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_create_embedded_draft_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_create_embedded_draft_response_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28864 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_create_response_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_edit_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_remove_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24253 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_account_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_cc_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12435 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16900 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20643 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16468 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21458 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_field_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_field_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19217 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19680 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_date_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22170 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_hyperlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19658 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_initials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23608 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18460 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_date_signed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_hyperlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_initials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19791 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_field_avg_text_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14377 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_named_form_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12356 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_response_signer_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_update_files_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_update_files_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/template_update_files_response_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47111 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_embedded_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37337 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_embedded_with_template_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36686 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17571 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_edit_and_resend_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12457 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model/warning_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81874 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.563309 dropbox-sign-1.4.0/dropbox_sign/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/dropbox_sign/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.567309 dropbox-sign-1.4.0/dropbox_sign.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26677 2024-04-03 22:48:47.000000 dropbox-sign-1.4.0/dropbox_sign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-04-03 22:48:47.000000 dropbox-sign-1.4.0/dropbox_sign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:48:47.000000 dropbox-sign-1.4.0/dropbox_sign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 22:48:47.000000 dropbox-sign-1.4.0/dropbox_sign.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 22:48:47.000000 dropbox-sign-1.4.0/dropbox_sign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 22:48:47.567309 dropbox-sign-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:48:47.567309 dropbox-sign-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_api_app_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_bulk_send_job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_embedded_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_event_callback_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_model_signature_request_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_oauth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_signature_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_sub_form_fields_per_document_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_team_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_template_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_unclaimed_draft_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-03 22:48:44.000000 dropbox-sign-1.4.0/tests/test_utils.py
```

### Comparing `dropbox-sign-1.3.0/LICENSE` & `dropbox-sign-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/PKG-INFO` & `dropbox-sign-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropbox-sign
-Version: 1.3.0
+Version: 1.4.0
 Summary: Dropbox Sign API
 Home-page: https://github.com/hellosign/dropbox-sign-python
 Author: Dropbox Sign API Team
 Author-email: apisupport@hellosign.com
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Dropbox Sign API
 Requires-Python: >=3.7
@@ -61,15 +61,15 @@
 Python >=3.7
 
 ### pip
 
 Install using `pip`:
 
 ```shell
-python3 -m pip install dropbox-sign==1.3.0
+python3 -m pip install dropbox-sign==1.4.0
 ```
 
 Alternatively:
 
 ```shell
 pip install git+https://github.com/hellosign/dropbox-sign-python.git
 ```
@@ -137,14 +137,18 @@
 ```OAuthApi``` | [```oauth_token_refresh```](docs/OAuthApi.md#oauth_token_refresh) | ```POST /oauth/token?refresh``` | OAuth Token Refresh|
 |```ReportApi``` | [```report_create```](docs/ReportApi.md#report_create) | ```POST /report/create``` | Create Report|
 |```SignatureRequestApi``` | [```signature_request_bulk_create_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_bulk_create_embedded_with_template) | ```POST /signature_request/bulk_create_embedded_with_template``` | Embedded Bulk Send with Template|
 ```SignatureRequestApi``` | [```signature_request_bulk_send_with_template```](docs/SignatureRequestApi.md#signature_request_bulk_send_with_template) | ```POST /signature_request/bulk_send_with_template``` | Bulk Send with Template|
 ```SignatureRequestApi``` | [```signature_request_cancel```](docs/SignatureRequestApi.md#signature_request_cancel) | ```POST /signature_request/cancel/{signature_request_id}``` | Cancel Incomplete Signature Request|
 ```SignatureRequestApi``` | [```signature_request_create_embedded```](docs/SignatureRequestApi.md#signature_request_create_embedded) | ```POST /signature_request/create_embedded``` | Create Embedded Signature Request|
 ```SignatureRequestApi``` | [```signature_request_create_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_create_embedded_with_template) | ```POST /signature_request/create_embedded_with_template``` | Create Embedded Signature Request with Template|
+```SignatureRequestApi``` | [```signature_request_edit```](docs/SignatureRequestApi.md#signature_request_edit) | ```PUT /signature_request/edit/{signature_request_id}``` | Edit Signature Request|
+```SignatureRequestApi``` | [```signature_request_edit_embedded```](docs/SignatureRequestApi.md#signature_request_edit_embedded) | ```PUT /signature_request/edit_embedded/{signature_request_id}``` | Edit Embedded Signature Request|
+```SignatureRequestApi``` | [```signature_request_edit_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_edit_embedded_with_template) | ```PUT /signature_request/edit_embedded_with_template/{signature_request_id}``` | Edit Embedded Signature Request with Template|
+```SignatureRequestApi``` | [```signature_request_edit_with_template```](docs/SignatureRequestApi.md#signature_request_edit_with_template) | ```PUT /signature_request/edit_with_template/{signature_request_id}``` | Edit Signature Request With Template|
 ```SignatureRequestApi``` | [```signature_request_files```](docs/SignatureRequestApi.md#signature_request_files) | ```GET /signature_request/files/{signature_request_id}``` | Download Files|
 ```SignatureRequestApi``` | [```signature_request_files_as_data_uri```](docs/SignatureRequestApi.md#signature_request_files_as_data_uri) | ```GET /signature_request/files_as_data_uri/{signature_request_id}``` | Download Files as Data Uri|
 ```SignatureRequestApi``` | [```signature_request_files_as_file_url```](docs/SignatureRequestApi.md#signature_request_files_as_file_url) | ```GET /signature_request/files_as_file_url/{signature_request_id}``` | Download Files as File Url|
 ```SignatureRequestApi``` | [```signature_request_get```](docs/SignatureRequestApi.md#signature_request_get) | ```GET /signature_request/{signature_request_id}``` | Get Signature Request|
 ```SignatureRequestApi``` | [```signature_request_list```](docs/SignatureRequestApi.md#signature_request_list) | ```GET /signature_request/list``` | List Signature Requests|
 ```SignatureRequestApi``` | [```signature_request_release_hold```](docs/SignatureRequestApi.md#signature_request_release_hold) | ```POST /signature_request/release_hold/{signature_request_id}``` | Release On-Hold Signature Request|
 ```SignatureRequestApi``` | [```signature_request_remind```](docs/SignatureRequestApi.md#signature_request_remind) | ```POST /signature_request/remind/{signature_request_id}``` | Send Request Reminder|
@@ -223,14 +227,18 @@
  - [ReportCreateRequest](docs/ReportCreateRequest.md)
  - [ReportCreateResponse](docs/ReportCreateResponse.md)
  - [ReportResponse](docs/ReportResponse.md)
  - [SignatureRequestBulkCreateEmbeddedWithTemplateRequest](docs/SignatureRequestBulkCreateEmbeddedWithTemplateRequest.md)
  - [SignatureRequestBulkSendWithTemplateRequest](docs/SignatureRequestBulkSendWithTemplateRequest.md)
  - [SignatureRequestCreateEmbeddedRequest](docs/SignatureRequestCreateEmbeddedRequest.md)
  - [SignatureRequestCreateEmbeddedWithTemplateRequest](docs/SignatureRequestCreateEmbeddedWithTemplateRequest.md)
+ - [SignatureRequestEditEmbeddedRequest](docs/SignatureRequestEditEmbeddedRequest.md)
+ - [SignatureRequestEditEmbeddedWithTemplateRequest](docs/SignatureRequestEditEmbeddedWithTemplateRequest.md)
+ - [SignatureRequestEditRequest](docs/SignatureRequestEditRequest.md)
+ - [SignatureRequestEditWithTemplateRequest](docs/SignatureRequestEditWithTemplateRequest.md)
  - [SignatureRequestGetResponse](docs/SignatureRequestGetResponse.md)
  - [SignatureRequestListResponse](docs/SignatureRequestListResponse.md)
  - [SignatureRequestRemindRequest](docs/SignatureRequestRemindRequest.md)
  - [SignatureRequestResponse](docs/SignatureRequestResponse.md)
  - [SignatureRequestResponseAttachment](docs/SignatureRequestResponseAttachment.md)
  - [SignatureRequestResponseCustomFieldBase](docs/SignatureRequestResponseCustomFieldBase.md)
  - [SignatureRequestResponseCustomFieldCheckbox](docs/SignatureRequestResponseCustomFieldCheckbox.md)
@@ -373,10 +381,10 @@
 
 
 ## About this package
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 3.0.0
-- Package version: 1.3.0
+- Package version: 1.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
```

### Comparing `dropbox-sign-1.3.0/README.md` & `dropbox-sign-1.4.0/dropbox_sign.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: dropbox-sign
+Version: 1.4.0
+Summary: Dropbox Sign API
+Home-page: https://github.com/hellosign/dropbox-sign-python
+Author: Dropbox Sign API Team
+Author-email: apisupport@hellosign.com
+License: MIT
+Keywords: OpenAPI,OpenAPI-Generator,Dropbox Sign API
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: urllib3>=1.25.3
+Requires-Dist: python-dateutil
+
 # dropbox-sign
 
 Dropbox Sign v3 API
 
 ## Migrating from legacy SDK
 
 This SDK is generated from our officially maintained [OpenAPI spec](https://github.com/hellosign/hellosign-openapi/blob/main/openapi.yaml).
@@ -46,15 +61,15 @@
 Python >=3.7
 
 ### pip
 
 Install using `pip`:
 
 ```shell
-python3 -m pip install dropbox-sign==1.3.0
+python3 -m pip install dropbox-sign==1.4.0
 ```
 
 Alternatively:
 
 ```shell
 pip install git+https://github.com/hellosign/dropbox-sign-python.git
 ```
@@ -122,14 +137,18 @@
 ```OAuthApi``` | [```oauth_token_refresh```](docs/OAuthApi.md#oauth_token_refresh) | ```POST /oauth/token?refresh``` | OAuth Token Refresh|
 |```ReportApi``` | [```report_create```](docs/ReportApi.md#report_create) | ```POST /report/create``` | Create Report|
 |```SignatureRequestApi``` | [```signature_request_bulk_create_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_bulk_create_embedded_with_template) | ```POST /signature_request/bulk_create_embedded_with_template``` | Embedded Bulk Send with Template|
 ```SignatureRequestApi``` | [```signature_request_bulk_send_with_template```](docs/SignatureRequestApi.md#signature_request_bulk_send_with_template) | ```POST /signature_request/bulk_send_with_template``` | Bulk Send with Template|
 ```SignatureRequestApi``` | [```signature_request_cancel```](docs/SignatureRequestApi.md#signature_request_cancel) | ```POST /signature_request/cancel/{signature_request_id}``` | Cancel Incomplete Signature Request|
 ```SignatureRequestApi``` | [```signature_request_create_embedded```](docs/SignatureRequestApi.md#signature_request_create_embedded) | ```POST /signature_request/create_embedded``` | Create Embedded Signature Request|
 ```SignatureRequestApi``` | [```signature_request_create_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_create_embedded_with_template) | ```POST /signature_request/create_embedded_with_template``` | Create Embedded Signature Request with Template|
+```SignatureRequestApi``` | [```signature_request_edit```](docs/SignatureRequestApi.md#signature_request_edit) | ```PUT /signature_request/edit/{signature_request_id}``` | Edit Signature Request|
+```SignatureRequestApi``` | [```signature_request_edit_embedded```](docs/SignatureRequestApi.md#signature_request_edit_embedded) | ```PUT /signature_request/edit_embedded/{signature_request_id}``` | Edit Embedded Signature Request|
+```SignatureRequestApi``` | [```signature_request_edit_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_edit_embedded_with_template) | ```PUT /signature_request/edit_embedded_with_template/{signature_request_id}``` | Edit Embedded Signature Request with Template|
+```SignatureRequestApi``` | [```signature_request_edit_with_template```](docs/SignatureRequestApi.md#signature_request_edit_with_template) | ```PUT /signature_request/edit_with_template/{signature_request_id}``` | Edit Signature Request With Template|
 ```SignatureRequestApi``` | [```signature_request_files```](docs/SignatureRequestApi.md#signature_request_files) | ```GET /signature_request/files/{signature_request_id}``` | Download Files|
 ```SignatureRequestApi``` | [```signature_request_files_as_data_uri```](docs/SignatureRequestApi.md#signature_request_files_as_data_uri) | ```GET /signature_request/files_as_data_uri/{signature_request_id}``` | Download Files as Data Uri|
 ```SignatureRequestApi``` | [```signature_request_files_as_file_url```](docs/SignatureRequestApi.md#signature_request_files_as_file_url) | ```GET /signature_request/files_as_file_url/{signature_request_id}``` | Download Files as File Url|
 ```SignatureRequestApi``` | [```signature_request_get```](docs/SignatureRequestApi.md#signature_request_get) | ```GET /signature_request/{signature_request_id}``` | Get Signature Request|
 ```SignatureRequestApi``` | [```signature_request_list```](docs/SignatureRequestApi.md#signature_request_list) | ```GET /signature_request/list``` | List Signature Requests|
 ```SignatureRequestApi``` | [```signature_request_release_hold```](docs/SignatureRequestApi.md#signature_request_release_hold) | ```POST /signature_request/release_hold/{signature_request_id}``` | Release On-Hold Signature Request|
 ```SignatureRequestApi``` | [```signature_request_remind```](docs/SignatureRequestApi.md#signature_request_remind) | ```POST /signature_request/remind/{signature_request_id}``` | Send Request Reminder|
@@ -208,14 +227,18 @@
  - [ReportCreateRequest](docs/ReportCreateRequest.md)
  - [ReportCreateResponse](docs/ReportCreateResponse.md)
  - [ReportResponse](docs/ReportResponse.md)
  - [SignatureRequestBulkCreateEmbeddedWithTemplateRequest](docs/SignatureRequestBulkCreateEmbeddedWithTemplateRequest.md)
  - [SignatureRequestBulkSendWithTemplateRequest](docs/SignatureRequestBulkSendWithTemplateRequest.md)
  - [SignatureRequestCreateEmbeddedRequest](docs/SignatureRequestCreateEmbeddedRequest.md)
  - [SignatureRequestCreateEmbeddedWithTemplateRequest](docs/SignatureRequestCreateEmbeddedWithTemplateRequest.md)
+ - [SignatureRequestEditEmbeddedRequest](docs/SignatureRequestEditEmbeddedRequest.md)
+ - [SignatureRequestEditEmbeddedWithTemplateRequest](docs/SignatureRequestEditEmbeddedWithTemplateRequest.md)
+ - [SignatureRequestEditRequest](docs/SignatureRequestEditRequest.md)
+ - [SignatureRequestEditWithTemplateRequest](docs/SignatureRequestEditWithTemplateRequest.md)
  - [SignatureRequestGetResponse](docs/SignatureRequestGetResponse.md)
  - [SignatureRequestListResponse](docs/SignatureRequestListResponse.md)
  - [SignatureRequestRemindRequest](docs/SignatureRequestRemindRequest.md)
  - [SignatureRequestResponse](docs/SignatureRequestResponse.md)
  - [SignatureRequestResponseAttachment](docs/SignatureRequestResponseAttachment.md)
  - [SignatureRequestResponseCustomFieldBase](docs/SignatureRequestResponseCustomFieldBase.md)
  - [SignatureRequestResponseCustomFieldCheckbox](docs/SignatureRequestResponseCustomFieldCheckbox.md)
@@ -358,10 +381,10 @@
 
 
 ## About this package
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 3.0.0
-- Package version: 1.3.0
+- Package version: 1.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/__init__.py` & `dropbox-sign-1.4.0/dropbox_sign/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 3.0.0
     Contact: apisupport@hellosign.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 # import ApiClient
 from dropbox_sign.api_client import ApiClient
 
 # import Configuration
 from dropbox_sign.configuration import Configuration
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/account_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/account_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/api_app_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/api_app_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['api_app_create_request'] = \
             api_app_create_request
         try:
             return self.api_app_create_endpoint.call_with_http_info(**kwargs)
         except ApiException as e:
-            if e.status == 200:
+            if e.status == 201:
                 e.body = self.api_client.deserialize(
                     response=type('obj_dict', (object,), {'data': e.body}),
                     response_type=[ApiAppGetResponse],
                     _check_type=True,
                 )
 
                 raise e
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/bulk_send_job_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/bulk_send_job_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/embedded_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/embedded_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/o_auth_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/o_auth_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/report_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/report_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/signature_request_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/signature_request_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 from dropbox_sign.model.error_response import ErrorResponse
 from dropbox_sign.model.file_response import FileResponse
 from dropbox_sign.model.file_response_data_uri import FileResponseDataUri
 from dropbox_sign.model.signature_request_bulk_create_embedded_with_template_request import SignatureRequestBulkCreateEmbeddedWithTemplateRequest
 from dropbox_sign.model.signature_request_bulk_send_with_template_request import SignatureRequestBulkSendWithTemplateRequest
 from dropbox_sign.model.signature_request_create_embedded_request import SignatureRequestCreateEmbeddedRequest
 from dropbox_sign.model.signature_request_create_embedded_with_template_request import SignatureRequestCreateEmbeddedWithTemplateRequest
+from dropbox_sign.model.signature_request_edit_embedded_request import SignatureRequestEditEmbeddedRequest
+from dropbox_sign.model.signature_request_edit_embedded_with_template_request import SignatureRequestEditEmbeddedWithTemplateRequest
+from dropbox_sign.model.signature_request_edit_request import SignatureRequestEditRequest
+from dropbox_sign.model.signature_request_edit_with_template_request import SignatureRequestEditWithTemplateRequest
 from dropbox_sign.model.signature_request_get_response import SignatureRequestGetResponse
 from dropbox_sign.model.signature_request_list_response import SignatureRequestListResponse
 from dropbox_sign.model.signature_request_remind_request import SignatureRequestRemindRequest
 from dropbox_sign.model.signature_request_send_request import SignatureRequestSendRequest
 from dropbox_sign.model.signature_request_send_with_template_request import SignatureRequestSendWithTemplateRequest
 from dropbox_sign.model.signature_request_update_request import SignatureRequestUpdateRequest
 
@@ -313,14 +317,254 @@
                 'content_type': [
                     'application/json',
                     'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
+        self.signature_request_edit_endpoint = _Endpoint(
+            settings={
+                'response_type': (SignatureRequestGetResponse,),
+                'auth': [
+                    'api_key',
+                    'oauth2'
+                ],
+                'endpoint_path': '/signature_request/edit/{signature_request_id}',
+                'operation_id': 'signature_request_edit',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'signature_request_id',
+                    'signature_request_edit_request',
+                ],
+                'required': [
+                    'signature_request_id',
+                    'signature_request_edit_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'signature_request_id':
+                        (str,),
+                    'signature_request_edit_request':
+                        (SignatureRequestEditRequest,),
+                },
+                'attribute_map': {
+                    'signature_request_id': 'signature_request_id',
+                },
+                'location_map': {
+                    'signature_request_id': 'path',
+                    'signature_request_edit_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
+        self.signature_request_edit_embedded_endpoint = _Endpoint(
+            settings={
+                'response_type': (SignatureRequestGetResponse,),
+                'auth': [
+                    'api_key',
+                    'oauth2'
+                ],
+                'endpoint_path': '/signature_request/edit_embedded/{signature_request_id}',
+                'operation_id': 'signature_request_edit_embedded',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'signature_request_id',
+                    'signature_request_edit_embedded_request',
+                ],
+                'required': [
+                    'signature_request_id',
+                    'signature_request_edit_embedded_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'signature_request_id':
+                        (str,),
+                    'signature_request_edit_embedded_request':
+                        (SignatureRequestEditEmbeddedRequest,),
+                },
+                'attribute_map': {
+                    'signature_request_id': 'signature_request_id',
+                },
+                'location_map': {
+                    'signature_request_id': 'path',
+                    'signature_request_edit_embedded_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
+        self.signature_request_edit_embedded_with_template_endpoint = _Endpoint(
+            settings={
+                'response_type': (SignatureRequestGetResponse,),
+                'auth': [
+                    'api_key',
+                    'oauth2'
+                ],
+                'endpoint_path': '/signature_request/edit_embedded_with_template/{signature_request_id}',
+                'operation_id': 'signature_request_edit_embedded_with_template',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'signature_request_id',
+                    'signature_request_edit_embedded_with_template_request',
+                ],
+                'required': [
+                    'signature_request_id',
+                    'signature_request_edit_embedded_with_template_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'signature_request_id':
+                        (str,),
+                    'signature_request_edit_embedded_with_template_request':
+                        (SignatureRequestEditEmbeddedWithTemplateRequest,),
+                },
+                'attribute_map': {
+                    'signature_request_id': 'signature_request_id',
+                },
+                'location_map': {
+                    'signature_request_id': 'path',
+                    'signature_request_edit_embedded_with_template_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
+        self.signature_request_edit_with_template_endpoint = _Endpoint(
+            settings={
+                'response_type': (SignatureRequestGetResponse,),
+                'auth': [
+                    'api_key',
+                    'oauth2'
+                ],
+                'endpoint_path': '/signature_request/edit_with_template/{signature_request_id}',
+                'operation_id': 'signature_request_edit_with_template',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'signature_request_id',
+                    'signature_request_edit_with_template_request',
+                ],
+                'required': [
+                    'signature_request_id',
+                    'signature_request_edit_with_template_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'signature_request_id':
+                        (str,),
+                    'signature_request_edit_with_template_request':
+                        (SignatureRequestEditWithTemplateRequest,),
+                },
+                'attribute_map': {
+                    'signature_request_id': 'signature_request_id',
+                },
+                'location_map': {
+                    'signature_request_id': 'path',
+                    'signature_request_edit_with_template_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json',
+                    'multipart/form-data'
+                ]
+            },
+            api_client=api_client
+        )
         self.signature_request_files_endpoint = _Endpoint(
             settings={
                 'response_type': (file_type,),
                 'auth': [
                     'api_key',
                     'oauth2'
                 ],
@@ -1397,14 +1641,430 @@
         except ApiException as e:
             if e.status == 200:
                 e.body = self.api_client.deserialize(
                     response=type('obj_dict', (object,), {'data': e.body}),
                     response_type=[SignatureRequestGetResponse],
                     _check_type=True,
                 )
+
+                raise e
+            range_code = "4XX"[0]
+            range_code_left = int(f"{range_code}00")
+            range_code_right = int(f"{range_code}99")
+
+            if range_code_left <= e.status <= range_code_right:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[ErrorResponse],
+                    _check_type=True,
+                )
+
+                raise e
+
+    def signature_request_edit(
+        self,
+        signature_request_id,
+        signature_request_edit_request,
+        **kwargs
+    ) -> SignatureRequestGetResponse:
+        """Edit Signature Request  # noqa: E501
+
+        Edits and sends a SignatureRequest with the submitted documents. If `form_fields_per_document` is not specified, a signature page will be affixed where all signers will be required to add their signature, signifying their agreement to all contained documents.  **NOTE:** Edit and resend will not deduct your signature request quota.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.signature_request_edit(signature_request_id, signature_request_edit_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            signature_request_id (str): The id of the SignatureRequest to edit.
+            signature_request_edit_request (SignatureRequestEditRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SignatureRequestGetResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['signature_request_id'] = \
+            signature_request_id
+        kwargs['signature_request_edit_request'] = \
+            signature_request_edit_request
+        try:
+            return self.signature_request_edit_endpoint.call_with_http_info(**kwargs)
+        except ApiException as e:
+            if e.status == 200:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[SignatureRequestGetResponse],
+                    _check_type=True,
+                )
+
+                raise e
+            range_code = "4XX"[0]
+            range_code_left = int(f"{range_code}00")
+            range_code_right = int(f"{range_code}99")
+
+            if range_code_left <= e.status <= range_code_right:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[ErrorResponse],
+                    _check_type=True,
+                )
+
+                raise e
+
+    def signature_request_edit_embedded(
+        self,
+        signature_request_id,
+        signature_request_edit_embedded_request,
+        **kwargs
+    ) -> SignatureRequestGetResponse:
+        """Edit Embedded Signature Request  # noqa: E501
+
+        Edits a SignatureRequest with the submitted documents to be signed in an embedded iFrame. If form_fields_per_document is not specified, a signature page will be affixed where all signers will be required to add their signature, signifying their agreement to all contained documents. <u>Note</u> that embedded signature requests can only be signed in embedded iFrames whereas normal signature requests can only be signed on Dropbox Sign.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.signature_request_edit_embedded(signature_request_id, signature_request_edit_embedded_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            signature_request_id (str): The id of the SignatureRequest to edit.
+            signature_request_edit_embedded_request (SignatureRequestEditEmbeddedRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SignatureRequestGetResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['signature_request_id'] = \
+            signature_request_id
+        kwargs['signature_request_edit_embedded_request'] = \
+            signature_request_edit_embedded_request
+        try:
+            return self.signature_request_edit_embedded_endpoint.call_with_http_info(**kwargs)
+        except ApiException as e:
+            if e.status == 200:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[SignatureRequestGetResponse],
+                    _check_type=True,
+                )
+
+                raise e
+            range_code = "4XX"[0]
+            range_code_left = int(f"{range_code}00")
+            range_code_right = int(f"{range_code}99")
+
+            if range_code_left <= e.status <= range_code_right:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[ErrorResponse],
+                    _check_type=True,
+                )
+
+                raise e
+
+    def signature_request_edit_embedded_with_template(
+        self,
+        signature_request_id,
+        signature_request_edit_embedded_with_template_request,
+        **kwargs
+    ) -> SignatureRequestGetResponse:
+        """Edit Embedded Signature Request with Template  # noqa: E501
+
+        Edits a SignatureRequest based on the given Template(s) to be signed in an embedded iFrame. <u>Note</u> that embedded signature requests can only be signed in embedded iFrames whereas normal signature requests can only be signed on Dropbox Sign.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.signature_request_edit_embedded_with_template(signature_request_id, signature_request_edit_embedded_with_template_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            signature_request_id (str): The id of the SignatureRequest to edit.
+            signature_request_edit_embedded_with_template_request (SignatureRequestEditEmbeddedWithTemplateRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SignatureRequestGetResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['signature_request_id'] = \
+            signature_request_id
+        kwargs['signature_request_edit_embedded_with_template_request'] = \
+            signature_request_edit_embedded_with_template_request
+        try:
+            return self.signature_request_edit_embedded_with_template_endpoint.call_with_http_info(**kwargs)
+        except ApiException as e:
+            if e.status == 200:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[SignatureRequestGetResponse],
+                    _check_type=True,
+                )
+
+                raise e
+            range_code = "4XX"[0]
+            range_code_left = int(f"{range_code}00")
+            range_code_right = int(f"{range_code}99")
+
+            if range_code_left <= e.status <= range_code_right:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[ErrorResponse],
+                    _check_type=True,
+                )
+
+                raise e
+
+    def signature_request_edit_with_template(
+        self,
+        signature_request_id,
+        signature_request_edit_with_template_request,
+        **kwargs
+    ) -> SignatureRequestGetResponse:
+        """Edit Signature Request With Template  # noqa: E501
+
+        Edits and sends a SignatureRequest based off of the Template(s) specified with the template_ids parameter.  **NOTE:** Edit and resend will not deduct your signature request quota.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.signature_request_edit_with_template(signature_request_id, signature_request_edit_with_template_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            signature_request_id (str): The id of the SignatureRequest to edit.
+            signature_request_edit_with_template_request (SignatureRequestEditWithTemplateRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            SignatureRequestGetResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['signature_request_id'] = \
+            signature_request_id
+        kwargs['signature_request_edit_with_template_request'] = \
+            signature_request_edit_with_template_request
+        try:
+            return self.signature_request_edit_with_template_endpoint.call_with_http_info(**kwargs)
+        except ApiException as e:
+            if e.status == 200:
+                e.body = self.api_client.deserialize(
+                    response=type('obj_dict', (object,), {'data': e.body}),
+                    response_type=[SignatureRequestGetResponse],
+                    _check_type=True,
+                )
 
                 raise e
             range_code = "4XX"[0]
             range_code_left = int(f"{range_code}00")
             range_code_right = int(f"{range_code}99")
 
             if range_code_left <= e.status <= range_code_right:
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/team_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/team_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1328,15 +1328,15 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['team_remove_member_request'] = \
             team_remove_member_request
         try:
             return self.team_remove_member_endpoint.call_with_http_info(**kwargs)
         except ApiException as e:
-            if e.status == 200:
+            if e.status == 201:
                 e.body = self.api_client.deserialize(
                     response=type('obj_dict', (object,), {'data': e.body}),
                     response_type=[TeamGetResponse],
                     _check_type=True,
                 )
 
                 raise e
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/template_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/template_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api/unclaimed_draft_api.py` & `dropbox-sign-1.4.0/dropbox_sign/api/unclaimed_draft_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/api_client.py` & `dropbox-sign-1.4.0/dropbox_sign/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.4.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/apis/__init__.py` & `dropbox-sign-1.4.0/dropbox_sign/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/configuration.py` & `dropbox-sign-1.4.0/dropbox_sign/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0.0\n"\
-               "SDK Package Version: 1.3.0".\
+               "SDK Package Version: 1.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/event_callback_helper.py` & `dropbox-sign-1.4.0/dropbox_sign/event_callback_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,11 +30,11 @@
         "app_callback" will always include a value for "reported_for_app_id"
 
         Args:
             event_callback (EventCallbackRequest):
         """
         metadata: EventCallbackRequestEventMetadata = event_callback.event.event_metadata
 
-        if not metadata.reported_for_app_id:
+        if not metadata or not metadata.reported_for_app_id:
             return cls.EVENT_TYPE_ACCOUNT_CALLBACK
 
         return cls.EVENT_TYPE_APP_CALLBACK
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/exceptions.py` & `dropbox-sign-1.4.0/dropbox_sign/exceptions.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_create_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_create_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_create_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_create_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_get_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_get_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_response_quotas.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_response_quotas.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_update_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_update_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_verify_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_verify_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_verify_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_verify_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/account_verify_response_account.py` & `dropbox-sign-1.4.0/dropbox_sign/model/account_verify_response_account.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_create_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_create_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_get_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_get_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_list_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_list_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_o_auth.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_o_auth.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_options.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_options.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_owner_account.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_owner_account.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_response_white_labeling_options.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_response_white_labeling_options.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/api_app_update_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/api_app_update_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_get_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_get_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_get_response_signature_requests.py` & `dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_get_response_signature_requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,14 +120,15 @@
             'is_declined': (bool,),  # noqa: E501
             'has_error': (bool,),  # noqa: E501
             'files_url': (str,),  # noqa: E501
             'signing_url': (str, none_type,),  # noqa: E501
             'details_url': (str,),  # noqa: E501
             'cc_email_addresses': ([str],),  # noqa: E501
             'signing_redirect_url': (str, none_type,),  # noqa: E501
+            'final_copy_uri': (str, none_type,),  # noqa: E501
             'template_ids': ([str], none_type,),  # noqa: E501
             'custom_fields': ([SignatureRequestResponseCustomFieldBase], none_type,),  # noqa: E501
             'attachments': ([SignatureRequestResponseAttachment], none_type,),  # noqa: E501
             'response_data': ([SignatureRequestResponseDataBase], none_type,),  # noqa: E501
             'signatures': ([SignatureRequestResponseSignatures],),  # noqa: E501
             'bulk_send_job_id': (str,),  # noqa: E501
         }
@@ -168,14 +169,15 @@
         'is_declined': 'is_declined',  # noqa: E501
         'has_error': 'has_error',  # noqa: E501
         'files_url': 'files_url',  # noqa: E501
         'signing_url': 'signing_url',  # noqa: E501
         'details_url': 'details_url',  # noqa: E501
         'cc_email_addresses': 'cc_email_addresses',  # noqa: E501
         'signing_redirect_url': 'signing_redirect_url',  # noqa: E501
+        'final_copy_uri': 'final_copy_uri',  # noqa: E501
         'template_ids': 'template_ids',  # noqa: E501
         'custom_fields': 'custom_fields',  # noqa: E501
         'attachments': 'attachments',  # noqa: E501
         'response_data': 'response_data',  # noqa: E501
         'signatures': 'signatures',  # noqa: E501
         'bulk_send_job_id': 'bulk_send_job_id',  # noqa: E501
     }
@@ -324,14 +326,22 @@
         return self.get("signing_redirect_url")
 
     @signing_redirect_url.setter
     def signing_redirect_url(self, value: Optional[str]):
         setattr(self, "signing_redirect_url", value)
 
     @property
+    def final_copy_uri(self) -> Optional[str]:
+        return self.get("final_copy_uri")
+
+    @final_copy_uri.setter
+    def final_copy_uri(self, value: Optional[str]):
+        setattr(self, "final_copy_uri", value)
+
+    @property
     def template_ids(self) -> Optional[List[str]]:
         return self.get("template_ids")
 
     @template_ids.setter
     def template_ids(self, value: Optional[List[str]]):
         setattr(self, "template_ids", value)
 
@@ -425,14 +435,15 @@
             is_declined (bool): Whether or not the SignatureRequest has been declined by a signer.. [optional]  # noqa: E501
             has_error (bool): Whether or not an error occurred (either during the creation of the SignatureRequest or during one of the signings).. [optional]  # noqa: E501
             files_url (str): The URL where a copy of the request's documents can be downloaded.. [optional]  # noqa: E501
             signing_url (str, none_type): The URL where a signer, after authenticating, can sign the documents. This should only be used by users with existing Dropbox Sign accounts as they will be required to log in before signing.. [optional]  # noqa: E501
             details_url (str): The URL where the requester and the signers can view the current status of the SignatureRequest.. [optional]  # noqa: E501
             cc_email_addresses ([str]): A list of email addresses that were CCed on the SignatureRequest. They will receive a copy of the final PDF once all the signers have signed.. [optional]  # noqa: E501
             signing_redirect_url (str, none_type): The URL you want the signer redirected to after they successfully sign.. [optional]  # noqa: E501
+            final_copy_uri (str, none_type): The path where the completed document can be downloaded. [optional]  # noqa: E501
             template_ids ([str], none_type): Templates IDs used in this SignatureRequest (if any).. [optional]  # noqa: E501
             custom_fields ([SignatureRequestResponseCustomFieldBase], none_type): An array of Custom Field objects containing the name and type of each custom field.  * Text Field uses `SignatureRequestResponseCustomFieldText` * Checkbox Field uses `SignatureRequestResponseCustomFieldCheckbox`. [optional]  # noqa: E501
             attachments ([SignatureRequestResponseAttachment], none_type): Signer attachments.. [optional]  # noqa: E501
             response_data ([SignatureRequestResponseDataBase], none_type): An array of form field objects containing the name, value, and type of each textbox or checkmark field filled in by the signers.. [optional]  # noqa: E501
             signatures ([SignatureRequestResponseSignatures]): An array of signature objects, 1 for each signer.. [optional]  # noqa: E501
             bulk_send_job_id (str): The id of the BulkSendJob.. [optional]  # noqa: E501
         """
@@ -548,14 +559,15 @@
             is_declined (bool): Whether or not the SignatureRequest has been declined by a signer.. [optional]  # noqa: E501
             has_error (bool): Whether or not an error occurred (either during the creation of the SignatureRequest or during one of the signings).. [optional]  # noqa: E501
             files_url (str): The URL where a copy of the request's documents can be downloaded.. [optional]  # noqa: E501
             signing_url (str, none_type): The URL where a signer, after authenticating, can sign the documents. This should only be used by users with existing Dropbox Sign accounts as they will be required to log in before signing.. [optional]  # noqa: E501
             details_url (str): The URL where the requester and the signers can view the current status of the SignatureRequest.. [optional]  # noqa: E501
             cc_email_addresses ([str]): A list of email addresses that were CCed on the SignatureRequest. They will receive a copy of the final PDF once all the signers have signed.. [optional]  # noqa: E501
             signing_redirect_url (str, none_type): The URL you want the signer redirected to after they successfully sign.. [optional]  # noqa: E501
+            final_copy_uri (str, none_type): The path where the completed document can be downloaded. [optional]  # noqa: E501
             template_ids ([str], none_type): Templates IDs used in this SignatureRequest (if any).. [optional]  # noqa: E501
             custom_fields ([SignatureRequestResponseCustomFieldBase], none_type): An array of Custom Field objects containing the name and type of each custom field.  * Text Field uses `SignatureRequestResponseCustomFieldText` * Checkbox Field uses `SignatureRequestResponseCustomFieldCheckbox`. [optional]  # noqa: E501
             attachments ([SignatureRequestResponseAttachment], none_type): Signer attachments.. [optional]  # noqa: E501
             response_data ([SignatureRequestResponseDataBase], none_type): An array of form field objects containing the name, value, and type of each textbox or checkmark field filled in by the signers.. [optional]  # noqa: E501
             signatures ([SignatureRequestResponseSignatures]): An array of signature objects, 1 for each signer.. [optional]  # noqa: E501
             bulk_send_job_id (str): The id of the BulkSendJob.. [optional]  # noqa: E501
         """
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_list_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_list_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/bulk_send_job_send_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/bulk_send_job_send_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/embedded_edit_url_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/embedded_edit_url_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/embedded_edit_url_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/embedded_edit_url_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/embedded_edit_url_response_embedded.py` & `dropbox-sign-1.4.0/dropbox_sign/model/embedded_edit_url_response_embedded.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/embedded_sign_url_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/embedded_sign_url_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/embedded_sign_url_response_embedded.py` & `dropbox-sign-1.4.0/dropbox_sign/model/embedded_sign_url_response_embedded.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/error_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/error_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/error_response_error.py` & `dropbox-sign-1.4.0/dropbox_sign/model/error_response_error.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/event_callback_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/event_callback_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/event_callback_request_event.py` & `dropbox-sign-1.4.0/dropbox_sign/model/event_callback_request_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
             'SIGNATURE_REQUEST_REASSIGNED': "signature_request_reassigned",
             'SIGNATURE_REQUEST_INVALID': "signature_request_invalid",
             'SIGNATURE_REQUEST_PREPARED': "signature_request_prepared",
             'SIGNATURE_REQUEST_EXPIRED': "signature_request_expired",
             'TEMPLATE_CREATED': "template_created",
             'TEMPLATE_ERROR': "template_error",
             'CALLBACK_TEST': "callback_test",
+            'SIGNATURE_REQUEST_SIGNER_REMOVED': "signature_request_signer_removed",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -186,22 +187,21 @@
 
     @event_metadata.setter
     def event_metadata(self, value: EventCallbackRequestEventMetadata):
         setattr(self, "event_metadata", value)
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, event_time, event_type, event_hash, event_metadata, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, event_time, event_type, event_hash, *args, **kwargs):  # noqa: E501
         """EventCallbackRequestEvent - a model defined in OpenAPI
 
         Args:
             event_time (str): Time the event was created (using Unix time).
             event_type (str): Type of callback event that was triggered.
             event_hash (str): Generated hash used to verify source of event data.
-            event_metadata (EventCallbackRequestEventMetadata):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,14 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            event_metadata (EventCallbackRequestEventMetadata): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +257,14 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.event_time = event_time
         self.event_type = event_type
         self.event_hash = event_hash
-        self.event_metadata = event_metadata
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -277,22 +277,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, event_time, event_type, event_hash, event_metadata, *args, **kwargs):  # noqa: E501
+    def __init__(self, event_time, event_type, event_hash, *args, **kwargs):  # noqa: E501
         """EventCallbackRequestEvent - a model defined in OpenAPI
 
         Args:
             event_time (str): Time the event was created (using Unix time).
             event_type (str): Type of callback event that was triggered.
             event_hash (str): Generated hash used to verify source of event data.
-            event_metadata (EventCallbackRequestEventMetadata):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -317,14 +316,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            event_metadata (EventCallbackRequestEventMetadata): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -345,15 +345,14 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.event_time = event_time
         self.event_type = event_type
         self.event_hash = event_hash
-        self.event_metadata = event_metadata
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/event_callback_request_event_metadata.py` & `dropbox-sign-1.4.0/dropbox_sign/model/event_callback_request_event_metadata.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/file_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/file_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/file_response_data_uri.py` & `dropbox-sign-1.4.0/dropbox_sign/model/file_response_data_uri.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/list_info_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/list_info_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/o_auth_token_generate_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/o_auth_token_generate_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/o_auth_token_refresh_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/o_auth_token_refresh_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/o_auth_token_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/o_auth_token_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/report_create_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/report_create_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/report_create_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/report_create_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/report_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/report_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_bulk_create_embedded_with_template_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_bulk_create_embedded_with_template_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -307,15 +307,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
+            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
             signer_list ([SubBulkSignerList]): `signer_list` is an array defining values and options for signer fields. Required unless a `signer_file` is used, you may not use both.. [optional]  # noqa: E501
             allow_decline (bool): Allows signers to decline to sign a document if `true`. Defaults to `false`.. [optional] if omitted the server will use the default value of False  # noqa: E501
             ccs ([SubCC]): Add CC email recipients. Required when a CC role exists for the Template.. [optional]  # noqa: E501
             custom_fields ([SubCustomField]): When used together with merge fields, `custom_fields` allows users to add pre-filled data to their signature requests.  Pre-filled data can be used with \"send-once\" signature requests by adding merge fields with `form_fields_per_document` or [Text Tags](https://app.hellosign.com/api/textTagsWalkthrough#TextTagIntro) while passing values back with `custom_fields` together in one API call.  For using pre-filled on repeatable signature requests, merge fields are added to templates in the Dropbox Sign UI or by calling [/template/create_embedded_draft](/api/reference/operation/templateCreateEmbeddedDraft) and then passing `custom_fields` on subsequent signature requests referencing that template.. [optional]  # noqa: E501
             message (str): The custom message in the email that will be sent to the signers.. [optional]  # noqa: E501
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Key-value data that should be attached to the signature request. This metadata is included in all API responses and events involving the signature request. For example, use the metadata field to store a signer's order number for look up when receiving events for the signature request.  Each request can include up to 10 metadata keys (or 50 nested metadata keys), with key names up to 40 characters long and values up to 1000 characters long.. [optional]  # noqa: E501
             signing_redirect_url (str): The URL you want signers redirected to after they successfully sign.. [optional]  # noqa: E501
@@ -405,15 +405,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
+            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
             signer_list ([SubBulkSignerList]): `signer_list` is an array defining values and options for signer fields. Required unless a `signer_file` is used, you may not use both.. [optional]  # noqa: E501
             allow_decline (bool): Allows signers to decline to sign a document if `true`. Defaults to `false`.. [optional] if omitted the server will use the default value of False  # noqa: E501
             ccs ([SubCC]): Add CC email recipients. Required when a CC role exists for the Template.. [optional]  # noqa: E501
             custom_fields ([SubCustomField]): When used together with merge fields, `custom_fields` allows users to add pre-filled data to their signature requests.  Pre-filled data can be used with \"send-once\" signature requests by adding merge fields with `form_fields_per_document` or [Text Tags](https://app.hellosign.com/api/textTagsWalkthrough#TextTagIntro) while passing values back with `custom_fields` together in one API call.  For using pre-filled on repeatable signature requests, merge fields are added to templates in the Dropbox Sign UI or by calling [/template/create_embedded_draft](/api/reference/operation/templateCreateEmbeddedDraft) and then passing `custom_fields` on subsequent signature requests referencing that template.. [optional]  # noqa: E501
             message (str): The custom message in the email that will be sent to the signers.. [optional]  # noqa: E501
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Key-value data that should be attached to the signature request. This metadata is included in all API responses and events involving the signature request. For example, use the metadata field to store a signer's order number for look up when receiving events for the signature request.  Each request can include up to 10 metadata keys (or 50 nested metadata keys), with key names up to 40 characters long and values up to 1000 characters long.. [optional]  # noqa: E501
             signing_redirect_url (str): The URL you want signers redirected to after they successfully sign.. [optional]  # noqa: E501
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_bulk_send_with_template_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_bulk_send_with_template_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
+            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
             signer_list ([SubBulkSignerList]): `signer_list` is an array defining values and options for signer fields. Required unless a `signer_file` is used, you may not use both.. [optional]  # noqa: E501
             allow_decline (bool): Allows signers to decline to sign a document if `true`. Defaults to `false`.. [optional] if omitted the server will use the default value of False  # noqa: E501
             ccs ([SubCC]): Add CC email recipients. Required when a CC role exists for the Template.. [optional]  # noqa: E501
             client_id (str): The client id of the API App you want to associate with this request. Used to apply the branding and callback url defined for the app.. [optional]  # noqa: E501
             custom_fields ([SubCustomField]): When used together with merge fields, `custom_fields` allows users to add pre-filled data to their signature requests.  Pre-filled data can be used with \"send-once\" signature requests by adding merge fields with `form_fields_per_document` or [Text Tags](https://app.hellosign.com/api/textTagsWalkthrough#TextTagIntro) while passing values back with `custom_fields` together in one API call.  For using pre-filled on repeatable signature requests, merge fields are added to templates in the Dropbox Sign UI or by calling [/template/create_embedded_draft](/api/reference/operation/templateCreateEmbeddedDraft) and then passing `custom_fields` on subsequent signature requests referencing that template.. [optional]  # noqa: E501
             message (str): The custom message in the email that will be sent to the signers.. [optional]  # noqa: E501
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Key-value data that should be attached to the signature request. This metadata is included in all API responses and events involving the signature request. For example, use the metadata field to store a signer's order number for look up when receiving events for the signature request.  Each request can include up to 10 metadata keys (or 50 nested metadata keys), with key names up to 40 characters long and values up to 1000 characters long.. [optional]  # noqa: E501
@@ -403,15 +403,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
+            signer_file (file_type): `signer_file` is a CSV file defining values and options for signer fields. Required unless a `signer_list` is used, you may not use both. The CSV can have the following columns:  - `name`: the name of the signer filling the role of RoleName - `email_address`: email address of the signer filling the role of RoleName - `pin`: the 4- to 12-character access code that will secure this signer's signature page (optional) - `sms_phone_number`: An E.164 formatted phone number that will receive a code via SMS to access this signer's signature page. (optional)      By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).      **Note**: Not available in test mode and requires a Standard plan or higher. - `*_field`: any column with a _field\" suffix will be treated as a custom field (optional)      You may only specify field values here, any other options should be set in the custom_fields request parameter.  Example CSV:  ``` name, email_address, pin, company_field George, george@example.com, d79a3td, ABC Corp Mary, mary@example.com, gd9as5b, 123 LLC ```. [optional]  # noqa: E501
             signer_list ([SubBulkSignerList]): `signer_list` is an array defining values and options for signer fields. Required unless a `signer_file` is used, you may not use both.. [optional]  # noqa: E501
             allow_decline (bool): Allows signers to decline to sign a document if `true`. Defaults to `false`.. [optional] if omitted the server will use the default value of False  # noqa: E501
             ccs ([SubCC]): Add CC email recipients. Required when a CC role exists for the Template.. [optional]  # noqa: E501
             client_id (str): The client id of the API App you want to associate with this request. Used to apply the branding and callback url defined for the app.. [optional]  # noqa: E501
             custom_fields ([SubCustomField]): When used together with merge fields, `custom_fields` allows users to add pre-filled data to their signature requests.  Pre-filled data can be used with \"send-once\" signature requests by adding merge fields with `form_fields_per_document` or [Text Tags](https://app.hellosign.com/api/textTagsWalkthrough#TextTagIntro) while passing values back with `custom_fields` together in one API call.  For using pre-filled on repeatable signature requests, merge fields are added to templates in the Dropbox Sign UI or by calling [/template/create_embedded_draft](/api/reference/operation/templateCreateEmbeddedDraft) and then passing `custom_fields` on subsequent signature requests referencing that template.. [optional]  # noqa: E501
             message (str): The custom message in the email that will be sent to the signers.. [optional]  # noqa: E501
             metadata ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): Key-value data that should be attached to the signature request. This metadata is included in all API responses and events involving the signature request. For example, use the metadata field to store a signer's order number for look up when receiving events for the signature request.  Each request can include up to 10 metadata keys (or 50 nested metadata keys), with key names up to 40 characters long and values up to 1000 characters long.. [optional]  # noqa: E501
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_create_embedded_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_create_embedded_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_create_embedded_with_template_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_create_embedded_with_template_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_get_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_get_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_list_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_list_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_remind_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_remind_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,19 +117,21 @@
             'is_declined': (bool,),  # noqa: E501
             'has_error': (bool,),  # noqa: E501
             'files_url': (str,),  # noqa: E501
             'signing_url': (str, none_type,),  # noqa: E501
             'details_url': (str,),  # noqa: E501
             'cc_email_addresses': ([str],),  # noqa: E501
             'signing_redirect_url': (str, none_type,),  # noqa: E501
+            'final_copy_uri': (str, none_type,),  # noqa: E501
             'template_ids': ([str], none_type,),  # noqa: E501
             'custom_fields': ([SignatureRequestResponseCustomFieldBase], none_type,),  # noqa: E501
             'attachments': ([SignatureRequestResponseAttachment], none_type,),  # noqa: E501
             'response_data': ([SignatureRequestResponseDataBase], none_type,),  # noqa: E501
             'signatures': ([SignatureRequestResponseSignatures],),  # noqa: E501
+            'bulk_send_job_id': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     @staticmethod
@@ -163,19 +165,21 @@
         'is_declined': 'is_declined',  # noqa: E501
         'has_error': 'has_error',  # noqa: E501
         'files_url': 'files_url',  # noqa: E501
         'signing_url': 'signing_url',  # noqa: E501
         'details_url': 'details_url',  # noqa: E501
         'cc_email_addresses': 'cc_email_addresses',  # noqa: E501
         'signing_redirect_url': 'signing_redirect_url',  # noqa: E501
+        'final_copy_uri': 'final_copy_uri',  # noqa: E501
         'template_ids': 'template_ids',  # noqa: E501
         'custom_fields': 'custom_fields',  # noqa: E501
         'attachments': 'attachments',  # noqa: E501
         'response_data': 'response_data',  # noqa: E501
         'signatures': 'signatures',  # noqa: E501
+        'bulk_send_job_id': 'bulk_send_job_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -320,14 +324,22 @@
         return self.get("signing_redirect_url")
 
     @signing_redirect_url.setter
     def signing_redirect_url(self, value: Optional[str]):
         setattr(self, "signing_redirect_url", value)
 
     @property
+    def final_copy_uri(self) -> Optional[str]:
+        return self.get("final_copy_uri")
+
+    @final_copy_uri.setter
+    def final_copy_uri(self, value: Optional[str]):
+        setattr(self, "final_copy_uri", value)
+
+    @property
     def template_ids(self) -> Optional[List[str]]:
         return self.get("template_ids")
 
     @template_ids.setter
     def template_ids(self, value: Optional[List[str]]):
         setattr(self, "template_ids", value)
 
@@ -359,14 +371,22 @@
     def signatures(self) -> List[SignatureRequestResponseSignatures]:
         return self.get("signatures")
 
     @signatures.setter
     def signatures(self, value: List[SignatureRequestResponseSignatures]):
         setattr(self, "signatures", value)
 
+    @property
+    def bulk_send_job_id(self) -> Optional[str]:
+        return self.get("bulk_send_job_id")
+
+    @bulk_send_job_id.setter
+    def bulk_send_job_id(self, value: Optional[str]):
+        setattr(self, "bulk_send_job_id", value)
+
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """SignatureRequestResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -413,19 +433,21 @@
             is_declined (bool): Whether or not the SignatureRequest has been declined by a signer.. [optional]  # noqa: E501
             has_error (bool): Whether or not an error occurred (either during the creation of the SignatureRequest or during one of the signings).. [optional]  # noqa: E501
             files_url (str): The URL where a copy of the request's documents can be downloaded.. [optional]  # noqa: E501
             signing_url (str, none_type): The URL where a signer, after authenticating, can sign the documents. This should only be used by users with existing Dropbox Sign accounts as they will be required to log in before signing.. [optional]  # noqa: E501
             details_url (str): The URL where the requester and the signers can view the current status of the SignatureRequest.. [optional]  # noqa: E501
             cc_email_addresses ([str]): A list of email addresses that were CCed on the SignatureRequest. They will receive a copy of the final PDF once all the signers have signed.. [optional]  # noqa: E501
             signing_redirect_url (str, none_type): The URL you want the signer redirected to after they successfully sign.. [optional]  # noqa: E501
+            final_copy_uri (str, none_type): The path where the completed document can be downloaded. [optional]  # noqa: E501
             template_ids ([str], none_type): Templates IDs used in this SignatureRequest (if any).. [optional]  # noqa: E501
             custom_fields ([SignatureRequestResponseCustomFieldBase], none_type): An array of Custom Field objects containing the name and type of each custom field.  * Text Field uses `SignatureRequestResponseCustomFieldText` * Checkbox Field uses `SignatureRequestResponseCustomFieldCheckbox`. [optional]  # noqa: E501
             attachments ([SignatureRequestResponseAttachment], none_type): Signer attachments.. [optional]  # noqa: E501
             response_data ([SignatureRequestResponseDataBase], none_type): An array of form field objects containing the name, value, and type of each textbox or checkmark field filled in by the signers.. [optional]  # noqa: E501
             signatures ([SignatureRequestResponseSignatures]): An array of signature objects, 1 for each signer.. [optional]  # noqa: E501
+            bulk_send_job_id (str, none_type): The ID of the Bulk Send job which sent the signature request, if applicable.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -517,19 +539,21 @@
             is_declined (bool): Whether or not the SignatureRequest has been declined by a signer.. [optional]  # noqa: E501
             has_error (bool): Whether or not an error occurred (either during the creation of the SignatureRequest or during one of the signings).. [optional]  # noqa: E501
             files_url (str): The URL where a copy of the request's documents can be downloaded.. [optional]  # noqa: E501
             signing_url (str, none_type): The URL where a signer, after authenticating, can sign the documents. This should only be used by users with existing Dropbox Sign accounts as they will be required to log in before signing.. [optional]  # noqa: E501
             details_url (str): The URL where the requester and the signers can view the current status of the SignatureRequest.. [optional]  # noqa: E501
             cc_email_addresses ([str]): A list of email addresses that were CCed on the SignatureRequest. They will receive a copy of the final PDF once all the signers have signed.. [optional]  # noqa: E501
             signing_redirect_url (str, none_type): The URL you want the signer redirected to after they successfully sign.. [optional]  # noqa: E501
+            final_copy_uri (str, none_type): The path where the completed document can be downloaded. [optional]  # noqa: E501
             template_ids ([str], none_type): Templates IDs used in this SignatureRequest (if any).. [optional]  # noqa: E501
             custom_fields ([SignatureRequestResponseCustomFieldBase], none_type): An array of Custom Field objects containing the name and type of each custom field.  * Text Field uses `SignatureRequestResponseCustomFieldText` * Checkbox Field uses `SignatureRequestResponseCustomFieldCheckbox`. [optional]  # noqa: E501
             attachments ([SignatureRequestResponseAttachment], none_type): Signer attachments.. [optional]  # noqa: E501
             response_data ([SignatureRequestResponseDataBase], none_type): An array of form field objects containing the name, value, and type of each textbox or checkmark field filled in by the signers.. [optional]  # noqa: E501
             signatures ([SignatureRequestResponseSignatures]): An array of signature objects, 1 for each signer.. [optional]  # noqa: E501
+            bulk_send_job_id (str, none_type): The ID of the Bulk Send job which sent the signature request, if applicable.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_attachment.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_attachment.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_base.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_base.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_checkbox.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_checkbox.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_text.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_text.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_custom_field_type_enum.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_custom_field_type_enum.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_base.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_base.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_type_enum.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_type_enum.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_checkbox.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_checkbox.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_checkbox_merge.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_checkbox_merge.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_date_signed.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_date_signed.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_dropdown.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_dropdown.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_initials.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_initials.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_radio.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_radio.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_signature.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_signature.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_text.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_text.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_data_value_text_merge.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_data_value_text_merge.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_response_signatures.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_response_signatures.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_send_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_send_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_send_with_template_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_send_with_template_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/signature_request_update_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/signature_request_update_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_attachment.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_attachment.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_bulk_signer_list.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_bulk_signer_list.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_bulk_signer_list_custom_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_bulk_signer_list_custom_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_cc.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_cc.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_custom_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_custom_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_editor_options.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_editor_options.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_field_options.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_field_options.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_group.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_group.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_rule.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_rule.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_rule_action.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_rule_action.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_field_rule_trigger.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_field_rule_trigger.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_base.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_base.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_checkbox.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_checkbox.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_checkbox_merge.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_checkbox_merge.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_date_signed.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_date_signed.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "date_signed")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -426,15 +426,15 @@
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "date_signed")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_dropdown.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_dropdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             content (str): Selected value in `options` array. Value must exist in array.. [optional]  # noqa: E501
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "dropdown")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -453,15 +453,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             content (str): Selected value in `options` array. Value must exist in array.. [optional]  # noqa: E501
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "dropdown")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_font_enum.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_font_enum.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_hyperlink.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_hyperlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "hyperlink")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -450,15 +450,15 @@
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "hyperlink")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_initials.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_initials.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_radio.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_radio.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_signature.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_signature.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_text.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,15 +413,15 @@
             link_id (str): Link two or more text fields. Enter data into one linked text field, which automatically fill all other linked text fields.. [optional]  # noqa: E501
             masked (bool): Masks entered data. For more information see [Masking sensitive information](https://faq.hellosign.com/hc/en-us/articles/360040742811-Masking-sensitive-information). `true` for masking the data in a text field, otherwise `false`.. [optional]  # noqa: E501
             validation_type (str): Each text field may contain a `validation_type` parameter. Check out the list of [validation types](https://faq.hellosign.com/hc/en-us/articles/217115577) to learn more about the possible values.  **NOTE**: When using `custom_regex` you are required to pass a second parameter `validation_custom_regex` and you can optionally provide `validation_custom_regex_format_label` for the error message the user will see in case of an invalid value.. [optional]  # noqa: E501
             validation_custom_regex (str): [optional]  # noqa: E501
             validation_custom_regex_format_label (str): [optional]  # noqa: E501
             content (str): Content of a `me_now` text field. [optional]  # noqa: E501
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "text")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -534,15 +534,15 @@
             link_id (str): Link two or more text fields. Enter data into one linked text field, which automatically fill all other linked text fields.. [optional]  # noqa: E501
             masked (bool): Masks entered data. For more information see [Masking sensitive information](https://faq.hellosign.com/hc/en-us/articles/360040742811-Masking-sensitive-information). `true` for masking the data in a text field, otherwise `false`.. [optional]  # noqa: E501
             validation_type (str): Each text field may contain a `validation_type` parameter. Check out the list of [validation types](https://faq.hellosign.com/hc/en-us/articles/217115577) to learn more about the possible values.  **NOTE**: When using `custom_regex` you are required to pass a second parameter `validation_custom_regex` and you can optionally provide `validation_custom_regex_format_label` for the error message the user will see in case of an invalid value.. [optional]  # noqa: E501
             validation_custom_regex (str): [optional]  # noqa: E501
             validation_custom_regex_format_label (str): [optional]  # noqa: E501
             content (str): Content of a `me_now` text field. [optional]  # noqa: E501
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "text")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_text_merge.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_text_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "text-merge")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -426,15 +426,15 @@
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             font_family (str): Font family for the field.. [optional]  # noqa: E501
-            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional]  # noqa: E501
+            font_size (int): The initial px font size for the field contents. Can be any integer value between `7` and `49`.  **NOTE**: Font size may be reduced during processing in order to fit the contents within the dimensions of the field.. [optional] if omitted the server will use the default value of 12  # noqa: E501
             name (str): Display name for the field.. [optional]  # noqa: E501
             page (int, none_type): Page in the document where the field should be placed (requires documents be PDF files).  - When the page number parameter is supplied, the API will use the new coordinate system. - Check out the differences between both [coordinate systems](https://faq.hellosign.com/hc/en-us/articles/217115577) and how to use them.. [optional]  # noqa: E501
         """
 
         type = kwargs.get('type', "text-merge")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_form_fields_per_document_type_enum.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_form_fields_per_document_type_enum.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_merge_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_merge_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_o_auth.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_o_auth.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_options.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_options.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_signature_request_grouped_signers.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_signature_request_grouped_signers.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_signature_request_signer.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_signature_request_template_signer.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from dropbox_sign.exceptions import ApiAttributeError
 
 
 
-class SubSignatureRequestSigner(ModelNormal):
+class SubSignatureRequestTemplateSigner(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -90,57 +90,65 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'role': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'email_address': (str,),  # noqa: E501
-            'order': (int, none_type,),  # noqa: E501
             'pin': (str,),  # noqa: E501
             'sms_phone_number': (str,),  # noqa: E501
             'sms_phone_number_type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     @staticmethod
-    def init(data: any) -> SubSignatureRequestSigner:
+    def init(data: any) -> SubSignatureRequestTemplateSigner:
         """
         Attempt to instantiate and hydrate a new instance of this class
         """
         try:
             obj_data = json.dumps(data)
         except TypeError:
             obj_data = data
 
         return ApiClient().deserialize(
             response=type('obj_dict', (object,), {'data': obj_data}),
-            response_type=[SubSignatureRequestSigner],
+            response_type=[SubSignatureRequestTemplateSigner],
             _check_type=True,
         )
 
     attribute_map = {
+        'role': 'role',  # noqa: E501
         'name': 'name',  # noqa: E501
         'email_address': 'email_address',  # noqa: E501
-        'order': 'order',  # noqa: E501
         'pin': 'pin',  # noqa: E501
         'sms_phone_number': 'sms_phone_number',  # noqa: E501
         'sms_phone_number_type': 'sms_phone_number_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @property
+    def role(self) -> str:
+        return self.get("role")
+
+    @role.setter
+    def role(self, value: str):
+        setattr(self, "role", value)
+
+    @property
     def name(self) -> str:
         return self.get("name")
 
     @name.setter
     def name(self, value: str):
         setattr(self, "name", value)
 
@@ -149,22 +157,14 @@
         return self.get("email_address")
 
     @email_address.setter
     def email_address(self, value: str):
         setattr(self, "email_address", value)
 
     @property
-    def order(self) -> Optional[int]:
-        return self.get("order")
-
-    @order.setter
-    def order(self, value: Optional[int]):
-        setattr(self, "order", value)
-
-    @property
     def pin(self) -> str:
         return self.get("pin")
 
     @pin.setter
     def pin(self, value: str):
         setattr(self, "pin", value)
 
@@ -182,18 +182,19 @@
 
     @sms_phone_number_type.setter
     def sms_phone_number_type(self, value: str):
         setattr(self, "sms_phone_number_type", value)
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, email_address, *args, **kwargs):  # noqa: E501
-        """SubSignatureRequestSigner - a model defined in OpenAPI
+    def _from_openapi_data(cls, role, name, email_address, *args, **kwargs):  # noqa: E501
+        """SubSignatureRequestTemplateSigner - a model defined in OpenAPI
 
         Args:
+            role (str): Must match an existing role in chosen Template(s). It's case-sensitive.
             name (str): The name of the signer.
             email_address (str): The email address of the signer.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -220,17 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            order (int, none_type): The order the signer is required to sign in.. [optional]  # noqa: E501
             pin (str): The 4- to 12-character access code that will secure this signer's signature page.. [optional]  # noqa: E501
-            sms_phone_number (str): An E.164 formatted phone number.  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
+            sms_phone_number (str): An E.164 formatted phone number.  By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
             sms_phone_number_type (str): Specifies the feature used with the `sms_phone_number`. Default `authentication`.  If `authentication`, signer is sent a verification code via SMS that is required to access the document.  If `delivery`, a link to complete the signature request is delivered via SMS (_and_ email).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -251,14 +251,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.role = role
         self.name = name
         self.email_address = email_address
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -273,18 +274,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, email_address, *args, **kwargs):  # noqa: E501
-        """SubSignatureRequestSigner - a model defined in OpenAPI
+    def __init__(self, role, name, email_address, *args, **kwargs):  # noqa: E501
+        """SubSignatureRequestTemplateSigner - a model defined in OpenAPI
 
         Args:
+            role (str): Must match an existing role in chosen Template(s). It's case-sensitive.
             name (str): The name of the signer.
             email_address (str): The email address of the signer.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -311,17 +313,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            order (int, none_type): The order the signer is required to sign in.. [optional]  # noqa: E501
             pin (str): The 4- to 12-character access code that will secure this signer's signature page.. [optional]  # noqa: E501
-            sms_phone_number (str): An E.164 formatted phone number.  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
+            sms_phone_number (str): An E.164 formatted phone number.  By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
             sms_phone_number_type (str): Specifies the feature used with the `sms_phone_number`. Default `authentication`.  If `authentication`, signer is sent a verification code via SMS that is required to access the document.  If `delivery`, a link to complete the signature request is delivered via SMS (_and_ email).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -340,14 +341,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.role = role
         self.name = name
         self.email_address = email_address
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_signature_request_template_signer.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_signature_request_signer.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from dropbox_sign.exceptions import ApiAttributeError
 
 
 
-class SubSignatureRequestTemplateSigner(ModelNormal):
+class SubSignatureRequestSigner(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -90,65 +90,57 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'role': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'email_address': (str,),  # noqa: E501
+            'order': (int, none_type,),  # noqa: E501
             'pin': (str,),  # noqa: E501
             'sms_phone_number': (str,),  # noqa: E501
             'sms_phone_number_type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     @staticmethod
-    def init(data: any) -> SubSignatureRequestTemplateSigner:
+    def init(data: any) -> SubSignatureRequestSigner:
         """
         Attempt to instantiate and hydrate a new instance of this class
         """
         try:
             obj_data = json.dumps(data)
         except TypeError:
             obj_data = data
 
         return ApiClient().deserialize(
             response=type('obj_dict', (object,), {'data': obj_data}),
-            response_type=[SubSignatureRequestTemplateSigner],
+            response_type=[SubSignatureRequestSigner],
             _check_type=True,
         )
 
     attribute_map = {
-        'role': 'role',  # noqa: E501
         'name': 'name',  # noqa: E501
         'email_address': 'email_address',  # noqa: E501
+        'order': 'order',  # noqa: E501
         'pin': 'pin',  # noqa: E501
         'sms_phone_number': 'sms_phone_number',  # noqa: E501
         'sms_phone_number_type': 'sms_phone_number_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @property
-    def role(self) -> str:
-        return self.get("role")
-
-    @role.setter
-    def role(self, value: str):
-        setattr(self, "role", value)
-
-    @property
     def name(self) -> str:
         return self.get("name")
 
     @name.setter
     def name(self, value: str):
         setattr(self, "name", value)
 
@@ -157,14 +149,22 @@
         return self.get("email_address")
 
     @email_address.setter
     def email_address(self, value: str):
         setattr(self, "email_address", value)
 
     @property
+    def order(self) -> Optional[int]:
+        return self.get("order")
+
+    @order.setter
+    def order(self, value: Optional[int]):
+        setattr(self, "order", value)
+
+    @property
     def pin(self) -> str:
         return self.get("pin")
 
     @pin.setter
     def pin(self, value: str):
         setattr(self, "pin", value)
 
@@ -182,19 +182,18 @@
 
     @sms_phone_number_type.setter
     def sms_phone_number_type(self, value: str):
         setattr(self, "sms_phone_number_type", value)
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, role, name, email_address, *args, **kwargs):  # noqa: E501
-        """SubSignatureRequestTemplateSigner - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, email_address, *args, **kwargs):  # noqa: E501
+        """SubSignatureRequestSigner - a model defined in OpenAPI
 
         Args:
-            role (str): Must match an existing role in chosen Template(s). It's case-sensitive.
             name (str): The name of the signer.
             email_address (str): The email address of the signer.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -221,16 +220,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            order (int, none_type): The order the signer is required to sign in.. [optional]  # noqa: E501
             pin (str): The 4- to 12-character access code that will secure this signer's signature page.. [optional]  # noqa: E501
-            sms_phone_number (str): An E.164 formatted phone number.  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
+            sms_phone_number (str): An E.164 formatted phone number.  By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
             sms_phone_number_type (str): Specifies the feature used with the `sms_phone_number`. Default `authentication`.  If `authentication`, signer is sent a verification code via SMS that is required to access the document.  If `delivery`, a link to complete the signature request is delivered via SMS (_and_ email).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -251,15 +251,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.role = role
         self.name = name
         self.email_address = email_address
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -274,19 +273,18 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, role, name, email_address, *args, **kwargs):  # noqa: E501
-        """SubSignatureRequestTemplateSigner - a model defined in OpenAPI
+    def __init__(self, name, email_address, *args, **kwargs):  # noqa: E501
+        """SubSignatureRequestSigner - a model defined in OpenAPI
 
         Args:
-            role (str): Must match an existing role in chosen Template(s). It's case-sensitive.
             name (str): The name of the signer.
             email_address (str): The email address of the signer.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -313,16 +311,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            order (int, none_type): The order the signer is required to sign in.. [optional]  # noqa: E501
             pin (str): The 4- to 12-character access code that will secure this signer's signature page.. [optional]  # noqa: E501
-            sms_phone_number (str): An E.164 formatted phone number.  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
+            sms_phone_number (str): An E.164 formatted phone number.  By using the feature, you agree you are responsible for obtaining a signer's consent to receive text messages from Dropbox Sign related to this signature request and confirm you have obtained such consent from all signers prior to enabling SMS delivery for this signature request. [Learn more](https://faq.hellosign.com/hc/en-us/articles/15815316468877-Dropbox-Sign-SMS-tools-add-on).  **Note**: Not available in test mode and requires a Standard plan or higher.. [optional]  # noqa: E501
             sms_phone_number_type (str): Specifies the feature used with the `sms_phone_number`. Default `authentication`.  If `authentication`, signer is sent a verification code via SMS that is required to access the document.  If `delivery`, a link to complete the signature request is delivered via SMS (_and_ email).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -341,15 +340,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.role = role
         self.name = name
         self.email_address = email_address
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_signing_options.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_signing_options.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_team_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_team_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_template_role.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_template_role.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_unclaimed_draft_signer.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_unclaimed_draft_signer.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_unclaimed_draft_template_signer.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_unclaimed_draft_template_signer.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/sub_white_labeling_options.py` & `dropbox-sign-1.4.0/dropbox_sign/model/sub_white_labeling_options.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_add_member_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_add_member_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_create_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_create_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_get_info_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_get_info_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_get_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_get_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_info_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_info_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_invite_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_invite_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_invites_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_invites_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_member_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_member_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_members_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_members_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_parent_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_parent_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_remove_member_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_remove_member_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_sub_teams_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_sub_teams_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/team_update_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/team_update_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_add_user_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_add_user_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_create_embedded_draft_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_create_embedded_draft_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_create_embedded_draft_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_create_embedded_draft_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_create_embedded_draft_response_template.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_create_embedded_draft_response_template.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_create_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_create_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_create_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_create_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_create_response_template.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_create_response_template.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_edit_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_edit_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_get_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_get_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_list_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_list_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_remove_user_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_remove_user_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_account.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_account.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_account_quota.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_account_quota.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_cc_role.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_cc_role.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_custom_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_custom_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field_base.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field_base.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field_checkbox.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field_checkbox.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_custom_field_text.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_custom_field_text.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_field_group.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_field_group.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_field_group_rule.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_field_group_rule.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_base.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_base.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_checkbox.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_checkbox.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_date_signed.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_date_signed.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_dropdown.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_dropdown.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_hyperlink.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_hyperlink.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_initials.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_initials.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_radio.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_radio.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_signature.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_signature.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_form_field_text.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_form_field_text.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_base.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_base.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_checkbox.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_checkbox.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_date_signed.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_date_signed.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_dropdown.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_dropdown.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_hyperlink.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_hyperlink.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_initials.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_initials.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_radio.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_radio.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_signature.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_signature.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_document_static_field_text.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_document_static_field_text.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_field_avg_text_length.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_field_avg_text_length.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_named_form_field.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_named_form_field.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_response_signer_role.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_response_signer_role.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_update_files_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_update_files_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_update_files_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_update_files_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/template_update_files_response_template.py` & `dropbox-sign-1.4.0/dropbox_sign/model/template_update_files_response_template.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_embedded_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_embedded_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_embedded_with_template_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_embedded_with_template_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_create_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_create_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_edit_and_resend_request.py` & `dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_edit_and_resend_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/unclaimed_draft_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/unclaimed_draft_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model/warning_response.py` & `dropbox-sign-1.4.0/dropbox_sign/model/warning_response.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/model_utils.py` & `dropbox-sign-1.4.0/dropbox_sign/model_utils.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign/models/__init__.py` & `dropbox-sign-1.4.0/dropbox_sign/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 from dropbox_sign.model.report_create_request import ReportCreateRequest
 from dropbox_sign.model.report_create_response import ReportCreateResponse
 from dropbox_sign.model.report_response import ReportResponse
 from dropbox_sign.model.signature_request_bulk_create_embedded_with_template_request import SignatureRequestBulkCreateEmbeddedWithTemplateRequest
 from dropbox_sign.model.signature_request_bulk_send_with_template_request import SignatureRequestBulkSendWithTemplateRequest
 from dropbox_sign.model.signature_request_create_embedded_request import SignatureRequestCreateEmbeddedRequest
 from dropbox_sign.model.signature_request_create_embedded_with_template_request import SignatureRequestCreateEmbeddedWithTemplateRequest
+from dropbox_sign.model.signature_request_edit_embedded_request import SignatureRequestEditEmbeddedRequest
+from dropbox_sign.model.signature_request_edit_embedded_with_template_request import SignatureRequestEditEmbeddedWithTemplateRequest
+from dropbox_sign.model.signature_request_edit_request import SignatureRequestEditRequest
+from dropbox_sign.model.signature_request_edit_with_template_request import SignatureRequestEditWithTemplateRequest
 from dropbox_sign.model.signature_request_get_response import SignatureRequestGetResponse
 from dropbox_sign.model.signature_request_list_response import SignatureRequestListResponse
 from dropbox_sign.model.signature_request_remind_request import SignatureRequestRemindRequest
 from dropbox_sign.model.signature_request_response import SignatureRequestResponse
 from dropbox_sign.model.signature_request_response_attachment import SignatureRequestResponseAttachment
 from dropbox_sign.model.signature_request_response_custom_field_base import SignatureRequestResponseCustomFieldBase
 from dropbox_sign.model.signature_request_response_custom_field_checkbox import SignatureRequestResponseCustomFieldCheckbox
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign/rest.py` & `dropbox-sign-1.4.0/dropbox_sign/rest.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/dropbox_sign.egg-info/PKG-INFO` & `dropbox-sign-1.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dropbox-sign
-Version: 1.3.0
-Summary: Dropbox Sign API
-Home-page: https://github.com/hellosign/dropbox-sign-python
-Author: Dropbox Sign API Team
-Author-email: apisupport@hellosign.com
-License: MIT
-Keywords: OpenAPI,OpenAPI-Generator,Dropbox Sign API
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: urllib3>=1.25.3
-Requires-Dist: python-dateutil
-
 # dropbox-sign
 
 Dropbox Sign v3 API
 
 ## Migrating from legacy SDK
 
 This SDK is generated from our officially maintained [OpenAPI spec](https://github.com/hellosign/hellosign-openapi/blob/main/openapi.yaml).
@@ -61,15 +46,15 @@
 Python >=3.7
 
 ### pip
 
 Install using `pip`:
 
 ```shell
-python3 -m pip install dropbox-sign==1.3.0
+python3 -m pip install dropbox-sign==1.4.0
 ```
 
 Alternatively:
 
 ```shell
 pip install git+https://github.com/hellosign/dropbox-sign-python.git
 ```
@@ -137,14 +122,18 @@
 ```OAuthApi``` | [```oauth_token_refresh```](docs/OAuthApi.md#oauth_token_refresh) | ```POST /oauth/token?refresh``` | OAuth Token Refresh|
 |```ReportApi``` | [```report_create```](docs/ReportApi.md#report_create) | ```POST /report/create``` | Create Report|
 |```SignatureRequestApi``` | [```signature_request_bulk_create_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_bulk_create_embedded_with_template) | ```POST /signature_request/bulk_create_embedded_with_template``` | Embedded Bulk Send with Template|
 ```SignatureRequestApi``` | [```signature_request_bulk_send_with_template```](docs/SignatureRequestApi.md#signature_request_bulk_send_with_template) | ```POST /signature_request/bulk_send_with_template``` | Bulk Send with Template|
 ```SignatureRequestApi``` | [```signature_request_cancel```](docs/SignatureRequestApi.md#signature_request_cancel) | ```POST /signature_request/cancel/{signature_request_id}``` | Cancel Incomplete Signature Request|
 ```SignatureRequestApi``` | [```signature_request_create_embedded```](docs/SignatureRequestApi.md#signature_request_create_embedded) | ```POST /signature_request/create_embedded``` | Create Embedded Signature Request|
 ```SignatureRequestApi``` | [```signature_request_create_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_create_embedded_with_template) | ```POST /signature_request/create_embedded_with_template``` | Create Embedded Signature Request with Template|
+```SignatureRequestApi``` | [```signature_request_edit```](docs/SignatureRequestApi.md#signature_request_edit) | ```PUT /signature_request/edit/{signature_request_id}``` | Edit Signature Request|
+```SignatureRequestApi``` | [```signature_request_edit_embedded```](docs/SignatureRequestApi.md#signature_request_edit_embedded) | ```PUT /signature_request/edit_embedded/{signature_request_id}``` | Edit Embedded Signature Request|
+```SignatureRequestApi``` | [```signature_request_edit_embedded_with_template```](docs/SignatureRequestApi.md#signature_request_edit_embedded_with_template) | ```PUT /signature_request/edit_embedded_with_template/{signature_request_id}``` | Edit Embedded Signature Request with Template|
+```SignatureRequestApi``` | [```signature_request_edit_with_template```](docs/SignatureRequestApi.md#signature_request_edit_with_template) | ```PUT /signature_request/edit_with_template/{signature_request_id}``` | Edit Signature Request With Template|
 ```SignatureRequestApi``` | [```signature_request_files```](docs/SignatureRequestApi.md#signature_request_files) | ```GET /signature_request/files/{signature_request_id}``` | Download Files|
 ```SignatureRequestApi``` | [```signature_request_files_as_data_uri```](docs/SignatureRequestApi.md#signature_request_files_as_data_uri) | ```GET /signature_request/files_as_data_uri/{signature_request_id}``` | Download Files as Data Uri|
 ```SignatureRequestApi``` | [```signature_request_files_as_file_url```](docs/SignatureRequestApi.md#signature_request_files_as_file_url) | ```GET /signature_request/files_as_file_url/{signature_request_id}``` | Download Files as File Url|
 ```SignatureRequestApi``` | [```signature_request_get```](docs/SignatureRequestApi.md#signature_request_get) | ```GET /signature_request/{signature_request_id}``` | Get Signature Request|
 ```SignatureRequestApi``` | [```signature_request_list```](docs/SignatureRequestApi.md#signature_request_list) | ```GET /signature_request/list``` | List Signature Requests|
 ```SignatureRequestApi``` | [```signature_request_release_hold```](docs/SignatureRequestApi.md#signature_request_release_hold) | ```POST /signature_request/release_hold/{signature_request_id}``` | Release On-Hold Signature Request|
 ```SignatureRequestApi``` | [```signature_request_remind```](docs/SignatureRequestApi.md#signature_request_remind) | ```POST /signature_request/remind/{signature_request_id}``` | Send Request Reminder|
@@ -223,14 +212,18 @@
  - [ReportCreateRequest](docs/ReportCreateRequest.md)
  - [ReportCreateResponse](docs/ReportCreateResponse.md)
  - [ReportResponse](docs/ReportResponse.md)
  - [SignatureRequestBulkCreateEmbeddedWithTemplateRequest](docs/SignatureRequestBulkCreateEmbeddedWithTemplateRequest.md)
  - [SignatureRequestBulkSendWithTemplateRequest](docs/SignatureRequestBulkSendWithTemplateRequest.md)
  - [SignatureRequestCreateEmbeddedRequest](docs/SignatureRequestCreateEmbeddedRequest.md)
  - [SignatureRequestCreateEmbeddedWithTemplateRequest](docs/SignatureRequestCreateEmbeddedWithTemplateRequest.md)
+ - [SignatureRequestEditEmbeddedRequest](docs/SignatureRequestEditEmbeddedRequest.md)
+ - [SignatureRequestEditEmbeddedWithTemplateRequest](docs/SignatureRequestEditEmbeddedWithTemplateRequest.md)
+ - [SignatureRequestEditRequest](docs/SignatureRequestEditRequest.md)
+ - [SignatureRequestEditWithTemplateRequest](docs/SignatureRequestEditWithTemplateRequest.md)
  - [SignatureRequestGetResponse](docs/SignatureRequestGetResponse.md)
  - [SignatureRequestListResponse](docs/SignatureRequestListResponse.md)
  - [SignatureRequestRemindRequest](docs/SignatureRequestRemindRequest.md)
  - [SignatureRequestResponse](docs/SignatureRequestResponse.md)
  - [SignatureRequestResponseAttachment](docs/SignatureRequestResponseAttachment.md)
  - [SignatureRequestResponseCustomFieldBase](docs/SignatureRequestResponseCustomFieldBase.md)
  - [SignatureRequestResponseCustomFieldCheckbox](docs/SignatureRequestResponseCustomFieldCheckbox.md)
@@ -373,10 +366,10 @@
 
 
 ## About this package
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 3.0.0
-- Package version: 1.3.0
+- Package version: 1.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
```

### Comparing `dropbox-sign-1.3.0/dropbox_sign.egg-info/SOURCES.txt` & `dropbox-sign-1.4.0/dropbox_sign.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 dropbox_sign/model/report_create_request.py
 dropbox_sign/model/report_create_response.py
 dropbox_sign/model/report_response.py
 dropbox_sign/model/signature_request_bulk_create_embedded_with_template_request.py
 dropbox_sign/model/signature_request_bulk_send_with_template_request.py
 dropbox_sign/model/signature_request_create_embedded_request.py
 dropbox_sign/model/signature_request_create_embedded_with_template_request.py
+dropbox_sign/model/signature_request_edit_embedded_request.py
+dropbox_sign/model/signature_request_edit_embedded_with_template_request.py
+dropbox_sign/model/signature_request_edit_request.py
+dropbox_sign/model/signature_request_edit_with_template_request.py
 dropbox_sign/model/signature_request_get_response.py
 dropbox_sign/model/signature_request_list_response.py
 dropbox_sign/model/signature_request_remind_request.py
 dropbox_sign/model/signature_request_response.py
 dropbox_sign/model/signature_request_response_attachment.py
 dropbox_sign/model/signature_request_response_custom_field_base.py
 dropbox_sign/model/signature_request_response_custom_field_checkbox.py
```

### Comparing `dropbox-sign-1.3.0/setup.py` & `dropbox-sign-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 from pathlib import Path
 
 NAME = "dropbox-sign"
-VERSION = "1.3.0"
+VERSION = "1.4.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `dropbox-sign-1.3.0/tests/test_account_api.py` & `dropbox-sign-1.4.0/tests/test_account_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_api_app_api.py` & `dropbox-sign-1.4.0/tests/test_api_app_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_bulk_send_job_api.py` & `dropbox-sign-1.4.0/tests/test_bulk_send_job_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_embedded_api.py` & `dropbox-sign-1.4.0/tests/test_embedded_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_fixtures.py` & `dropbox-sign-1.4.0/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_model_signature_request_send_request.py` & `dropbox-sign-1.4.0/tests/test_model_signature_request_send_request.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_oauth_api.py` & `dropbox-sign-1.4.0/tests/test_oauth_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_report_api.py` & `dropbox-sign-1.4.0/tests/test_report_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_signature_request_api.py` & `dropbox-sign-1.4.0/tests/test_signature_request_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_sub_form_fields_per_document_base.py` & `dropbox-sign-1.4.0/tests/test_sub_form_fields_per_document_base.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_team_api.py` & `dropbox-sign-1.4.0/tests/test_team_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_template_api.py` & `dropbox-sign-1.4.0/tests/test_template_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_unclaimed_draft_api.py` & `dropbox-sign-1.4.0/tests/test_unclaimed_draft_api.py`

 * *Files identical despite different names*

### Comparing `dropbox-sign-1.3.0/tests/test_utils.py` & `dropbox-sign-1.4.0/tests/test_utils.py`

 * *Files identical despite different names*

