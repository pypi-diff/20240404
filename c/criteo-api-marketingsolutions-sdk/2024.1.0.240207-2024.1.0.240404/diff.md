# Comparing `tmp/criteo-api-marketingsolutions-sdk-2024.1.0.240207.tar.gz` & `tmp/criteo-api-marketingsolutions-sdk-2024.1.0.240404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-marketingsolutions-sdk-2024.1.0.240207.tar", last modified: Wed Feb  7 14:28:42 2024, max compression
+gzip compressed data, was "criteo-api-marketingsolutions-sdk-2024.1.0.240404.tar", last modified: Thu Apr  4 16:25:30 2024, max compression
```

## Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207.tar` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404.tar`

### file list

```diff
@@ -1,295 +1,295 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.091808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-07 14:28:42.091808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.091808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-07 14:28:42.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20931 2024-02-07 14:28:42.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 14:28:42.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-07 14:28:42.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-07 14:28:42.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.035808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.039808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/advertiser_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   103164 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    83985 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    96298 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/creative_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39256 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.039808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16743 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/flow_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.087808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_input_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_filter_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_request_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/adaptive_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/adaptive_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/adaptive_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/algebra_node_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_create_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_delete_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_update_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_compute_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_compute_sizes_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_delete_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_audience_search_metadata_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_name_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    12554 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11782 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_create_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_delete_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_update_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_sizes_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_delete_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_estimate_size_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_input_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12117 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/basic_audience_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/behavioral_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_search_filters_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_search_request_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_spend_limit_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_coupon_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_coupon_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_image_slide.py
--rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_write_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/criteo_api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    14106 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/criteo_api_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/delete_audience_contact_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15174 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/dynamic_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/dynamic_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/entity_of_portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/error_code_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/get_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/html_tag_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/html_tag_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_set_base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_slide.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_write_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_size_estimation_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/lookalike_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/lookalike_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/lookalike_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/modify_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_gender_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_int32.py
--rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_string.py
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/point_of_interest_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    14720 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/problems_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/prospecting_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12516 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/prospecting_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/prospecting_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15849 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/requests_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/requests_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/responses_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/responses_read_ad_set_v23_q1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/retargeting_create_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/retargeting_update_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/retargeting_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/size.py
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/statistics_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_query_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/update_coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/update_coupon_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/update_coupon_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/video_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/write_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/write_model_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    82579 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.087808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/models/
--rw-r--r--   0 runner    (1001) docker     (127)    28396 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 14:28:42.091808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:28:42.091808 criteo-api-marketingsolutions-sdk-2024.1.0.240207/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-07 14:27:45.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240207/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.209398 criteo-api-marketingsolutions-sdk-2024.1.0.240404/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-04 16:25:30.209398 criteo-api-marketingsolutions-sdk-2024.1.0.240404/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18967 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.205398 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-04 16:25:30.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20931 2024-04-04 16:25:30.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:25:30.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 16:25:30.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 16:25:30.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.153397 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.153397 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/advertiser_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103164 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83985 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96298 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/creative_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39256 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.153397 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16743 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.205398 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11832 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_input_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_filter_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_request_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/adaptive_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/adaptive_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/adaptive_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12205 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/algebra_node_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_create_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_delete_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_update_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_compute_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_compute_sizes_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_delete_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_audience_search_metadata_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_name_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12554 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11782 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_create_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_delete_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11904 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_update_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_sizes_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_delete_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_estimate_size_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12663 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12117 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12556 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/basic_audience_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/behavioral_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_search_filters_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_search_request_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_spend_limit_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12496 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13840 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12173 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15607 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_coupon_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_image_slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11714 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/criteo_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14106 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/criteo_api_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/delete_audience_contact_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15174 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/dynamic_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/dynamic_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/entity_of_portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/error_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/get_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/html_tag_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/html_tag_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_set_base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13353 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/lookalike_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/lookalike_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/lookalike_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/modify_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_gender_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_int32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11848 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12639 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16610 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/point_of_interest_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14720 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/problems_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/prospecting_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12516 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/prospecting_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/prospecting_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15849 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12160 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/requests_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/requests_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12413 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/responses_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/responses_read_ad_set_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/retargeting_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/retargeting_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/retargeting_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/statistics_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/update_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/update_coupon_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/update_coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/video_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/write_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/write_model_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82579 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.205398 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    28396 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 16:25:30.209398 criteo-api-marketingsolutions-sdk-2024.1.0.240404/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:30.205398 criteo-api-marketingsolutions-sdk-2024.1.0.240404/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-04 16:25:04.000000 criteo-api-marketingsolutions-sdk-2024.1.0.240404/test/test_gateway_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
-Version: 2024.1.0.240207
+Version: 2024.1.0.240404
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -22,17 +22,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207
+pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2024_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/README.md` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 API Client Libraries can facilitate your use of the Criteo API allowing you to build unique and customized solutions to serve your businesses and clients.
 These libraries can reduce the amount of code you need to write in order to start accessing Criteo programmatically. They also can help expedite troubleshooting, should you encounter any issues.
 
 More information: [https://developers.criteo.com/](https://developers.criteo.com/)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- Package version: 2024.01.0.240207
+- Package version: 2024.01.0.240404
 
 ## Requirements
 
 Python 2.7 and 3.5+
 
 ## Installation & Usage
 ### pip install
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207
+pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2024_01
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
-Version: 2024.1.0.240207
+Version: 2024.1.0.240404
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -22,17 +22,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207
+pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2024_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/__init__.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Criteo API - MarketingSolutions  # noqa: E501
 
     The version of the OpenAPI document: 2024-01
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2024.01.0.240207"
+__version__ = "2024.01.0.240404"
 
 # import ApiClient
 from criteo_api_marketingsolutions_v2024_01.api_client import ApiClient
 from criteo_api_marketingsolutions_v2024_01.criteo_api_client import CriteoApiClient
 from criteo_api_marketingsolutions_v2024_01.api_client_builder import ApiClientBuilder
 from criteo_api_marketingsolutions_v2024_01 import flow_constants
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/advertiser_api.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/advertiser_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/analytics_api.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/analytics_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/audience_api.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/audience_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/campaign_api.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/campaign_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/creative_api.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/creative_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api/gateway_api.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api/gateway_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api_client.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.01.0.240207/python'
+        self.user_agent = 'OpenAPI-Generator/2024.01.0.240404/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/api_client_builder.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/apis/__init__.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/configuration.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2024-01\n"\
-               "SDK Package Version: 2024.01.0.240207".\
+               "SDK Package Version: 2024.01.0.240404".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/criteo_api_client.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/criteo_api_client.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/criteo_auth.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/criteo_auth.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/criteo_rest.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/criteo_rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/exceptions.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/exceptions.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_entity_v1_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_input_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_audience_link_input_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_category_bid_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_delivery_limitations_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_display_multiplier_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_frequency_capping_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_geo_location_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_filter_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_filter_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_request_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_search_request_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_rule_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_set_targeting_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_write.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_write.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_write_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_write_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/ad_write_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/ad_write_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/adaptive_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/adaptive_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/adaptive_colors.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/adaptive_colors.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/adaptive_write_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/adaptive_write_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/algebra_node_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/algebra_node_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/application_summary_model.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/application_summary_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/application_summary_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_create_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_create_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_delete_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_delete_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_update_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_bulk_update_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_compute_size_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_compute_size_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_compute_sizes_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_compute_sizes_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_create_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_delete_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_delete_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_audience_search_metadata_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_audience_search_metadata_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_error.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_estimate_size_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_id_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_name_description.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_name_description.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_search_metadata_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_search_metadata_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_create_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_create_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_delete_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_delete_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_update_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_bulk_update_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_size_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_size_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_sizes_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_compute_sizes_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_create_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_delete_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_delete_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_estimate_size_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_estimate_size_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_id_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_input_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_input_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_metadata_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_search_metadata_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_size_estimation_v1_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_segment_update_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_size_estimation_v1_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_update_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/audience_warning.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/audience_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/basic_audience_definition.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/basic_audience_definition.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/behavioral_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/behavioral_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_search_filters_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_search_filters_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_search_request_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_search_request_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_spend_limit_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_spend_limit_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/campaign_v23_q1_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/common_problem.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/common_problem.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_statistics_entity_v1_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contact_list_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contact_list_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_amendment_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/contactlist_operation_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/coupon_supported_sizes_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_bidding.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_budget.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_geo_location.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_geo_location.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_schedule.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_schedule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_targeting.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_ad_set_targeting.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_campaign_spend_limit.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_coupon.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_coupon.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_coupon_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_coupon_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_coupon_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_coupon_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/create_image_slide.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/create_image_slide.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_write.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_write.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_write_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_write_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/creative_write_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/creative_write_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/criteo_api_error.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/criteo_api_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/criteo_api_warning.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/criteo_api_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/delete_audience_contact_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/delete_audience_contact_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/dynamic_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/dynamic_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/dynamic_write_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/dynamic_write_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/entity_of_portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/entity_of_portfolio_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/error_code_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/error_code_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/get_portfolio_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/get_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/html_tag_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/html_tag_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/html_tag_write_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/html_tag_write_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_set_base64.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_set_base64.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_shape.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_shape.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_slide.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_slide.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/image_write_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/image_write_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_brand_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_audience_segment_interest_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_create_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_create_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_size_estimation_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_size_estimation_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_update_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_update_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/in_market_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/in_market_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_create_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_create_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_size_estimation_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_size_estimation_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_update_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_update_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/location_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/location_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/lookalike_create_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/lookalike_create_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/lookalike_update_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/lookalike_update_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/lookalike_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/lookalike_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/modify_audience_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/modify_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1_value.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_v23_q1_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_value.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_ad_set_targeting_rule_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_date_time.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_date_time.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_decimal.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_decimal.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_gender_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_gender_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_int32.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_int32.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/nillable_string.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/nillable_string.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_bidding.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_budget.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_list_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_category_bid_result_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_list_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_display_multiplier_result_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_scheduling.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_ad_set_scheduling.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_list_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_spend_limit.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_write_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_campaign_write_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/patch_result_campaign_read_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/placements_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/point_of_interest_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/point_of_interest_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/portfolio_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/problem_details.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/problems_details.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/problems_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/prospecting_create_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/prospecting_create_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/prospecting_update_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/prospecting_update_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/prospecting_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/prospecting_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_bidding_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_budget_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_schedule_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_ad_set_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_model_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/read_model_read_ad_set_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/requests_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/requests_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/requests_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/requests_patch_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/response_read_ad_set_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/responses_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/responses_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/responses_read_ad_set_v23_q1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/responses_read_ad_set_v23_q1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/retargeting_create_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/retargeting_create_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/retargeting_update_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/retargeting_update_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/retargeting_v1.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/retargeting_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/size.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/size.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/statistics_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/statistics_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/tag.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/tag.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transactions_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_query_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_attributes.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_data_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_entity_message.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/transparency_report_file.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/transparency_report_file.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/update_coupon.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/update_coupon.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/update_coupon_request.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/update_coupon_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/update_coupon_resource.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/update_coupon_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/video_detail.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/video_detail.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/write_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/write_model_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model/write_model_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model/write_model_patch_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/model_utils.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/model_utils.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/models/__init__.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/models/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/criteo_api_marketingsolutions_v2024_01/rest.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/criteo_api_marketingsolutions_v2024_01/rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/setup.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-marketingsolutions-sdk"
-VERSION = "2024.01.0.240207"
+VERSION = "2024.01.0.240404"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -20,17 +20,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207
+pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2024_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2024.1.0.240207/test/test_gateway_api.py` & `criteo-api-marketingsolutions-sdk-2024.1.0.240404/test/test_gateway_api.py`

 * *Files identical despite different names*

