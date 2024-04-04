# Comparing `tmp/criteo-api-retailmedia-sdk-2024.1.0.240207.tar.gz` & `tmp/criteo-api-retailmedia-sdk-2024.1.0.240404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-retailmedia-sdk-2024.1.0.240207.tar", last modified: Wed Feb  7 14:29:52 2024, max compression
+gzip compressed data, was "criteo-api-retailmedia-sdk-2024.1.0.240404.tar", last modified: Thu Apr  4 16:25:59 2024, max compression
```

## Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207.tar` & `criteo-api-retailmedia-sdk-2024.1.0.240404.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.327484 criteo-api-retailmedia-sdk-2024.1.0.240207/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-07 14:29:52.327484 criteo-api-retailmedia-sdk-2024.1.0.240207/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.327484 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-07 14:29:52.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-02-07 14:29:52.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 14:29:52.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-07 14:29:52.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-07 14:29:52.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.287485 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.287485 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26445 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   422793 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    39276 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.287485 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/flow_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.327484 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_funds_to_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_to_basket_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/asset_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/asset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18704 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_campaigns_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    18762 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_line_items_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_line_items_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_line_items_report_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_report_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19595 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_revenue_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_revenue_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_revenue_report_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_create_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_update_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/audience_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/audience_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/audience_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_response_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_daily_budget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_monthly_budget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    18708 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/category202204.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/category202204_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/change_dates_of_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/choice_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/choice_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/choice_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/color_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/create_balance_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12806 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202110_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202210.py
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202210_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202210_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative_create_model202207.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative_update_model202207.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/daily_line_item_budget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/editable_campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_add_funds_to_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_change_dates_of_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_create_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_line_item_capping202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_line_item_page202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_line_item_page_category202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    16309 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    15046 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_retailer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_retailer_pages202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_update_balance_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/files_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/files_variables_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/hyperlink_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/input_resource_of_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/input_resource_of_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_retailer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_request_of_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/keyword_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/keyword_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/monthly_line_item_budeget_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/page_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/page_type_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/post_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item_create_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/promoted_product202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/promoted_product202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/put_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/report_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_add_funds_to_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_balance_campaign202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_category202204.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_change_dates_of_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_create_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_creative202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_creative202210.py
--rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_update_balance_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keyword_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_input_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13663 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keyword_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_problem_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12352 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_resource_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bid_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_create_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_customer_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13142 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_create_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/section.py
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/status_response_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/store_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/store_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/store_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/text_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/text_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/update_balance_model_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_of_campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_of_line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_campaign_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_line_item_budget_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    12114 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (127)    82565 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.327484 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/models/
--rw-r--r--   0 runner    (1001) docker     (127)    24843 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 14:29:52.327484 criteo-api-retailmedia-sdk-2024.1.0.240207/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:29:52.327484 criteo-api-retailmedia-sdk-2024.1.0.240207/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-02-07 14:27:45.000000 criteo-api-retailmedia-sdk-2024.1.0.240207/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.193655 criteo-api-retailmedia-sdk-2024.1.0.240404/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-04 16:25:59.193655 criteo-api-retailmedia-sdk-2024.1.0.240404/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.193655 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-04 16:25:59.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-04-04 16:25:59.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:25:59.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 16:25:59.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 16:25:59.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.149655 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.153655 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26445 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   422793 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39276 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.153655 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.193655 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_funds_to_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_to_basket_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/asset_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_campaigns_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18908 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_line_items_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_line_items_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_line_items_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19499 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_revenue_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_revenue_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_revenue_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_create_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_update_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/audience_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/audience_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/audience_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_response_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_daily_budget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_monthly_budget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18708 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/category202204.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/category202204_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/change_dates_of_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/choice_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/choice_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/choice_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/color_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12763 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/create_balance_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12806 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202110_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202210_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202210_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative_create_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative_update_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/daily_line_item_budget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/editable_campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_add_funds_to_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15894 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12259 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_change_dates_of_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_create_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_line_item_capping202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_line_item_page202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_line_item_page_category202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16309 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15046 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11510 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_retailer_pages202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_update_balance_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/files_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/files_variables_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/hyperlink_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/input_resource_of_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/input_resource_of_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_account_and_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13156 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_request_of_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/keyword_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/keyword_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/monthly_line_item_budeget_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/page_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/page_type_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/post_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item_create_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14562 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/promoted_product202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/promoted_product202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/put_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/report_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12285 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_add_funds_to_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_balance_campaign202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_category202204.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_change_dates_of_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_create_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12278 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_update_balance_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keyword_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12208 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_input_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13663 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keyword_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12352 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_resource_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bid_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12284 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12604 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_create_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_customer_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13142 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_create_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13186 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/status_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/store_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/store_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/store_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11589 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/text_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/text_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/update_balance_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_of_campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_of_line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_campaign_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_line_item_budget_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12114 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12000 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11990 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82565 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.193655 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    24843 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 16:25:59.193655 criteo-api-retailmedia-sdk-2024.1.0.240404/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:25:59.193655 criteo-api-retailmedia-sdk-2024.1.0.240404/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-04 16:25:05.000000 criteo-api-retailmedia-sdk-2024.1.0.240404/test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/PKG-INFO` & `criteo-api-retailmedia-sdk-2024.1.0.240404/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240207
+pip install criteo-api-retailmedia-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2024_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/README.md` & `criteo-api-retailmedia-sdk-2024.1.0.240404/README.md`

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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240207
+pip install criteo-api-retailmedia-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2024_01
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/PKG-INFO` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240207
+pip install criteo-api-retailmedia-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2024_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/__init__.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Criteo API - RetailMedia  # noqa: E501
 
     The version of the OpenAPI document: 2024-01
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2024.01.0.240207"
+__version__ = "2024.01.0.240404"
 
 # import ApiClient
 from criteo_api_retailmedia_v2024_01.api_client import ApiClient
 from criteo_api_retailmedia_v2024_01.criteo_api_client import CriteoApiClient
 from criteo_api_retailmedia_v2024_01.api_client_builder import ApiClientBuilder
 from criteo_api_retailmedia_v2024_01 import flow_constants
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/analytics_api.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/analytics_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/audience_api.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/audience_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/campaign_api.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/campaign_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api/gateway_api.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api/gateway_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api_client.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api_client.py`

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

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/api_client_builder.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/apis/__init__.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/configuration.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/configuration.py`

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

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/criteo_api_client.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/criteo_api_client.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/criteo_auth.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/criteo_auth.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/criteo_rest.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/criteo_rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/exceptions.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/exceptions.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_funds_to_balance_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_funds_to_balance_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_to_basket_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_to_basket_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/add_to_basket_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/application_summary_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/application_summary_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/application_summary_model_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/application_summary_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/application_summary_model_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/application_summary_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/asset.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/asset.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/asset_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/asset_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/asset_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/asset_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_campaigns_report.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_campaigns_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,51 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('metrics',): {
-            'None': None,
-            'IMPRESSIONS': "impressions",
-            'CLICKS': "clicks",
-            'SPEND': "spend",
-            'ATTRIBUTEDSALES': "attributedSales",
-            'ATTRIBUTEDUNITS': "attributedUnits",
-            'ATTRIBUTEDORDERS': "attributedOrders",
-            'CTR': "ctr",
-            'CPC': "cpc",
-            'CPO': "cpo",
-            'CPM': "cpm",
-            'ROAS': "roas",
-            'UNIQUEVISITORS': "uniqueVisitors",
-            'FREQUENCY': "frequency",
-            'ASSISTEDUNITS': "assistedUnits",
-            'ASSISTEDSALES': "assistedSales",
-        },
-        ('dimensions',): {
-            'None': None,
-            'DATE': "date",
-            'HOUR': "hour",
-            'CAMPAIGNID': "campaignId",
-            'CAMPAIGNNAME': "campaignName",
-            'CAMPAIGNTYPENAME': "campaignTypeName",
-            'ADVPRODUCTCATEGORY': "advProductCategory",
-            'ADVPRODUCTID': "advProductId",
-            'ADVPRODUCTNAME': "advProductName",
-            'BRANDID': "brandId",
-            'BRANDNAME': "brandName",
-            'PAGETYPENAME': "pageTypeName",
-            'ENVIRONMENT': "environment",
-            'KEYWORD': "keyword",
-            'SALESCHANNEL': "salesChannel",
-            'RETAILERID': "retailerId",
-            'RETAILERNAME': "retailerName",
-        },
         ('campaign_type',): {
             'None': None,
             'SPONSOREDPRODUCTS': "sponsoredProducts",
             'ONSITEDISPLAYS': "onSiteDisplays",
         },
         ('sales_channel',): {
             'None': None,
@@ -131,14 +94,55 @@
             'None': None,
             '1D': "1D",
             '7D': "7D",
             '14D': "14D",
             '30D': "30D",
             'NONE': "none",
         },
+        ('dimensions',): {
+            'None': None,
+            'DATE': "date",
+            'HOUR': "hour",
+            'ACCOUNTID': "accountId",
+            'ACCOUNTNAME': "accountName",
+            'CAMPAIGNID': "campaignId",
+            'CAMPAIGNNAME': "campaignName",
+            'CAMPAIGNTYPENAME': "campaignTypeName",
+            'ADVPRODUCTCATEGORY': "advProductCategory",
+            'ADVPRODUCTID': "advProductId",
+            'ADVPRODUCTNAME': "advProductName",
+            'BRANDID': "brandId",
+            'BRANDNAME': "brandName",
+            'LINEITEMID': "lineItemId",
+            'LINEITEMNAME': "lineItemName",
+            'RETAILERID': "retailerId",
+            'RETAILERNAME': "retailerName",
+            'KEYWORD': "keyword",
+            'PAGETYPENAME': "pageTypeName",
+            'SALESCHANNEL': "salesChannel",
+            'ENVIRONMENT': "environment",
+        },
+        ('metrics',): {
+            'None': None,
+            'IMPRESSIONS': "impressions",
+            'CLICKS': "clicks",
+            'SPEND': "spend",
+            'ATTRIBUTEDSALES': "attributedSales",
+            'ATTRIBUTEDUNITS': "attributedUnits",
+            'ATTRIBUTEDORDERS': "attributedOrders",
+            'ASSISTEDSALES': "assistedSales",
+            'ASSISTEDUNITS': "assistedUnits",
+            'CTR': "ctr",
+            'CPC': "cpc",
+            'CPO': "cpo",
+            'CPM': "cpm",
+            'ROAS': "roas",
+            'UNIQUEVISITORS': "uniqueVisitors",
+            'FREQUENCY': "frequency",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -159,45 +163,45 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'start_date': (datetime,),  # noqa: E501
             'end_date': (datetime,),  # noqa: E501
-            'metrics': ([str], none_type,),  # noqa: E501
-            'dimensions': ([str], none_type,),  # noqa: E501
+            'ids': ([str], none_type,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
             'campaign_type': (str, none_type,),  # noqa: E501
             'sales_channel': (str, none_type,),  # noqa: E501
             'format': (str, none_type,),  # noqa: E501
             'report_type': (str, none_type,),  # noqa: E501
             'click_attribution_window': (str, none_type,),  # noqa: E501
             'view_attribution_window': (str, none_type,),  # noqa: E501
-            'ids': ([str], none_type,),  # noqa: E501
-            'id': (str, none_type,),  # noqa: E501
+            'dimensions': ([str], none_type,),  # noqa: E501
+            'metrics': ([str], none_type,),  # noqa: E501
             'timezone': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'start_date': 'startDate',  # noqa: E501
         'end_date': 'endDate',  # noqa: E501
-        'metrics': 'metrics',  # noqa: E501
-        'dimensions': 'dimensions',  # noqa: E501
+        'ids': 'ids',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'campaign_type': 'campaignType',  # noqa: E501
         'sales_channel': 'salesChannel',  # noqa: E501
         'format': 'format',  # noqa: E501
         'report_type': 'reportType',  # noqa: E501
         'click_attribution_window': 'clickAttributionWindow',  # noqa: E501
         'view_attribution_window': 'viewAttributionWindow',  # noqa: E501
-        'ids': 'ids',  # noqa: E501
-        'id': 'id',  # noqa: E501
+        'dimensions': 'dimensions',  # noqa: E501
+        'metrics': 'metrics',  # noqa: E501
         'timezone': 'timezone',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -238,24 +242,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
-            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            ids ([str], none_type): Campaign ids to report on. [optional]  # noqa: E501
+            id (str, none_type): Campaign id to report on. [optional]  # noqa: E501
             campaign_type (str, none_type): Filter the type of campaigns to report on: sponsoredProducts or onSiteDisplays. [optional]  # noqa: E501
             sales_channel (str, none_type): Filter on specific sales channel: offline or online. [optional]  # noqa: E501
             format (str, none_type): Format of the output. [optional] if omitted the server will use the default value of "json-compact"  # noqa: E501
             report_type (str, none_type): Type of report, if no dimensions/metrics are provided, falls back to summary reportType. [optional] if omitted the server will use the default value of "summary"  # noqa: E501
             click_attribution_window (str, none_type): Click attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             view_attribution_window (str, none_type): View attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
-            ids ([str], none_type): Ids to report on. [optional]  # noqa: E501
-            id (str, none_type): Id to report on. [optional]  # noqa: E501
+            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
             timezone (str, none_type): Time zone : see criteo developer portal for supported time zones. [optional] if omitted the server will use the default value of "UTC"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -340,24 +344,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
-            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            ids ([str], none_type): Campaign ids to report on. [optional]  # noqa: E501
+            id (str, none_type): Campaign id to report on. [optional]  # noqa: E501
             campaign_type (str, none_type): Filter the type of campaigns to report on: sponsoredProducts or onSiteDisplays. [optional]  # noqa: E501
             sales_channel (str, none_type): Filter on specific sales channel: offline or online. [optional]  # noqa: E501
             format (str, none_type): Format of the output. [optional] if omitted the server will use the default value of "json-compact"  # noqa: E501
             report_type (str, none_type): Type of report, if no dimensions/metrics are provided, falls back to summary reportType. [optional] if omitted the server will use the default value of "summary"  # noqa: E501
             click_attribution_window (str, none_type): Click attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             view_attribution_window (str, none_type): View attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
-            ids ([str], none_type): Ids to report on. [optional]  # noqa: E501
-            id (str, none_type): Id to report on. [optional]  # noqa: E501
+            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
             timezone (str, none_type): Time zone : see criteo developer portal for supported time zones. [optional] if omitted the server will use the default value of "UTC"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_campaigns_report_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_line_items_report.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_line_items_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,52 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('metrics',): {
-            'None': None,
-            'IMPRESSIONS': "impressions",
-            'CLICKS': "clicks",
-            'SPEND': "spend",
-            'ATTRIBUTEDSALES': "attributedSales",
-            'ATTRIBUTEDUNITS': "attributedUnits",
-            'ATTRIBUTEDORDERS': "attributedOrders",
-            'CTR': "ctr",
-            'CPC': "cpc",
-            'CPO': "cpo",
-            'ROAS': "roas",
-            'ASSISTEDUNITS': "assistedUnits",
-            'ASSISTEDSALES': "assistedSales",
-            'UNIQUEVISITORS': "uniqueVisitors",
-            'FREQUENCY': "frequency",
-        },
-        ('dimensions',): {
-            'None': None,
-            'DATE': "date",
-            'HOUR': "hour",
-            'CAMPAIGNID': "campaignId",
-            'CAMPAIGNNAME': "campaignName",
-            'CAMPAIGNTYPENAME': "campaignTypeName",
-            'ADVPRODUCTCATEGORY': "advProductCategory",
-            'ADVPRODUCTID': "advProductId",
-            'ADVPRODUCTNAME': "advProductName",
-            'BRANDID': "brandId",
-            'BRANDNAME': "brandName",
-            'LINEITEMID': "lineItemId",
-            'LINEITEMNAME': "lineItemName",
-            'RETAILERID': "retailerId",
-            'RETAILERNAME': "retailerName",
-            'KEYWORD': "keyword",
-            'PAGETYPENAME': "pageTypeName",
-            'SALESCHANNEL': "salesChannel",
-            'ENVIRONMENT': "environment",
-        },
         ('campaign_type',): {
             'None': None,
             'SPONSOREDPRODUCTS': "sponsoredProducts",
             'ONSITEDISPLAYS': "onSiteDisplays",
         },
         ('sales_channel',): {
             'None': None,
@@ -132,14 +94,55 @@
             'None': None,
             '1D': "1D",
             '7D': "7D",
             '14D': "14D",
             '30D': "30D",
             'NONE': "none",
         },
+        ('dimensions',): {
+            'None': None,
+            'DATE': "date",
+            'HOUR': "hour",
+            'ACCOUNTID': "accountId",
+            'ACCOUNTNAME': "accountName",
+            'CAMPAIGNID': "campaignId",
+            'CAMPAIGNNAME': "campaignName",
+            'CAMPAIGNTYPENAME': "campaignTypeName",
+            'ADVPRODUCTCATEGORY': "advProductCategory",
+            'ADVPRODUCTID': "advProductId",
+            'ADVPRODUCTNAME': "advProductName",
+            'BRANDID': "brandId",
+            'BRANDNAME': "brandName",
+            'LINEITEMID': "lineItemId",
+            'LINEITEMNAME': "lineItemName",
+            'RETAILERID': "retailerId",
+            'RETAILERNAME': "retailerName",
+            'KEYWORD': "keyword",
+            'PAGETYPENAME': "pageTypeName",
+            'SALESCHANNEL': "salesChannel",
+            'ENVIRONMENT': "environment",
+        },
+        ('metrics',): {
+            'None': None,
+            'IMPRESSIONS': "impressions",
+            'CLICKS': "clicks",
+            'SPEND': "spend",
+            'ATTRIBUTEDSALES': "attributedSales",
+            'ATTRIBUTEDUNITS': "attributedUnits",
+            'ATTRIBUTEDORDERS': "attributedOrders",
+            'ASSISTEDSALES': "assistedSales",
+            'ASSISTEDUNITS': "assistedUnits",
+            'CTR': "ctr",
+            'CPC': "cpc",
+            'CPO': "cpo",
+            'CPM': "cpm",
+            'ROAS': "roas",
+            'UNIQUEVISITORS': "uniqueVisitors",
+            'FREQUENCY': "frequency",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -160,45 +163,45 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'start_date': (datetime,),  # noqa: E501
             'end_date': (datetime,),  # noqa: E501
-            'metrics': ([str], none_type,),  # noqa: E501
-            'dimensions': ([str], none_type,),  # noqa: E501
+            'ids': ([str], none_type,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
             'campaign_type': (str, none_type,),  # noqa: E501
             'sales_channel': (str, none_type,),  # noqa: E501
             'format': (str, none_type,),  # noqa: E501
             'report_type': (str, none_type,),  # noqa: E501
             'click_attribution_window': (str, none_type,),  # noqa: E501
             'view_attribution_window': (str, none_type,),  # noqa: E501
-            'ids': ([str], none_type,),  # noqa: E501
-            'id': (str, none_type,),  # noqa: E501
+            'dimensions': ([str], none_type,),  # noqa: E501
+            'metrics': ([str], none_type,),  # noqa: E501
             'timezone': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'start_date': 'startDate',  # noqa: E501
         'end_date': 'endDate',  # noqa: E501
-        'metrics': 'metrics',  # noqa: E501
-        'dimensions': 'dimensions',  # noqa: E501
+        'ids': 'ids',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'campaign_type': 'campaignType',  # noqa: E501
         'sales_channel': 'salesChannel',  # noqa: E501
         'format': 'format',  # noqa: E501
         'report_type': 'reportType',  # noqa: E501
         'click_attribution_window': 'clickAttributionWindow',  # noqa: E501
         'view_attribution_window': 'viewAttributionWindow',  # noqa: E501
-        'ids': 'ids',  # noqa: E501
-        'id': 'id',  # noqa: E501
+        'dimensions': 'dimensions',  # noqa: E501
+        'metrics': 'metrics',  # noqa: E501
         'timezone': 'timezone',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -239,24 +242,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
-            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            ids ([str], none_type): Line Item ids to report on. [optional]  # noqa: E501
+            id (str, none_type): Line Item id to report on. [optional]  # noqa: E501
             campaign_type (str, none_type): Filter the type of campaigns to report on: sponsoredProducts or onSiteDisplays. [optional]  # noqa: E501
             sales_channel (str, none_type): Filter on specific sales channel: offline or online. [optional]  # noqa: E501
             format (str, none_type): Format of the output. [optional] if omitted the server will use the default value of "json-compact"  # noqa: E501
             report_type (str, none_type): Type of report, if no dimensions/metrics are provided, falls back to summary reportType. [optional] if omitted the server will use the default value of "summary"  # noqa: E501
             click_attribution_window (str, none_type): Click attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             view_attribution_window (str, none_type): View attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
-            ids ([str], none_type): Ids to report on. [optional]  # noqa: E501
-            id (str, none_type): Id to report on. [optional]  # noqa: E501
+            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
             timezone (str, none_type): Time zone : see criteo developer portal for supported time zones. [optional] if omitted the server will use the default value of "UTC"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -341,24 +344,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
-            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            ids ([str], none_type): Line Item ids to report on. [optional]  # noqa: E501
+            id (str, none_type): Line Item id to report on. [optional]  # noqa: E501
             campaign_type (str, none_type): Filter the type of campaigns to report on: sponsoredProducts or onSiteDisplays. [optional]  # noqa: E501
             sales_channel (str, none_type): Filter on specific sales channel: offline or online. [optional]  # noqa: E501
             format (str, none_type): Format of the output. [optional] if omitted the server will use the default value of "json-compact"  # noqa: E501
             report_type (str, none_type): Type of report, if no dimensions/metrics are provided, falls back to summary reportType. [optional] if omitted the server will use the default value of "summary"  # noqa: E501
             click_attribution_window (str, none_type): Click attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             view_attribution_window (str, none_type): View attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
-            ids ([str], none_type): Ids to report on. [optional]  # noqa: E501
-            id (str, none_type): Id to report on. [optional]  # noqa: E501
+            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
             timezone (str, none_type): Time zone : see criteo developer portal for supported time zones. [optional] if omitted the server will use the default value of "UTC"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_line_items_report_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_line_items_report_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_line_items_report_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_line_items_report_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_report_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_report_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_revenue_report.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_revenue_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,46 +64,14 @@
             'BRAND': "brand",
         },
         ('revenue_type',): {
             'None': None,
             'AUCTION': "auction",
             'PREFERRED': "preferred",
         },
-        ('metrics',): {
-            'None': None,
-            'CLICKS': "clicks",
-            'SPEND': "spend",
-            'ATTRIBUTEDORDERS': "attributedOrders",
-            'ATTRIBUTEDSALES': "attributedSales",
-            'ATTRIBUTEDUNITS': "attributedUnits",
-            'CPC': "cpc",
-            'CPO': "cpo",
-            'ROAS': "roas",
-            'OPENAUCTIONREVENUE': "openAuctionRevenue",
-            'PREFERREDDEALSREVENUE': "preferredDealsRevenue",
-            'AVGCPC': "avgCpc",
-            'AVGCPM': "avgCpm",
-        },
-        ('dimensions',): {
-            'None': None,
-            'DATE': "date",
-            'CAMPAIGNID': "campaignId",
-            'CAMPAIGNNAME': "campaignName",
-            'ACCOUNTID': "accountId",
-            'ACCOUNTNAME': "accountName",
-            'ENVIRONMENT': "environment",
-            'ADVPRODUCTCATEGORY': "advProductCategory",
-            'BRANDID': "brandId",
-            'BRANDNAME': "brandName",
-            'PAGETYPENAME': "pageTypeName",
-            'ADVPRODUCTNAME': "advProductName",
-            'ADVPRODUCTGTIN': "advProductGtin",
-            'ADVPRODUCTMPN': "advProductMpn",
-            'ADVPRODUCTID': "advProductId",
-        },
         ('format',): {
             'None': None,
             'JSON': "json",
             'JSON-COMPACT': "json-compact",
             'JSON-NEWLINE': "json-newline",
             'CSV': "csv",
         },
@@ -139,14 +107,45 @@
             'ONSITEDISPLAYS': "onSiteDisplays",
         },
         ('sales_channel',): {
             'None': None,
             'OFFLINE': "offline",
             'ONLINE': "online",
         },
+        ('dimensions',): {
+            'None': None,
+            'DATE': "date",
+            'CAMPAIGNID': "campaignId",
+            'CAMPAIGNNAME': "campaignName",
+            'ACCOUNTID': "accountId",
+            'ACCOUNTNAME': "accountName",
+            'ENVIRONMENT': "environment",
+            'ADVPRODUCTCATEGORY': "advProductCategory",
+            'BRANDID': "brandId",
+            'BRANDNAME': "brandName",
+            'PAGETYPENAME': "pageTypeName",
+            'ADVPRODUCTNAME': "advProductName",
+            'ADVPRODUCTGTIN': "advProductGtin",
+            'ADVPRODUCTMPN': "advProductMpn",
+            'ADVPRODUCTID': "advProductId",
+        },
+        ('metrics',): {
+            'None': None,
+            'IMPRESSIONS': "impressions",
+            'CLICKS': "clicks",
+            'SPEND': "spend",
+            'SALES': "sales",
+            'UNITS': "units",
+            'CPO': "cpo",
+            'ROAS': "roas",
+            'OPENAUCTIONREVENUE': "openAuctionRevenue",
+            'PREFERREDDEALSREVENUE': "preferredDealsRevenue",
+            'AVGCPC': "avgCpc",
+            'AVGCPM': "avgCpm",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -167,51 +166,51 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'start_date': (datetime,),  # noqa: E501
             'end_date': (datetime,),  # noqa: E501
-            'report_type': (str, none_type,),  # noqa: E501
-            'revenue_type': (str, none_type,),  # noqa: E501
             'ids': ([str], none_type,),  # noqa: E501
             'id': (str, none_type,),  # noqa: E501
-            'metrics': ([str], none_type,),  # noqa: E501
-            'dimensions': ([str], none_type,),  # noqa: E501
+            'report_type': (str, none_type,),  # noqa: E501
+            'revenue_type': (str, none_type,),  # noqa: E501
             'format': (str, none_type,),  # noqa: E501
             'sold_by': (str, none_type,),  # noqa: E501
             'campaign_sub_type': (str, none_type,),  # noqa: E501
             'click_attribution_window': (str, none_type,),  # noqa: E501
             'view_attribution_window': (str, none_type,),  # noqa: E501
             'campaign_type': (str, none_type,),  # noqa: E501
             'sales_channel': (str, none_type,),  # noqa: E501
+            'dimensions': ([str], none_type,),  # noqa: E501
+            'metrics': ([str], none_type,),  # noqa: E501
             'timezone': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'start_date': 'startDate',  # noqa: E501
         'end_date': 'endDate',  # noqa: E501
-        'report_type': 'reportType',  # noqa: E501
-        'revenue_type': 'revenueType',  # noqa: E501
         'ids': 'ids',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'metrics': 'metrics',  # noqa: E501
-        'dimensions': 'dimensions',  # noqa: E501
+        'report_type': 'reportType',  # noqa: E501
+        'revenue_type': 'revenueType',  # noqa: E501
         'format': 'format',  # noqa: E501
         'sold_by': 'soldBy',  # noqa: E501
         'campaign_sub_type': 'campaignSubType',  # noqa: E501
         'click_attribution_window': 'clickAttributionWindow',  # noqa: E501
         'view_attribution_window': 'viewAttributionWindow',  # noqa: E501
         'campaign_type': 'campaignType',  # noqa: E501
         'sales_channel': 'salesChannel',  # noqa: E501
+        'dimensions': 'dimensions',  # noqa: E501
+        'metrics': 'metrics',  # noqa: E501
         'timezone': 'timezone',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -252,27 +251,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            ids ([str], none_type): Campaign ids to report on. [optional]  # noqa: E501
+            id (str, none_type): Campaign id to report on. [optional]  # noqa: E501
             report_type (str, none_type): Type of report. [optional]  # noqa: E501
             revenue_type (str, none_type): Type of revenue. [optional]  # noqa: E501
-            ids ([str], none_type): List of campaign Ids to filter. [optional]  # noqa: E501
-            id (str, none_type): List of campaign Id to filter. [optional]  # noqa: E501
-            metrics ([str], none_type): List of Metrics to report on. [optional]  # noqa: E501
-            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
             format (str, none_type): Format of the output. [optional]  # noqa: E501
             sold_by (str, none_type): Filter on the seller: indirect, direct or private market. [optional]  # noqa: E501
             campaign_sub_type (str, none_type): Filter on campaign subType : Auction and Preferred Deals or Lockout campaign. [optional]  # noqa: E501
             click_attribution_window (str, none_type): Click attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             view_attribution_window (str, none_type): View attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             campaign_type (str, none_type): Filter the type of campaigns to report on: sponsoredProducts or onSiteDisplays. [optional]  # noqa: E501
             sales_channel (str, none_type): Filter on specific sales channel: offline or online. [optional]  # noqa: E501
+            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
             timezone (str, none_type): Time zone : see criteo developer portal for supported time zones. [optional] if omitted the server will use the default value of "UTC"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -357,27 +356,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            ids ([str], none_type): Campaign ids to report on. [optional]  # noqa: E501
+            id (str, none_type): Campaign id to report on. [optional]  # noqa: E501
             report_type (str, none_type): Type of report. [optional]  # noqa: E501
             revenue_type (str, none_type): Type of revenue. [optional]  # noqa: E501
-            ids ([str], none_type): List of campaign Ids to filter. [optional]  # noqa: E501
-            id (str, none_type): List of campaign Id to filter. [optional]  # noqa: E501
-            metrics ([str], none_type): List of Metrics to report on. [optional]  # noqa: E501
-            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
             format (str, none_type): Format of the output. [optional]  # noqa: E501
             sold_by (str, none_type): Filter on the seller: indirect, direct or private market. [optional]  # noqa: E501
             campaign_sub_type (str, none_type): Filter on campaign subType : Auction and Preferred Deals or Lockout campaign. [optional]  # noqa: E501
             click_attribution_window (str, none_type): Click attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             view_attribution_window (str, none_type): View attribution window. [optional] if omitted the server will use the default value of "none"  # noqa: E501
             campaign_type (str, none_type): Filter the type of campaigns to report on: sponsoredProducts or onSiteDisplays. [optional]  # noqa: E501
             sales_channel (str, none_type): Filter on specific sales channel: offline or online. [optional]  # noqa: E501
+            dimensions ([str], none_type): List of dimensions to report on. [optional]  # noqa: E501
+            metrics ([str], none_type): List of metrics to report on. [optional]  # noqa: E501
             timezone (str, none_type): Time zone : see criteo developer portal for supported time zones. [optional] if omitted the server will use the default value of "UTC"  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_revenue_report_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_revenue_report_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/async_revenue_report_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/async_revenue_report_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_create_model_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_create_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/auction_line_item_update_model_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/auction_line_item_update_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/audience_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/audience_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/audience_target202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/audience_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/audience_target202110_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/audience_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_list_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_campaign202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/balance_response_paged_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/balance_response_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_attributes_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_daily_budget_override.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_daily_budget_override.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_monthly_budget_override.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_monthly_budget_override.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/category202204.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/category202204.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/category202204_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/category202204_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/change_dates_of_balance_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/change_dates_of_balance_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/choice_option.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/choice_option.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/choice_variable_specification.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/choice_variable_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/choice_variable_value.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/choice_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/color_variable_value.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/color_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_error.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_line_item_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_line_item_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_line_item_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_problem.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_problem.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/common_warning.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/common_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/create_balance_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/create_balance_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202110_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202110_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202210.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202210.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202210_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202210_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative202210_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative202210_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative_create_model202207.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative_create_model202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/creative_update_model202207.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/creative_update_model202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/daily_line_item_budget_override.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/daily_line_item_budget_override.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/editable_campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/editable_campaign_attributes_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_account.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_add_funds_to_balance.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_add_funds_to_balance.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_add_to_basket_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_auction_line_item.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_auction_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_create_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_auction_line_item_update_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_audience_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_audience_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_audience_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_balance_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_balance_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_brand.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_catalog_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_catalog_status.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_change_dates_of_balance.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_change_dates_of_balance.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_common_line_item.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_common_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_create_balance.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_create_balance.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_keyword_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_line_item_capping202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_line_item_capping202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_line_item_page202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_line_item_page202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_line_item_page_category202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_line_item_page_category202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_create_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_preferred_line_item_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_promoted_product202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_retailer.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_retailer_pages202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_retailer_pages202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_store_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_store_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_store_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/external_update_balance_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/external_update_balance_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/files_variable_value.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/files_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/files_variables_specification.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/files_variables_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/hyperlink_variable_value.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/hyperlink_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/input_resource_of_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/input_resource_of_auction_line_item_create_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/input_resource_of_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/input_resource_of_preferred_line_item_create_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_account_and_account.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_account_and_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_brand_and_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_account.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_brand.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_retailer.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_page_response_of_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_request_of_catalog_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_request_of_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_catalog_status.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/json_api_single_response_of_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/keyword_target202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/keyword_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/keyword_target202110_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/keyword_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_bid_multipliers_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/line_item_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/line_item_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/monthly_line_item_budeget_override.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/monthly_line_item_budeget_override.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/page_metadata.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/page_metadata.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/page_type_environment.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/page_type_environment.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/post_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/post_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item_create_model202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item_create_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/preferred_line_item_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/preferred_line_item_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/problem_details.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/promoted_product202110_list_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/promoted_product202110_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/promoted_product202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/promoted_product202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/put_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/put_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/report_outcome.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/report_outcome.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_add_funds_to_balance.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_add_funds_to_balance.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_auction_line_item_update_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_balance_campaign202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_balance_campaign202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_balance_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_balance_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_category202204.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_category202204.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_change_dates_of_balance.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_change_dates_of_balance.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_common_line_item.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_common_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_create_balance.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_create_balance.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_creative202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_creative202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_creative202210.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_creative202210.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_preferred_line_item_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_promoted_product202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_template.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_template.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/resource_of_update_balance_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/resource_of_update_balance_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keyword_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keyword_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_add_remove_keywords_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_input_keywords_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_input_keywords_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keyword_data_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keyword_data_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_keywords_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_problem_details.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_proposal_status_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_resource_outcome.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_resource_outcome.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bid_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bid_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/retail_media_externalv1_set_bids_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v1_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_entity_v2_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v1.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v2.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_create_input_entity_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v1_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_get_entity_v2_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_create_v2.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_create_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_details_v2.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_audience_user_behavior_details_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_customer_list.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_customer_list.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_create_v2.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_create_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v1.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v1.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v2.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/rm_legacy_segment_user_behavior_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/section.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/section.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/status_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/status_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/status_response_resource.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/status_response_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/store_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/store_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/store_target202110_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/store_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/store_target202110_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/store_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_list_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_response.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_variable.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_variable.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/template_variable_value.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/template_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/text_variable_specification.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/text_variable_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/text_variable_value.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/text_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/update_balance_model_request.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/update_balance_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_campaign_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_campaign_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_line_item_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_input_of_line_item_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_of_campaign_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_of_campaign_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_of_line_item_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_of_line_item_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_campaign_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_campaign_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_line_item_budget_overrides.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_resource_outcome_of_line_item_budget_overrides.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_add_to_basket_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_audience_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_keyword_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_target202110.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model/value_type_resource_of_store_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/model_utils.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/model_utils.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/models/__init__.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/models/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/criteo_api_retailmedia_v2024_01/rest.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/criteo_api_retailmedia_v2024_01/rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/setup.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-retailmedia-sdk"
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
-pip install criteo-api-retailmedia-sdk==2024.01.0.240207
+pip install criteo-api-retailmedia-sdk==2024.01.0.240404
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240207`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2024.01.0.240404`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2024_01
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2024.1.0.240207/test/test_gateway_api.py` & `criteo-api-retailmedia-sdk-2024.1.0.240404/test/test_gateway_api.py`

 * *Files identical despite different names*

